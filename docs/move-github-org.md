# Moving LoopBack repos to new GitHub organization

This document is to capture the set up of the `loopbackio` GH organization and transferring the repositories to https://github.com/loopbackio. 

## GitHub teams

There are 4 teams 
- [loopback-admins](https://github.com/orgs/loopbackio/teams/loopback-admins): individuals in this team are the owners of this GitHub org
- [loopback-tsc](https://github.com/orgs/loopbackio/teams/loopback-tsc): individuals are part of the LoopBack's Technical Steering Committee
- [loopback-maintainers](https://github.com/orgs/loopbackio/teams/loopback-maintainers): maintainers of loopback-next repos.
- [loopback-ibmi-maintainers](https://github.com/orgs/loopbackio/teams/loopback-ibmi-maintainers): maintainers of `loopback-connector-ibmi` repo.

## Installed GitHub Apps
- [DCO bot](https://github.com/probot/dco)
    - Usage: bot to enforces the DCO on pull requests.
    - How to enable: go to https://github.com/apps/dco to configure. Currently it's enabled for all repos under `loopbackio` org.
- [stalebot](https://github.com/apps/stale)
    - Usage: bot that closes stale issues or pull requests based on the configuration
    - How to enable: go to https://github.com/apps/stale to configure. Currently it's enabled for all repos under `loopbackio` org.

## Repository level settings 
- delete branch on PR merge: Previously for repos in `strongloop` org, the [delete-merged-branch](https://github.com/SvanBoxel/delete-merged-branch) bot are enabled so that when a PR has merged, the branch will automatically deleted (with the ability to restore the branch later). GitHub has the feature to [manage the automatic deletion on branches](https://docs.github.com/en/github/administering-a-repository/configuring-pull-request-merges/managing-the-automatic-deletion-of-branches). This is being used instead.