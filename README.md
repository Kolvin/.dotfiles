<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
## Contents

- [dotfiles](#dotfiles)
- [Prerequisites](#prerequisites)
  - [Install](#install)
- [Features](#features)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->
___

# dotfiles

> this repo is dependant on my own password vault, get yer ain

Powered by [`Chezmoi 🏠`](https://www.chezmoi.io/)
___

# Prerequisites
The following inputs are required for machine bootstap
 - [git commit email](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-user-account/managing-email-preferences/setting-your-commit-email-address)
 - [git commit username](https://docs.github.com/en/get-started/getting-started-with-git/setting-your-username-in-git)
 - [GPG](https://docs.github.com/en/authentication/managing-commit-signature-verification/telling-git-about-your-signing-key) signing key ID
 - 1password login details
   - url
   - email
   - master key

## Install
```
sh -c "$(curl -fsLS chezmoi.io/get)" -- init --apply https://github.com/Kolvin/dotfiles --verbose
```
___

# Features
- [x] [chezmoi](https://www.chezmoi.io/) setup
- [x] .zsh
  - [x] ~~theme: [powerlevel10k](https://github.com/romkatv/powerlevel10k)~~
  - [x] theme: [starship](https://starship.rs/)q
- [x] .ssh
- [ ] cross platform
  - [x] macOS
  - [ ] linux 
