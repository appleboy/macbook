# Macbook tips

Some tips and command for MacOS.

<img src="./images/macos.png">

## Command

### [Install Bash git completion](https://github.com/bobthecow/git-flow-completion/wiki/Install-Bash-git-completion)

```
$ brew install git bash-completion
```

Add bash-completion to your `~/.bash_profile` or `.extra`

```
[ -f /usr/local/etc/bash_completion ] && . /usr/local/etc/bash_completion
```

### [How to Change Screenshot Save Location](https://discussions.apple.com/docs/DOC-9081)

1. create new folder in `Desktop`

```
$ mkdir ~/Desktop/screenshots/
```

2. Copy and paste this command to the terminal window:

```
$ defaults write com.apple.screencapture location ~/Desktop/screenshots/
```

### Monospaced font with programming ligatures: [FiraCode](https://github.com/tonsky/FiraCode)

Use [brew](http://brew.sh/) and [cask](https://caskroom.github.io/): Not officially supported, might install outdated version

```
$ brew tap caskroom/fonts
$ brew cask install font-fira-code
```

screenshot: see the `!=` symbol

<img src="./images/firacode.png">

## IDE

- [GraphQL IDE for better development workflows](https://github.com/prisma/graphql-playground)
- [Visual Studio Code](https://code.visualstudio.com)
- [SSH Tunnel Manager](https://www.tynsoe.org/v2/stm/)
- [Elegant Facebook Messenger desktop app](https://github.com/sindresorhus/caprine)
- [Discord App](https://discordapp.com/)
- [Gitter is a chat and networking platform](https://gitter.im/)
- [Docker for Mac](https://docs.docker.com/docker-for-mac/install/)
- [Wechat in China](https://www.wechat.com/en/)
- [Google Chrome](https://www.google.com/chrome/)
- [Telegram Messenger](https://telegram.org/)
- [iTerm2 is a replacement for Terminal and the successor to iTerm](https://www.iterm2.com/downloads.html)
- [Evernote skitch](https://evernote.com/intl/en/products/skitch)

## Tips

### Show all filename extensions in `Finder`

See the following screenshots:

<img src="./images/finder.png">

### How to change the Keyboard Shortcut

You can see the [reference](https://www.wikihow.com/Change-the-Keyboard-Shortcut-for-a-Mac-Screenshot).

<img src="images/shortcut_001.png">

<img src="images/shortcut_002.png">

### Change the Shell in Mac OS X Terminal

You can see the [reference](http://osxdaily.com/2012/03/21/change-shell-mac-os-x/).

open the `terminal` app and select the `preferences`

<img src="./images/terminal_001.png">

<img src="./images/terminal_002.png">
