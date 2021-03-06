# ArDrive Web

![deploy](https://github.com/ardriveapp/ardrive-web/workflows/deploy/badge.svg)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/ardriveapp/ardrive-web/issues)

The ArDrive Web App allows a user to log in to securely view, upload and manage their ArDrive files.

Have any questions? Join the ArDrive Discord channel for support, news and updates. https://discord.gg/ya4hf2H

## Development

To start code generation, run:

```shell
flutter packages pub run build_runner watch
```

To start a development instance for web, run:

```shell
flutter run -d Chrome
```

All changes made to `dev` will be continuously deployed to [staging.ardrive.io](https://staging.ardrive.io). All PRs from this repo merging into `dev` will trigger a preview build that can be shared freely.

## Release

To create a release to [app.ardrive.io](https://app.ardrive.io), first merge any changes from `dev` into `master` that are required, and publish a new release through the GitHub UI with the tag name matching the pattern `v*` eg. `v1.0.1`.

This will trigger a GitHub Action that will deploy `master` to production.
