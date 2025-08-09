# Macbook tips

## Table of Contents

- [Macbook tips](#macbook-tips)
  - [Table of Contents](#table-of-contents)
  - [Commands](#commands)
    - [Install Homebrew](#install-homebrew)
    - [Install Bash Git Completion](#install-bash-git-completion)
    - [How to Change Screenshot Save Location](#how-to-change-screenshot-save-location)
    - [Monospaced font with programming ligatures: FiraCode](#monospaced-font-with-programming-ligatures-firacode)
    - [Setting the Mac hostname or computer name from the terminal](#setting-the-mac-hostname-or-computer-name-from-the-terminal)
    - [Main font-bundle for sketch icon-font plugin](#main-font-bundle-for-sketch-icon-font-plugin)
    - [Install jq command](#install-jq-command)
  - [Recommended Applications \& IDEs](#recommended-applications--ides)
  - [Tips](#tips)
    - [Show all filename extensions in `Finder`](#show-all-filename-extensions-in-finder)
    - [How to change the ScreenShot Keyboard Shortcut](#how-to-change-the-screenshot-keyboard-shortcut)
    - [Change the Shell in Mac OS X Terminal](#change-the-shell-in-mac-os-x-terminal)
    - [Using a Windows PC Keyboard on Mac with Remapped Windows \& ALT Keys](#using-a-windows-pc-keyboard-on-mac-with-remapped-windows--alt-keys)
    - [Change default shell in terminal (iTerm2)](#change-default-shell-in-terminal-iterm2)
    - [Tmux scrollback in terminal (iTerm2)](#tmux-scrollback-in-terminal-iterm2)
    - [Native Sierra-tabs on VSCode](#native-sierra-tabs-on-vscode)
    - [Change keyboard mapping for windows keyboard](#change-keyboard-mapping-for-windows-keyboard)
    - [Change Hot keys in iTerm2](#change-hot-keys-in-iterm2)
    - [Turn on three finger drag for your Mac trackpad](#turn-on-three-finger-drag-for-your-mac-trackpad)
    - [Change Spodlight shortcut key](#change-spodlight-shortcut-key)
    - [Jump between words in a bash command](#jump-between-words-in-a-bash-command)
  - [Troubleshooting](#troubleshooting)
  - [Contributing](#contributing)

A curated collection of practical commands, tips, and tools for MacOS users.

This guide is designed for:

- **Power users** and developers seeking shortcuts, automation, and enhanced productivity on macOS.
- **New users** wanting to discover key utilities and improve their workflow.
- Anyone looking for trustworthy recommendations on setup, configuration, and essential software.

**How to use this guide:**

1. Use the [Table of Contents](#table-of-contents) above to browse sections quickly.
2. Each command or tip includes context and purpose—read before you copy!
3. External links and references provide deeper learning and troubleshooting help.
4. Visuals illustrate step-by-step actions wherever possible.

Feel free to contribute improvements or suggest new tips to keep this document up-to-date for all Macbook users!

![Screenshot of Apple MacBook M1 hardware](./images/apple_mac_m1.png)
*Apple MacBook M1 – sleek design and performance for macOS users*

## Commands

### Install Homebrew

Visit the [Homebrew homepage](https://brew.sh/) for details — official installation instructions and documentation.

**Purpose:** Homebrew is an essential package manager for macOS, allowing you to install apps and developer tools from the command line.

**How to install:**

1. Open your Terminal.
2. Run the following command (requires permission to install software):

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

*After installation, verify by running `brew --version`.*

---

### Install Bash Git Completion

**Purpose:** Enable tab completion for Git commands in Bash, improving workflow speed.

**How to install:**

1. Make sure Homebrew is already installed.
2. Run:

```bash
brew install git bash-completion
```

*Enables both Git and Bash tab completion.*

**Further setup:**
To activate bash-completion when opening new terminals, add this line to your `~/.bash_profile` or `.extra` config file:

```bash
[ -f /usr/local/etc/bash_completion ] && . /usr/local/etc/bash_completion
```

### [How to Change Screenshot Save Location](https://discussions.apple.com/docs/DOC-9081)

create new folder in `Desktop`

```bash
mkdir ~/Desktop/screenshots/
```

Copy and paste this command to the terminal window:

```bash
defaults write com.apple.screencapture location ~/Desktop/screenshots/
```

### Monospaced font with programming ligatures: [FiraCode](https://github.com/tonsky/FiraCode)

Use [brew](http://brew.sh/) and [cask](https://caskroom.github.io/): Not officially supported, might install outdated version

```bash
brew tap homebrew/cask-fonts
brew install font-fira-code --cask
```

screenshot: see the `!=` symbol

![firacode](./images/firacode.png)

### Setting the Mac hostname or computer name from the terminal

See the [reference](https://knowledge.autodesk.com/support/smoke/learn-explore/caas/sfdcarticles/sfdcarticles/Setting-the-Mac-hostname-or-computer-name-from-the-terminal.html). change the primary hostname of your Mac:

```bash
scutil --set HostName <new host name>
```

### Main font-bundle for sketch icon-font plugin

- FontAwesome
- Material Design Icons
- Ion Icons
- Simple Line Icons (@bohn002)
- Ant Design Icons

See the [detail](https://github.com/keremciu/font-bundles)

![font](./images/font.png)

### [Install jq command](https://stedolan.github.io/jq/)

jq is a lightweight and flexible command-line JSON processor. [Try it online](https://jqplay.org/).

![jq_command](./images/jq_command.png)

## Recommended Applications & IDEs

A curated list of productivity, development, and utility apps for macOS:

- [GraphQL Playground](https://github.com/prisma/graphql-playground) — Powerful GraphQL IDE for better development workflows.
- [Visual Studio Code](https://code.visualstudio.com) — Popular open-source code editor.
- [SSH Tunnel Manager](https://www.tynsoe.org/stm/) — Simplifies SSH tunnel setup.
- [Caprine](https://github.com/sindresorhus/caprine) — Elegant Facebook Messenger desktop client.
- [Discord](https://discordapp.com/) — Voice, video, and text chat for communities and developers.
- [Gitter](https://gitter.im/) — Chat and networking platform for devs.
- [Docker for Mac](https://docs.docker.com/docker-for-mac/install/) — Container platform for development.
- [WeChat](https://www.wechat.com/en/) — Messaging popular in Asia.
- [Google Chrome](https://www.google.com/chrome/) — Reliable web browser.
- [Telegram Desktop Messenger](https://github.com/telegramdesktop/tdesktop) — Secure messaging app.
- [iTerm2](https://www.iterm2.com/downloads.html) — Advanced replacement for the default Terminal.
- [Evernote Skitch](https://evernote.com/intl/en/products/skitch) — Screenshot and markup tool.
- [MPlayer OSX Extended](https://github.com/sttz/MPlayer-OSX-Extended) — Feature-rich media player.
- [DBeaver Community](https://dbeaver.io/) — Universal database tool.
- [Phiewer](https://phiewer.com/) — Fast and easy image viewer.
- [FileZilla Client](https://filezilla-project.org/) — Supports FTP, FTPS, SFTP.
- [Slack](https://slack.com/) — Team and project discussions.
- [Postman](https://www.getpostman.com/downloads/) — API client.
- [TablePlus](https://github.com/TablePlus/TablePlus) — Database management tool.
- [Keka](https://www.keka.io) — File archiver.
- [Elmedia Player](https://www.elmedia-video-player.com/) — Alternative macOS media player.
- [Robo 3T](https://robomongo.org/download) — MongoDB desktop client.
- [Microsoft Remote Desktop](https://apps.apple.com/tw/app/microsoft-remote-desktop/id1295203466?mt=12) — Remote access to Windows computers.
- [Diagrams.net](https://www.diagrams.net/) — Security-first diagramming for teams.
- [Mipony](https://www.mipony.net/en/) — Download manager.
- [IINA](https://iina.io/) — Modern macOS media player.
- [Fig](https://fig.io/) — IDE-style autocomplete for your terminal.
- [AppCleaner](https://freemacsoft.net/appcleaner/) — Thorough app uninstaller.
- [MacWhisper](https://goodsnooze.gumroad.com/l/macwhisper) — Fast AI-based audio transcription.
- [Mounty for NTFS](https://mounty.app/) — Enables write access to NTFS drives on macOS (Free and lightweight).

## Tips

### Show all filename extensions in `Finder`

See the following screenshots:

![Screenshot of Finder with filename extensions visible](./images/finder.png)
*Finder window showing filename extensions enabled in macOS*

### How to change the ScreenShot Keyboard Shortcut

See [WikiHow: Change Screenshot Shortcut](https://www.wikihow.com/Change-the-Keyboard-Shortcut-for-a-Mac-Screenshot) for step-by-step customization instructions.

![Screenshot of macOS keyboard shortcut settings for screenshots](./images/shortcut_001.png)
*macOS settings dialog for changing screenshot keyboard shortcuts*

![Screenshot: Additional screenshot shortcut key options in macOS](./images/shortcut_002.png)
*Other screenshot shortcut options available in macOS settings*

### Change the Shell in Mac OS X Terminal

More details in [OSXDaily: Change Shell on Mac OS X](http://osxdaily.com/2012/03/21/change-shell-mac-os-x/).

open the `terminal` app and select the `preferences`

![Mac Terminal Preferences window screenshot](./images/terminal_001.png)
*Selecting preferences in the macOS Terminal app*

![Screenshot: macOS Terminal app profile settings](./images/terminal_002.png)
*Changing Terminal profiles and shell options in preferences*

### Using a Windows PC Keyboard on Mac with Remapped Windows & ALT Keys

See [OSXDaily: Remap Option/Command Keys](http://osxdaily.com/2018/01/31/use-windows-pc-keyboard-mac-remap-option-command-keys/) — guidance on using Windows keyboards and adjusting mappings in macOS.

![Mac system keyboard mapping dialog for Windows keyboard](./images/keyboard_01.png)
*Mapping Windows and ALT keys to Command and Option in macOS system settings*

1. Select your windows keyboard.
2. Click the dropdown next to `OPTION Key` and select `Command`
3. Click the dropdown next to `COMMAND Key` and select `Option`

![keyboard_02](./images/keyboard_02.png)

### Change default shell in terminal (iTerm2)

![iterm2](./images/iterm2-command.png)

```sh
chsh -s /bin/bash
```

See [Use zsh as the default shell on your Mac](https://support.apple.com/en-us/HT208050)

### Tmux scrollback in terminal (iTerm2)

You can copy my [.tmux.conf](https://github.com/appleboy/dotfiles/blob/5c6bd88915b6ba97c50ff9f6f7627d9ad1ff31d9/.tmux.conf#L1) config file and [update the profile of iTerm2](https://stackoverflow.com/questions/12865559/leaving-tmux-scrollback-in-terminal-iterm2) as following screenshot:

![iterm2](./images/iterm2.png)

### Native Sierra-tabs on VSCode

See the [issue comment](https://github.com/microsoft/vscode/issues/76537#issuecomment-510070135)

![vscode 01](./images/vscode_01.png)

![vscode 02](./images/vscode_02.png)

See [Use tabs in windows on Mac](https://support.apple.com/guide/mac-help/use-tabs-in-windows-mchla4695cce/mac)

![native tab](./images/native_tab.png)

### Change keyboard mapping for windows keyboard

See the [solution](https://superuser.com/questions/158561/how-can-i-remap-windows-and-alt-keys-in-os-x/158568).

![keyboard](./images/window_keyboard.png)

### Change Hot keys in iTerm2

Go to iTerm Preferences → Profiles, select your profile, then the Keys tab. Click Presets... and choose `Natural Text Editing`. See tbe [reference](https://apple.stackexchange.com/questions/136928/using-alt-cmd-right-left-arrow-in-iterm).

![keyboard](./images/iterm2_hot_key.png)

### Turn on three finger drag for your Mac trackpad

![drag01](./images/three-finger-drag-01.png)
![drag02](./images/three-finger-drag-02.png)

### Change Spodlight shortcut key

![spotlight](./images/spotlight.png)

### Jump between words in a bash command

In iTerm2, if you want to use `Option + Right Arrow` to jump between words in a bash command, you can set it up as follows:

1. Open iTerm2.
2. In the top menu, select `iTerm2` -> `Preferences`.
3. In the Preferences window, select the `Profiles` tab.
4. On the left side, select the profile you are using (usually `Default`).
5. Select the `Keys` sub-tab.
6. Click the `+` button at the bottom right to add a new key binding.
7. In the pop-up window, set it as follows:
   - `Keyboard Shortcut`: Press `Option + Right Arrow`.
   - `Action`: Select `Send Escape Sequence`.
   - `Esc+`: Enter `f`.

This way, when you press `Option + Right Arrow`, iTerm2 will send `Esc+f`, which in bash will move to the beginning of the next word.

Similarly, you can set `Option + Left Arrow` to jump to the beginning of the previous word:

1. Repeat the above steps, click the `+` button to add a new key binding.
2. In the pop-up window, set it as follows:
   - `Keyboard Shortcut`: Press `Option + Left Arrow`.
   - `Action`: Select `Send Escape Sequence`.
   - `Esc+`: Enter `b`.

This way, when you press `Option + Left Arrow`, iTerm2 will send `Esc+b`, which in bash will move to the beginning of the previous word.

After completing these settings, you should be able to use `Option + Right Arrow` and `Option + Left Arrow` to jump between words in bash commands in iTerm2.

---

## Troubleshooting

If you encounter issues while following these tips or installing software:

- **Permissions errors:** Try running commands with `sudo` if appropriate, or check your user’s access rights.
- **Missing dependencies:** Ensure you have the latest version of macOS and Xcode command line tools (`xcode-select --install`).
- **Homebrew not found:** Reinstall using the latest [official guide](https://brew.sh/) and restart your terminal.
- **Command not found:** Double-check spelling and package installation status (e.g., `brew list`).
- For tool-specific issues, consult the linked official documentation in each section.

Feel free to [open an issue](https://github.com/appleboy/macbook/issues) or contact the project maintainer for additional help.

---

## Contributing

Contributions and suggestions are welcome!

- Fork this repository and submit a pull request with improvements.
- Review open issues or propose new tips for Macbook users.
- Ensure all new documentation is clear, concise, and uses consistent formatting.
- All contributors will be credited in release notes and documentation history.

Thank you for helping improve this guide for everyone!
