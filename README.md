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
| 2022-08-26 19:11:18 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 18:17:05 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 17:17:57 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 16:19:20 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 15:16:20 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 14:12:07 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 13:32:37 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 12:28:23 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 11:12:00 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 10:15:23 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 09:13:27 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 08:18:17 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 07:18:58 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 06:34:20 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 05:56:16 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-26 04:14:14 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 23:25:02 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 22:14:11 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 21:12:37 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 20:15:06 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 19:11:31 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 18:16:30 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 17:17:04 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 16:17:58 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 15:14:29 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 14:12:46 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 13:37:15 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 12:28:37 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 11:13:08 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 10:15:42 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 09:13:30 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 08:19:19 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 07:18:36 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 06:28:09 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 05:51:13 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 04:07:15 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-25 01:24:51 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 23:14:26 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 22:13:33 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 21:12:14 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 20:14:23 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 19:12:34 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 18:25:53 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 17:15:49 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 16:18:41 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 15:14:25 | v0.9.28 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 14:12:33 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 13:32:09 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 12:27:40 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 11:12:08 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 10:15:45 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 09:13:19 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 08:17:04 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 07:12:39 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 06:18:53 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 05:40:25 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 04:04:23 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-24 01:21:13 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 23:13:43 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 22:13:12 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 21:12:13 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 20:14:27 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 19:11:21 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 18:16:38 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 17:17:17 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 16:18:42 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 15:13:48 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 14:12:46 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 13:34:29 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 12:27:11 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 11:11:58 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 10:15:35 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 09:13:33 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 08:17:45 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 07:17:08 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 06:27:01 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 05:51:13 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 04:11:35 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-23 01:27:16 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 23:13:26 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 22:14:11 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 21:12:12 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 20:13:38 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 19:11:22 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 18:15:53 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 17:15:52 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 16:17:33 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 15:16:03 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 14:11:54 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 13:37:43 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 12:29:26 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 11:11:43 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 10:15:55 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 09:13:17 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 08:17:29 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 07:12:06 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 06:20:30 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 05:08:05 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 03:56:25 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-22 01:14:28 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 23:12:57 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 22:13:04 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 21:11:44 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 20:14:07 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 19:11:03 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 18:16:11 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 17:14:25 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 16:17:46 | null | v | UPDATE! | v | UPDATE! | null | null
| 2022-08-21 15:12:58 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 14:11:32 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 13:24:41 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 12:22:52 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 11:11:25 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 10:13:59 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 09:12:48 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 08:16:36 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 07:12:17 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 06:16:31 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 05:15:51 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 04:29:01 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 03:37:54 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-21 01:11:59 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 23:12:31 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 22:13:00 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 21:12:00 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 20:13:51 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 19:11:02 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 18:15:26 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 17:13:49 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 16:16:59 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 15:13:22 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 14:11:50 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 13:24:19 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 12:23:21 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 11:11:23 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 10:13:57 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 09:12:49 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 08:17:29 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 07:12:27 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 06:16:12 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 05:15:22 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 04:28:42 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 03:34:53 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-20 01:13:49 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 23:13:18 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 22:14:34 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 21:12:09 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 20:15:25 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 19:10:48 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 18:18:40 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 17:21:50 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 16:20:31 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 15:15:52 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 14:13:03 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 13:36:04 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 12:26:14 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 11:12:08 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 10:17:02 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 09:13:52 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 08:17:01 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 07:12:45 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 06:19:23 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 05:23:49 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 04:46:35 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 03:46:59 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-19 01:17:21 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 23:14:01 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 22:13:49 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 21:12:48 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 20:16:00 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 19:11:43 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 18:15:48 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 17:32:19 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 15:22:59 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 14:15:26 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 13:37:50 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 12:29:15 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 11:11:51 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 10:16:57 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 09:14:35 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 08:16:39 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 07:12:44 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 06:17:34 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 05:02:53 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 03:58:13 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-18 01:23:18 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-17 23:14:24 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-17 22:12:51 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-17 21:12:07 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-17 20:14:18 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-17 19:10:40 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-17 15:15:21 | v0.9.27 | v | UPDATE! | v0.9.27 | OK! | false | false
| 2022-08-17 10:15:34 | v0.9.27 | v | UPDATE! | v0.9.27 | OK! | false | false
| 2022-08-15 15:15:51 | v0.9.27 | v | UPDATE! | v0.9.27 | OK! | false | false
| 2022-08-13 11:11:12 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-12 15:15:26 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-11 17:16:39 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-09 03:40:39 | v0.9.27 | v | UPDATE! | v0.9.27 | OK! | false | false
| 2022-08-08 23:15:23 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-08 08:20:20 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-08 06:18:55 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-07 03:20:24 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-06 18:15:55 | v0.9.27 | v | UPDATE! | v0.9.27 | OK! | false | false
| 2022-08-06 06:16:15 | v0.9.27 | v | UPDATE! | v0.9.27 | OK! | false | false
| 2022-08-05 16:20:28 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-05 13:38:20 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-05 05:29:22 | v0.9.27 | v | UPDATE! | v0.9.27 | OK! | false | false
| 2022-08-05 03:40:23 | v0.9.27 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-04 06:18:52 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-04 05:26:38 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-04 04:39:11 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-04 03:23:09 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-04 01:19:57 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-03 23:14:15 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-03 22:13:00 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-03 21:12:37 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-03 20:14:47 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-03 19:11:01 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-03 18:17:27 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-03 17:16:21 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-03 16:19:13 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-03 15:15:49 | v0.9.27 | v0.9.26 | UPDATE! | v | UPDATE! | false | false
| 2022-08-03 14:12:16 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-03 13:36:41 | v0.9.27 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-03 05:43:21 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-03 01:21:20 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-08-02 19:10:54 | v0.9.25 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-02 18:16:47 | v0.9.25 | v0.9.26 | UPDATE! | v0.9.26 | UPDATE! | false | false
| 2022-08-02 11:11:36 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-08-02 07:14:17 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-08-02 04:01:06 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-01 23:16:00 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-08-01 17:23:00 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-01 12:29:38 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-08-01 10:16:05 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-31 05:15:24 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-31 03:40:30 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-30 21:11:14 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-30 18:15:22 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-30 03:45:13 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-30 01:10:25 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-29 20:14:22 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-29 18:17:22 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-29 16:20:43 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-29 10:15:27 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-29 05:25:27 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-29 01:16:18 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-28 23:15:27 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-28 19:10:36 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-28 16:21:10 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-28 13:38:05 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-28 12:31:09 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-28 10:15:24 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-28 07:12:37 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-27 17:23:13 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-27 15:15:44 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-27 13:41:02 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-27 05:29:46 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-26 15:15:46 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-26 05:37:00 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-25 21:12:09 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-25 18:17:04 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-25 17:20:48 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-25 12:29:31 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-25 05:24:17 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-25 04:44:19 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-24 18:16:36 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-24 04:29:06 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-24 01:20:37 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-23 18:15:46 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-23 17:15:47 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-23 16:18:00 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-23 05:15:23 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-22 17:23:50 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-22 04:40:33 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-21 15:15:28 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-21 05:25:26 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-21 03:37:40 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-20 17:20:31 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-19 19:10:36 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-19 15:15:22 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-19 12:29:35 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-19 10:15:44 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-18 17:21:36 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-18 16:20:39 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-18 13:40:59 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-18 01:12:59 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-17 19:10:49 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-15 19:10:52 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-15 16:20:45 | v0.9.26 | v | UPDATE! | v0.9.26 | OK! | false | false
| 2022-07-14 19:11:07 | v0.9.26 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-14 16:23:28 | v0.9.26 | v0.9.25 | UPDATE! | v0.9.25 | UPDATE! | false | false
| 2022-07-14 09:14:20 | v0.9.25 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-14 04:45:31 | v0.9.25 | v | UPDATE! | v0.9.25 | OK! | false | false
| 2022-07-13 17:20:41 | v0.9.25 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-12 13:35:20 | v0.9.25 | v | UPDATE! | v0.9.25 | OK! | false | false
| 2022-07-12 12:30:48 | v0.9.25 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-12 03:55:21 | v0.9.25 | v | UPDATE! | v0.9.25 | OK! | false | false
| 2022-07-11 16:20:39 | v0.9.25 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-11 11:20:53 | v0.9.25 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-11 03:29:50 | v0.9.25 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-11 01:15:27 | v0.9.25 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-10 18:15:38 | v0.9.25 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-10 08:15:33 | v0.9.25 | v | UPDATE! | v0.9.25 | OK! | false | false
| 2022-07-09 18:15:16 | v0.9.25 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-09 01:03:35 | v0.9.25 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-08 18:17:01 | v0.9.25 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-07 19:10:35 | v0.9.25 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-05 15:14:22 | v0.9.25 | v | UPDATE! | v0.9.24 | UPDATE! | false | false
| 2022-07-05 13:39:42 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-03 19:10:23 | v0.9.24 | v | UPDATE! | v0.9.24 | OK! | false | false
| 2022-07-03 08:15:17 | v0.9.24 | v | UPDATE! | v0.9.24 | OK! | false | false
| 2022-07-02 22:12:44 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-02 19:10:19 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-02 13:21:07 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-01 20:14:40 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-07-01 15:15:22 | v0.9.24 | v | UPDATE! | v0.9.24 | OK! | false | false
| 2022-07-01 05:30:28 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-06-30 11:11:30 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-06-29 22:12:59 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-06-29 16:38:36 | v0.9.24 | v | UPDATE! | v0.9.24 | OK! | false | false
| 2022-06-28 21:10:31 | v0.9.24 | v | UPDATE! | v0.9.24 | OK! | false | false
| 2022-06-28 19:10:27 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-06-27 12:28:40 | v0.9.24 | v | UPDATE! | v0.9.24 | OK! | false | false
| 2022-06-24 15:15:20 | v0.9.24 | v | UPDATE! | v0.9.24 | OK! | false | false
| 2022-06-23 15:15:23 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-06-22 08:20:14 | v0.9.24 | v | UPDATE! | v0.9.24 | OK! | false | false
| 2022-06-21 07:12:05 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-06-21 06:16:52 | v0.9.24 | v | UPDATE! | v0.9.24 | OK! | false | false
| 2022-06-19 08:15:12 | v0.9.24 | v | UPDATE! | v0.9.24 | OK! | false | false
| 2022-06-17 17:15:09 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-06-17 16:19:32 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-06-17 06:17:11 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-06-17 05:14:55 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-17 04:27:17 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-17 03:21:09 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-17 01:03:48 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 23:13:33 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 22:17:25 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 21:11:40 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 20:13:31 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 19:09:29 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 18:16:53 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 17:18:38 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 16:20:21 | v0.9.24 | v | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 15:12:59 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 14:11:39 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 13:31:45 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 12:26:29 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 11:10:35 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 10:14:07 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 09:13:12 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 08:18:50 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 07:12:57 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 06:15:49 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 05:15:29 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 04:28:28 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-16 03:20:19 | v0.9.24 | v0.9.23 | UPDATE! | v | UPDATE! | false | false
| 2022-06-16 01:08:54 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-15 23:13:45 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-15 22:13:21 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-15 21:11:21 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-15 20:13:48 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-15 19:11:23 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-15 18:15:22 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-15 17:15:23 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-15 16:17:33 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-15 15:13:46 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-15 14:11:40 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-15 13:32:24 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-15 12:25:22 | v0.9.24 | v | UPDATE! | v | UPDATE! | false | false
| 2022-06-15 11:11:53 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-15 10:14:36 | v0.9.24 | v0.9.23 | UPDATE! | v0.9.23 | UPDATE! | false | false
| 2022-06-13 16:17:44 | v0.9.23 | v | UPDATE! | v | UPDATE! | false | false
| 2022-06-12 08:15:12 | v0.9.23 | v | UPDATE! | v0.9.23 | OK! | false | false
| 2022-06-08 17:15:22 | v0.9.23 | v | UPDATE! | v0.9.23 | OK! | false | false
| 2022-06-04 06:15:17 | v0.9.23 | v | UPDATE! | v | UPDATE! | false | false
| 2022-06-03 01:00:21 | v0.9.23 | v | UPDATE! | v | UPDATE! | false | false
| 2022-06-02 14:17:17 | v0.9.23 | v | UPDATE! | v | UPDATE! | false | false
| 2022-06-01 16:20:21 | v0.9.23 | v0.9.22 | UPDATE! | v0.9.22 | UPDATE! | false | false
| 2022-06-01 15:16:08 | v0.9.23 | v0.9.22 | UPDATE! | v0.9.22 | UPDATE! | false | false
| 2022-06-01 14:20:29 | v0.9.23 | v0.9.22 | UPDATE! | v0.9.22 | UPDATE! | false | false
| 2022-05-31 09:13:51 | v0.9.22 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-30 20:15:15 | v0.9.22 | v | UPDATE! | v0.9.22 | OK! | false | false
| 2022-05-30 17:20:14 | v0.9.22 | v | UPDATE! | v0.9.22 | OK! | false | false
| 2022-05-30 15:16:29 | v0.9.22 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-23 08:18:08 | v0.9.22 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-23 07:15:25 | v0.9.22 | v | UPDATE! | v0.9.22 | OK! | false | false
| 2022-05-22 10:15:14 | v0.9.22 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-22 01:05:23 | v0.9.22 | v | UPDATE! | v0.9.22 | OK! | false | false
| 2022-05-21 18:15:43 | v0.9.22 | v | UPDATE! | v0.9.22 | OK! | false | false
| 2022-05-21 12:23:35 | v0.9.22 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-20 15:15:16 | v0.9.22 | v | UPDATE! | v0.9.22 | OK! | false | false
| 2022-05-20 14:12:48 | v0.9.22 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-19 15:20:30 | v0.9.22 | v | UPDATE! | v0.9.22 | OK! | false | false
| 2022-05-19 06:18:00 | v0.9.22 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-18 19:11:42 | v0.9.22 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-18 18:17:00 | v0.9.22 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-18 16:19:20 | v0.9.22 | v0.9.21 | UPDATE! | v0.9.21 | UPDATE! | false | false
| 2022-05-18 10:15:27 | v0.9.21 | v | UPDATE! | v0.9.21 | OK! | false | false
| 2022-05-18 08:17:24 | v0.9.21 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-18 05:18:25 | v0.9.21 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-17 21:10:42 | v0.9.21 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-17 19:09:56 | v0.9.21 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-17 15:14:40 | v0.9.21 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-16 22:13:42 | v0.9.21 | v | UPDATE! | v0.9.21 | OK! | false | false
| 2022-05-16 02:58:22 | v0.9.21 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-14 08:16:59 | v0.9.21 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-14 05:29:04 | v0.9.21 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-13 16:20:15 | v0.9.21 | v | UPDATE! | v0.9.21 | OK! | false | false
| 2022-05-13 05:37:46 | v0.9.21 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-12 16:20:41 | v0.9.21 | v | UPDATE! | v0.9.21 | OK! | false | false
| 2022-05-10 01:00:46 | v0.9.21 | v | UPDATE! | v | UPDATE! | false | false
| 2022-05-09 16:21:25 | v0.9.21 | v0.9.20 | UPDATE! | v0.9.21 | OK! | false | false
| 2022-05-09 01:05:21 | v0.9.20 | v | UPDATE! | v0.9.20 | OK! | false | false
| 2022-05-08 18:15:25 | v0.9.20 | v | UPDATE! | v0.9.20 | OK! | false | false
| 2022-05-07 01:00:57 | v0.9.20 | v | UPDATE! | v0.9.20 | OK! | false | false
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
