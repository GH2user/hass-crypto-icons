# hass-crypto-icons
Additional vector icons of various Crypto coins for Home Assistant.
Request for other icons are welcome, refer below.

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
Some of these have been hand drawn in Inkscape and others are reworked icons.

[//]: # (Start Crypto Icons)

| Icon | crypto:<TAG> |
  | Name |
  | Value |
  
| :--- | :--- | :--- | :--- |

![icons v1.0.0](https://github.com/GH2user/hass-crypto-icons/blob/main/docs/examples/icons_100.jpg?raw=true)


[//]: # (End Crypto Icons) 

  
### Icon Requests?
Your crypto coin not there? Let me know what's missing by raising a [Custom Icon Request](https://github.com/arallsopp/hass-hue-icons/issues/new?assignees=arallsopp&labels=icon+request&template=custom-icon-request.md&title=Icon%20Request%20%5Bname%20of%20fixture%5D).


### Sample Dash 
With view icons and state color applied, normally you would have them green or red depending on trend up or down.
![lovelace_example](https://raw.githubusercontent.com/arallsopp/hass-hue-icons/main/docs/examples/lovelace_example.png)

### Discussion:
There's a thread over at the [home assistant forums](https://community.home-assistant.io/t/created-custom-colorizable-hue-icons-as-a-lovelace-resource) that tracks this repo.

## Troubleshooting:

### Can't see the icons?
If you cannot see the new icons, or you get an empty box where you're expecting an icon, press CTRL-F5 when your browser window has focus. 

### Still can't see the icons?
If you cannot see the new icons, or you get an empty box where you're expecting an icon, flush your network cache. 

### Icons don't show on first load of the dash?
Did you add the frontend extra_module_url in your configuration.yaml? See the [installation section](#installation) for details.



 
## Thanks and Props
- based on original work of @arallsopp for which many thanks
- he received guidance from 
- - @hulkhaugen and @thomasloven for the technique.
- - @ludeeus for the installation guidance.
- Everyone who has helped make this repo so broad by raising an [Icon Request](https://github.com/arallsopp/hass-hue-icons/issues/new?assignees=arallsopp&labels=icon+request&template=custom-icon-request.md&title=Icon%20Request%20%5Bname%20of%20fixture%5D).

### Stargazers
[![Stargazers repo roster for @arallsopp/hass-hue-icons](https://reporoster.com/stars/arallsopp/hass-hue-icons)](https://github.com/arallsopp/hass-hue-icons/stargazers)

---


### License

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].
I do this for fun, without charge, and to give back to the community. You may remix, tweak, and build upon this work non-commercially, as long as you credit the original author, provide a link to the license, and indicate if any changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use unless agreed. If you remix, transform or build upon the material, you must distribute your contributions under the same or compatible license as the original. 

