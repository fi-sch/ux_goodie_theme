# UX Goodie Theme

[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg)](https://github.com/custom-components/hacs)

<a href="https://www.buymeacoffee.com/fisch" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-2.svg" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>

> The UX Goodie Theme for Home Assistant made by @fi-sch. Inspired by iOS Dark Mode and [@basnijholt](https://github.com/basnijholt/lovelace-ios-dark-mode-theme)'s theme.

See instructions below!

## Screenshots

### Overview

![Theme - Overview](https://raw.githubusercontent.com/fi-sch/ux_goodie_theme/master/docs/theme-overview.jpg)

### Logbook

![Theme - Logbook](https://raw.githubusercontent.com/fi-sch/ux_goodie_theme/master/docs/theme-logbook.png)

### History

![Theme - History](https://raw.githubusercontent.com/fi-sch/ux_goodie_theme/master/docs/theme-history.png)

### Developer Tools

![Theme - Developer Tools](https://raw.githubusercontent.com/fi-sch/ux_goodie_theme/master/docs/theme-developer-tools.png)

### Hass.io

![Theme - Hass.io](https://raw.githubusercontent.com/fi-sch/ux_goodie_theme/master/docs/theme-hassio.png)

### Configuration

![Theme - Configuration](https://raw.githubusercontent.com/fi-sch/ux_goodie_theme/master/docs/theme-configuration.png)

### Profile

![Theme - Profile](https://raw.githubusercontent.com/fi-sch/ux_goodie_theme/master/docs/theme-profile.png)

## Installation

1. Add the following code to your `configuration.yaml` file (reboot required).

```yaml
frontend:
  ... # your configuration.
  themes: !include_dir_merge_named themes
  ... # your configuration.
```

2. Put `background.jpg` into your `/config/www/` directory. For example file see `backgrounds/` directory of this repository.

3. (Optional) Add the following to your `lovelace-ui.yaml` or use the RAW editor: (you also need to install [`custom-header`](https://github.com/maykar/custom-header)) to display date and time in tab bar:

```
custom_header:
  button_text:
    options: '{{ time }}<br>{{ date }}'
  compact_mode: true
```
NOTE: `options:` from above example may not display properly in HACS. Please see GitHub repository.)

### HACS

1. Go to the Community Store.
2. Search for `UX Goodie Theme`.
3. Navigate to `UX Goodie Theme` theme.
4. Press `Install`.
5. Follow point 2 from `Installation` section above.
6. Go to services and trigger the `frontend.reload_themes` service.
7. (Optional) Follow point 3 from `Installation` section above.

### Manual

1. Clone this repository in your existing (or create it) `themes/` folder.

```bash
cd themes/
git clone https://github.com/home-assistant-community-themes/lovelace-ux-goodie-theme.git
```

Or using submodules:

```bash
cd themes/
git submodule add https://github.com/home-assistant-community-themes/lovelace-ux-goodie-theme.git
```

2. Follow points 2 and 3 from `Installation` section above.

