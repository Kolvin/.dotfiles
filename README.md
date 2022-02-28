# Kolvins .dotfiles
managed with [`chezmoi`](https://www.chezmoi.io/)

## How to use
```
sh -c "$(curl -fsLS chezmoi.io/get)" -- init --apply Kolvin
```

## Secret managment
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

## TODO
- [x] [chezmoi](https://www.chezmoi.io/) setup
- [x] .zsh
  - [x] theme: powerlevel10k
- [ ] .ssh