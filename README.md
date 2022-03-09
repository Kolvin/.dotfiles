# moi dotfiles
Powered by [`Chezmoi 🏠`](https://www.chezmoi.io/)

# Install

> this repo reads from my 1password acconut so it wont work for you, but you can use this for some inspo

## Prerequisites
Inital setup will ask for the following inputs, make sure you have em
 - [git commit email](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-user-account/managing-email-preferences/setting-your-commit-email-address)
 - [git commit username](https://docs.github.com/en/get-started/getting-started-with-git/setting-your-username-in-git)
 - [GPG](https://docs.github.com/en/authentication/managing-commit-signature-verification/telling-git-about-your-signing-key) signing key ID
 - 1password login details
   - url
   - email
   - master key
```
sh -c "$(curl -fsLS chezmoi.io/get)" -- init --apply https://github.com/Kolvin/dotfiles --verbose
```
___
# TODO
- [x] [chezmoi](https://www.chezmoi.io/) setup
- [x] .zsh
  - [x] theme: powerlevel10k
- [x] .ssh
- [ ] cross platform
  - [x] macOS
  - [ ] linux 

___

# Secret managment
Personal & Work secrets are stored in [1Password](https://1password.com/), and you'll need
the [1Password
CLI](https://support.1password.com/command-line-getting-started/) installed.
Login to 1Password for the first time with:
```
eval $(op signin <subdomain>.1password.com <email>)
```

Then, to login afterwards, run:
```
eval $(op signin)
```