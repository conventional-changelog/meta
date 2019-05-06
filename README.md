# conventional-changelog

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [conventional-changelog](#conventional-changelog)
  - [Joining the `conventional-changelog` Organization](#joining-the-conventional-changelog-organization)
    - [Setup Two-factor Authentication](#setup-two-factor-authentication)
  - [Setting Up a Project](#setting-up-a-project)
    - [GitHub Labels](#github-labels)
  - [Common Issues](#common-issues)
    - [Disabling Two Factor Authentication](#disabling-two-factor-authentication)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Joining the `conventional-changelog` Organization

There are a few tasks that will need to be completed prior to joining the `conventional-changelog` organization as an administrator, project owner, or outside collaborator.

Some tasks are requirements while others will simply make your experience, and that of others, better.

### Setup Two-factor Authentication

> **Required**

All accounts with access to the `conventional-changelog` organization must have [2FA authentication enabled with GitHUb](https://help.github.com/articles/securing-your-account-with-two-factor-authentication-2fa/).

> This is part of our continued efforts to improve the security of this organization (to minimize, or prevent, [incidents such as this](https://github.com/conventional-changelog/conventional-changelog/issues/282#issuecomment-365802521))

## Setting Up a Project

Once you have a new project on `conventional-changelog`'s organization, it's time to get your project setup with a few things to make your life easier.

### GitHub Labels

To help with issue and pull request management, we recommend a set of [GitHub Labels](https://help.github.com/articles/about-labels/) in this project's [`configuration.json`](./configuration.json) file.

To deploy these labels to a project, please install [`@hutson/github-metadata-sync`](https://www.npmjs.com/package/@hutson/github-metadata-sync), download the `configuration.json` file (or clone this repository), and run the following:

```bash
github-metadata-sync --token [PERSONAL ACCESS TOKEN] --config configuration.json
```

> **Note:** Please create a [_Personal Access Token_](https://help.github.com/articles/creating-a-personal-access-token-for-the-command-line/) with repository access to all repositories listed in the `configuration.json` file and pass that token to the `--token` flag.

## Common Issues

### Disabling Two Factor Authentication

[According to GitHub](https://help.github.com/articles/disabling-two-factor-authentication-for-your-personal-account/):

> Warning: If you're a member, billing manager, or outside collaborator to a public repository of an organization that requires two-factor authentication and you disable 2FA, you'll be automatically removed from the organization, and you'll lose your access to their repositories. To regain access to the organization, re-enable two-factor authentication and contact an organization owner.

In the event that you disable, and then re-enable, 2FA, please reach out to a member of the organization to be re-invited.
