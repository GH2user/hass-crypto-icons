# hass-crypto-icons
Additional vector icons for Home Assistant of various Crypto coins.
Only because I wanted to track a few coins by using Home Assistant.

[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs)
[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]
[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]


[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

## <a name="installation"></a>Installation

Hass-crypto-icons has been accepted into the [Home Assistant Community Store (HACS)](https://hacs.xyz). 

### HACS (Recommended):
This is the recommended way to install hass-hue-icons. Hass-hue-icons is a default repository for HACS. To install:

- Load HACS (installation instructions are [here](https://hacs.xyz/docs/installation/installation/)).
- Select 'Frontend' to see the list of front end plugins and repositories.
- Click the '+ Explore & Add repositories' button.
- Type 'hass crypto icons' into the search bar and click the row returned.
- Click 'Install this repository in HACS' from the resulting dialog. 
- Add the following to your configuration.yaml, save and restart HA.
```
frontend:
  extra_module_url:
    - /hacsfiles/hass-crypto-icons/hass-crypto-icons.js
```

### Manual:
- Copy `dist/hass-crypto-icons.js` into your `config/www` folder.
- Go to Configuration -> Lovelace Dashboards -> Resources -> Add Resource
- set url as `/local/hass-crypto-icons.js` and Resource Type as `Javascript Module`.
- Add the following to your configuration.yaml, save and restart HA.
```
frontend:
  extra_module_url:
    - /local/hass-crypto-icons.js
```

- Save, restart Home Assistant.


## Usage
- In your entity editor, specify an icon as `crypto:icon-name` 
- If you set `state_color: true` in your card, you'll see the icons get colorised based upon the current RGB setting.
- They will show up in the new icon-picker from HA 2021-11.0 and onwards

### Example:

```
title: Crypto
state_color: true
type: entities
entities:
  - entity: sensor.crypto_dot
    name: Polkadot
    icon: crypto:dot
```

## Icons

### Crypto Icons

hass-crypto-icons includes 20 crypto coin icons based on various sources.

[//]: # (Start Crypto Icons)

| Icon | Name | Icon | Name 
| :--- | :--- | :--- | :--- |
| ![hue:bloom](https://raw.githubusercontent.com/arallsopp/hass-hue-icons/main/docs/svgs/bloom.svg)| hue:bloom | ![hue:bollard](https://raw.githubusercontent.com/arallsopp/hass-hue-icons/main/docs/svgs/bollard.svg)| hue:bollard |
