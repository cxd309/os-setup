# os-setup

## enable sudo

[debian - sudo](https://wiki.debian.org/sudo)

## apt

### Nvidia drivers

Follow the pre installation instructions
[Debian nVidia docs](https://wiki.debian.org/NvidiaGraphicsDrivers). This probably means going in and changing deb sources.

```bash
sudo apt install nvidia-kernel-dkms nvidia-driver
```

### TeX

```bash
sudo apt install texlive-full texstudio
```

### Other

Get the following package feeds:

- [GitHub Desktop](https://github.com/shiftkey/desktop)
- [FortiClient 7.2](https://www.fortinet.com/uk/support/product-downloads/linux)

```bash
apt install git github-desktop forticlient  flatpak gnome-software-plugin-flatpak chromium curl
```

## flatpak

Add the flathub repository.

```bash
flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
```

Install the packages we are after

```bash
flatpak install flathub com.google.Chrome org.mozilla.Thunderbird io.dbeaver.DBeaverCommunity com.getpostman.Postman
```

## VS Code

[Download link to get the deb file](https://code.visualstudio.com/thank-you?dv=linux64_deb)

## Jetbrains

[Toolbox install instructions](https://www.jetbrains.com/help/toolbox-app/toolbox-app-silent-installation.html)

## dprint

[Website](https://dprint.dev/)

```bash
curl -fsSL https://dprint.dev/install.sh | sh
```

## Python Tools

[uv docs](https://docs.astral.sh/uv/getting-started/installation/)

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

[ruff docs](https://docs.astral.sh/ruff/installation/) [ty docs](https://docs.astral.sh/ty/installation/)

```bash
uv tool install ruff@latest && uv tool install ty@latest
```

[Poetry](https://python-poetry.org/docs/#installing-with-the-official-installer)

```bash
curl -sSL https://install.python-poetry.org | python3 -
```

## Gogh (Terminal Theme)

[Github](https://github.com/Gogh-Co/Gogh) GrubBox Dark

## Go Tools

- **Go** — https://go.dev/dl/
- **air** — live reload for development
  ```bash
  go install github.com/air-verse/air@latest
  ```
- **golangci-lint** — linting
  ```bash
  go install github.com/golangci/golangci-lint/cmd/golangci-lint@latest
  ```
- **sqlc** — generates Go code from SQL (only needed if working on DB queries)
  ```bash
  go install github.com/sqlc-dev/sqlc/cmd/sqlc@latest
  ```

## Docker engine

[Install Docs](https://docs.docker.com/engine/install)

## Gnome Extensions

Chromium browser extension and then get an extension manager in the software manager so you can change settings.

- App menu is back
- Dash to Dock
  - Position Left
  - Show on all monitors
  - Icon size 32px
  - Use default theme (remember to set system to dark mode)
- GNOME Fuzzy App Search
- Pomodoro Timer

## Keyboard shortcuts

- alt+tab -> switch windows
- super+enter -> custom `gnome-terminal`
