# WordPress + Codespaces Container Project 

Baseline project for creating a container to run PHP+MariaDB/MySQL CMS systems in a self-contained way in GitHub Codespaces. This repo is a testing ground using WordPress as the baseline for future explorations.

This project focuses on community development: Building plugins, themes, blocks, and sites with WordPress. It does not focus on [WordPress Core development](https://make.wordpress.org/core/2022/11/09/improving-the-contributor-experience-github-codespaces-for-wordpress-core/). See note below for further details.

## MVP

Success criteria for this MVP:

Upon opening a Codespace from this template, the following are pre-configured and working
- Fully operational WordPress
- Populated with [Theme Test data](https://github.com/WPTT/theme-test-data)
- Spun up on a dev server so it can be previewed in a separate tab
- Managed through [WP-CLI](https://wp-cli.org/)
- With fully functional XDebug support

These criteria serve to test the limits and edges of Codespaces PHP + DB support.

# Larger plan

Once the MVP criteria are met, the long term plan is to build a series of nested container templates for WordPress and other PHP-based CMS development. The structure will look something like this:

1. PHP CMS Dev template: Functional PHP + MariaDB container with full PHP, XDebug, and other structural supports
2. Baseline WordPress / Drupal / [other CMS] tempalte: Based on PHP CMS Dev template, these templates boot an updated vanilla install of the selected CMS, complete with database populated with test data. The user target here is anyone wanting to quickly mount a test site.
3. WP/Drupal/[other] Dev Template: Based on Baseline, these templates provide best-practice dev tools and packages for advanced site and extension development including theme and plugin development etc.

# WordPress Core development container

Additionally / parallell / adjacent to this project sits the larger and more complex project of creating a [WordPress Core development](https://make.wordpress.org/core/2022/11/09/improving-the-contributor-experience-github-codespaces-for-wordpress-core/) template for contribution to the core open source projects. While these two projects are overlapping, they are also separate as their target audiences have significantly different needs in terms of functionality and tooling.

# Relevant sources, links, and related projects

- [PHP+MariaDB dev container](https://github.com/microsoft/vscode-dev-containers/tree/main/containers/php-mariadb) by [@microsoft](https://github.com/microsoft)
- [WordPress Develop](https://github.com/helen/wordpress-develop/tree/add/devcontainer) by [@helen](https://github.com/helen)
- [WordPress Codespace](https://github.com/dinhtungdu/wordpress-codespace) by [@dinhtungdu](https://github.com/dinhtungdu)
- [VS Code Remote Try WP](https://github.com/soderlind/vscode-remote-try-wp) by [@soderlind](https://github.com/soderlind)
- [DrupalPod](https://www.drupal.org/docs/develop/development-tools/drupalpod/getting-started)
- [Reddit thread on issues encountered](https://www.reddit.com/r/github/comments/pg39cp/has_anyone_had_any_success_setting_up_wordpress/)

# How to contribute

This is an open source project licensed under GPL v3.0. All contributors welcome. File issues, open discussions, submit pull requests, etc.

# Contributors

This project is a collaboration between many interested parties including:

- [@mor10](https://github.com/mor10) [owner] Senior Staff Instructor, LinkedIn Learning (former WordPress contributor)
- [@burkeholland](https://github.com/burkeholland) [owner]

