# Dotfiles-workshop

**Før du starter** 
- Lag et nytt repo på github som heter 'dotfiles', eller hva du ønsker å kalle det.
- Vurder om du ønsker å ha ssh-nøkkel i 1Password. Hvis du er usikker, spør Hans Kristian.

## Homebrew
1. Lag et script som installerer Homebrew 
2. Kjør `homebrew bundle dump` for å starte med din `Brewfile` (da kan du f.eks. skrive `homebrew bundle dump > Brewfile`)
3. Fjern gammelt ræl og kjør `brew bundle cleanup --force`

## oh-my-zsh

1. Lag et script som installerer oh-my-zsh
2. Kopier custom-mappen over i dotfiles-repoet ditt og sett variablen `ZSH_CUSTOM` til å peke på custom-mappen du akkurat kopierte.
3. Gjør noen endringer i `zshrc` og kjør `omz reload` for å se endringene.

## Kitty

1. Kitty (https://sw.kovidgoyal.net/kitty/) kan installeres via homebrew, så rediger din `Brewfile` og legg den til der.
2. Kitty har veldig mange konfigmuligheter. Generer en `kitty.conf` (https://sw.kovidgoyal.net/kitty/conf/#sample-kitty-conf)
3. Legg `kitty.conf` i dotfiles-repoet ditt og symlink den til `~/.config/kitty/kitty.conf`

## Nerdfonts

1. Den feteste fonten heter Github Monaspace, installer den via homebrew https://github.com/githubnext/monaspace#macos
2. Dessverre er ikke det en ekte nerdfont, så installer også `font-symbols-only-nerd-font`.
3. Begge ligger i en egen Homebrew "tap", så du må legge til `tap "homebrew/cask-fonts"` øverst i Brewfile.
4. For å bruke monaspace i Kitty, så kan du se på en eksempelkonfig: https://github.com/heim/dotfiles/blob/master/kitty/kitty.conf


## Starship

1. Sjekk ut starship.rs
2. Installer via homebrew.
3. Rediger og legg til en `starship.toml`


# Inspirasjon og videre oppgaver

## 1Password-integrasjon

Sett opp signering av git-commits med 1password, sjekk bruksanvisning her:

https://developer.1password.com/docs/ssh/ 


## Github CLI

https://cli.github.com

## Thefuck

The Fuck er kanskje den util-en jeg bruker mest. Skrivefeil i kommandoen din? Bare skriv `fuck` også retter den det opp for deg. Årsverk spart!

https://github.com/nvbn/thefuck

## Bedre backwards search 

https://github.com/junegunn/fzf

## Terminal-GUI for git

https://github.com/jesseduffield/lazygit


## Alternativ til Starship - powerlevel10k

https://github.com/romkatv/powerlevel10k

## Installere og sette opp Vim-config

Eller installere NeoVim, LazyVim eller LunarVim hvis du vil!

## Lære seg tmux!

`tmux`
