# macos_setup
some initial configs for macos

## MacOS Setup

#### homebrew

- ```/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"```
- https://brew.sh/
- then follow these on terminal:
  - ```touch ~/.zshrc```
  - add this line at the end of .zshrc: ```export PATH=/opt/homebrew/bin:$PATH```
  - ```source ~/.zshrc```

#### emacs
- ```brew install --cask emacs```
- https://www.gnu.org/software/emacs/

#### git and gui
- ```brew install git```
- https://www.sourcetreeapp.com/

#### vscode
- ```brew install --cask visual-studio-code```
- https://code.visualstudio.com/

#### iterm2
- ```brew install --cask iterm2```
- https://iterm2.com/downloads.html

---

#### oh my zsh
- ```sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"```
- https://ohmyz.sh
- remove below comment to hide terminal context
prompt_context(){
  if [[ "$USER" != "$DEFAULT_USER" || -n "$SSH_CLIENT" ]]; then
    prompt_segment black default "%(!.%{%F{yellow}%}.)$USER"
  fi
}
- Add wisely, as too many plugins slow down shell startup.
plugins=(
	git
	python
	macos
	aliases
	docker
	zsh-autosuggestions
	)
- brew install zsh-autosuggestions

##### [Optional] powerline10k and nerdfonts
- https://github.com/romkatv/powerlevel10k
- https://www.nerdfonts.com/
- explore these online before installing

##### powerline fonts
- clone
    - ```git clone https://github.com/powerline/fonts.git --depth=1```
- install
    - ```cd fonts```
    - ```./install.sh```
- clean-up a bit
    - ```cd ..```
    - ```rm -rf fonts```
- https://github.com/powerline/fonts

##### color themes
- https://github.com/lysyi3m/macos-terminal-themes
- select theme by opening the downloaded theme file using terminal app
- for iterm2, just replace the existing color scheme with this new color theme

---

#### Python
- Install pyenv: ```brew install pyenv```

---

#### continaers
- ```brew install podman```
  - https://podman.io/
- ```brew install --cask docker```
  - https://www.docker.com/products/docker-desktop/

#### SQL DB
- sequel pro: https://www.sequelpro.com/
- dbeaver: https://dbeaver.io/
- sqlite browser: https://sqlitebrowser.org/

#### Terminal tools
- https://terminaltrove.com/categories/macos/
- disk usage:
  - ```brew install dust```
  - ```brew install nsdu```
- table of processes (top) tools:
  - ```brew install btop```
  - ```brew install nvtop```
- networking
  - [Trippy: a network diagnostic tool](https://github.com/fujiapple852/trippy): ```brew install trippy```
- todo manager
  - https://taskwarrior.org/: ```brew install taskwarrior-tui```
- docs converter
  - https://pandoc.org/: ```brew install pandoc```

#### appstore and other utilities
- productivity: color picker, unzip, brave browser (https://brave.com/), goodnotes, unsplash wallpaper, kindle
- play: typist, elpy, piano companion
- photo, audio, video, 3d editor: gimp (https://www.gimp.org/), audacity (https://www.audacityteam.org/), diagrams (https://app.diagrams.net/), vectornator, blender (https://www.blender.org/), vlc (https://www.videolan.org/vlc/)
- games: garage band, snakeio, asphalt9, mini metro, package inc
- office suite: libre office (https://www.libreoffice.org/)
- video recording: obs studio (https://obsproject.com/)
- video editing: openshot (https://www.openshot.org/), shotcut (https://shotcut.org/)
- vpn: proton vpn (https://protonvpn.com/), nord vpn (https://nordvpn.com/)
- programming: scratch (https://scratch.mit.edu/download)


