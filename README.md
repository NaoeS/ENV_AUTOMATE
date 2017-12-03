# ENV_AUTOMATE
- 自分専用の環境について諸々と

## 構成
### Browser
- Chrome

### Tools
- ShiftIt
- Docker
- Postman

### CUI
- Fish
- iTerm2
- Tmux(future)
- Powerline(future)
- git
  * tig

### Editor
- Atom
  * Packages
- CotEditor

### Package Manager
- HomeBrew
  * homebrew-bundle
  * mas-cli
  * nodebrew
  * pyenv
  * rbenv
- anyenv(future)
  * ndenv
  * rbenv
  * pyenv

## 環境構築手順
### 1. HomeBrew
```
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ git clone git@github.com:NaoeS/ENV_AUTOMATE.git
$ cd ENV_AUTOMATE
$ brew tap Homebrew/bundle
$ brew bundle
```

### 2. fish
```
$ sudo /etc/shells >> /usr/local/bin/fish
$ chsh -s /usr/local/bin/fish
$ fisher install omf/theme-bobthefish
$ git clone git@github.com:powerline/fonts.git
$ fonts/install.sh
$ rm -rf fonts //iTerm2でフォント設定を行う(D2Coding for Powerline)
$ cp config.fish ~/.config/fish/config.fish
$ . ~/.config/fish/config.fish
```

### 3. Atom
```
$ apm install --packages-file AtomFile
```
