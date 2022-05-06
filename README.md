# take-actions
Github actions to check if you need to take actions and update Polkadot to it's latest release. 
Based on GitHUB API v4, the action will check Polkadot git repository for tags: Version, Draft, Prerelease and will compare it with the 1KV Validators version. 

If each of the conditions DRAFT, PRERELEASE, VERSION pass it's check the README file will be updated and commited at: 
```
-- name: Update the README file
if: steps.versions.outputs.tag != steps.versions.outputs...*
```
#### How we are doing today... any UPDATES?
| Date | Polkadot | NodeA | Action | NodeB | Action | IsDraft | IsPrerelease
:--- | :--- | :--- | :--- | :--- | :--- | :--- | :---
| 2022-05-06 01:00:46 | v0.9.20 | v | UPDATE! | v0.9.20 | OK! | false | false
| 2022-04-28 00:20:54 | v0.9.19 | v0.9.18 | UPDATE! | v0.9.19 | OK! | false | false

Take a look at the actions file: [Git Actions] and change the addresses for the validators you need to monitor.

![polkadot](https://github.com/ksmnetwork/take-actions/actions/workflows/polkadot-versions-check.yml/badge.svg)

#### Prerequisites if you want to add SMS notification on release:
- A Twilio Account. [Sign up for free]
- A [Twilio API Key and Secret]
- https://github.com/twilio-labs/actions-sms

Add to [Git Actions]
```
      - name: 'Sending SMS Notification'
        if: steps.versions.outputs.tag != steps.versions.outputs.v1version && steps.versions.outputs.tag != steps.versions.outputs.v21version && steps.versions.outputs.draft != true && steps.versions.outputs.prerelease != true
        uses: twilio-labs/actions-sms@v1
        with:
          fromPhoneNumber: ${{ secrets.FROM_PHONE }}
          toPhoneNumber: ${{ secrets.TO_PHONE }}
          message: 'Polkadot has new version: ${{ steps.versions.outputs.tag }}'
        env:
          TWILIO_ACCOUNT_SID: ${{ secrets.TWILIO_ACCOUNT_SID }}
          TWILIO_API_KEY: ${{ secrets.TWILIO_API_KEY }}
          TWILIO_API_SECRET: ${{ secrets.TWILIO_API_SECRET }}
```
Validators aresses are set at:
```
echo ::set-output name=v1version::
```

and 

```
echo ::set-output name=v2version::
```

To dispatch the workflow manually:
```
on:
  workflow_dispatch
```

### Action scheduling 
November 1, 2019 GitHub Actions—scheduled jobs maximum frequency is changing.

In order to provide a more reliable experience, we’ve set the minimum time period for scheduled runs to 5 minutes. A schedule of * * * * * which would previously run every minute will now run every five minutes.

if you want to use:
```
on:
  schedule:
    - cron:  '* * * * *'
```

### For Support && Nominations #
* Display name for Validators. KSMNETWORK && KSMNETWORK-WEST 
* Riot @gtoocool:matrix.org

* KUSAMA (KSM) Address
```H1bSKJxoxzxYRCdGQutVqFGeW7xU3AcN6vyEdZBU7Qb1rsZ```
* **URL for nomination at PolkadotJS: [KSMNETWORK]**

* PolkaDOT (DOT) Address:
```15FxvBFDd3X7H9qcMGqsiuvFYEg4D3mBoTA2LQufreysTHKA```
* **URL for nomination at PolkadotJS: [KSMNETWORK-WEST]**

[Git Actions]: https://github.com/ksmnetwork/take-actions/blob/main/.github/workflows/polkadot-versions-check.yml
[KSMNETWORK]: https://polkadot.js.org/apps/#/staking?filter=KSMNETWORK&rpc=wss://kusama.api.onfinality.io/public-ws
[KSMNETWORK-WEST]: https://polkadot.js.org/apps/#/staking?filter=KSMNETWORK-WEST&rpc=wss://kusama.api.onfinality.io/public-ws
[Sign up for free]: https://www.twilio.com/try-twilio
[Twilio API Key and Secret]: https://www.twilio.com/docs/iam/keys/api-key
