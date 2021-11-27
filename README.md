# hass-crypto-icons
Additional vector icons of various Crypto coins for Home Assistant.
Request for other icons are welcome, refer below.
![header-bar](https://github.com/GH2user/hass-crypto-icons/blob/main/docs/examples/header_bar.jpg?raw=true)

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]
[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]


[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

## <a name="installation"></a>Installation

Hass-crypto-icons has been accepted into the [Home Assistant Community Store (HACS)](https://hacs.xyz). 

### HACS:
Not Yet, please STAR this repository so it might get added to the default HACS repositories !


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
- In your entity editor, specify an icon as `crypto:coin-TAG` 
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

hass-crypto-icons initially includes 40 crypto coin icons based on various sources.
Some of these have been hand drawn in Inkscape and others are reworked icons from the net.

Shown in the button screenshot below are:
- icon + coin tag
- coin name
- 
To show the icon the coin TAG is used; eg.  crypto:ada

[//]: # (Start Crypto Icons)

![icons v1.0.0AJ](https://github.com/GH2user/hass-crypto-icons/blob/main/docs/examples/v1-0-0%20A_J.jpg?raw=true)

![icons v1.0.0KZ](https://github.com/GH2user/hass-crypto-icons/blob/main/docs/examples/v1-0-0%20K-Z.jpg?raw=true)

![icons v1.0.0circular](https://github.com/GH2user/hass-crypto-icons/blob/main/docs/examples/v1-0-0%20circular.jpg?raw=true)


[//]: # (End Crypto Icons) 

  
### Icon Requests?
Your crypto coin not there? You like another design? Let me know what's missing by raising a [Custom Icon Request](https://github.com/arallsopp/hass-hue-icons/issues/new?assignees=arallsopp&labels=icon+request&template=custom-icon-request.md&title=Icon%20Request%20%5Bname%20of%20fixture%5D).



## Discussion:
Currently there is no dedicated area to discuss this, if sufficient interest we can open one on the [home assistant forums](https://community.home-assistant.io/c/projects/9).


## Troubleshooting:

### Can't see the icons?
If you cannot see the new icons, or you get an empty box where you're expecting an icon, press CTRL-F5 when your browser window has focus. 

### Still can't see the icons?
If you cannot see the new icons, or you get an empty box where you're expecting an icon, flush your network cache. 

### Icons don't show on first load of the dash?
Did you add the frontend extra_module_url in your configuration.yaml? See the [installation section](#installation) for details.



 
## Thanks and 
- based on original work of @arallsopp for which many thanks
- he received guidance from 
- - @hulkhaugen and @thomasloven for the technique.
- - @ludeeus for the installation guidance.
- Everyone who has helped extending this repo by raising an [Icon Request](https://github.com/GH2user/hass-crypto-icons/issues/new?assignees=GH2user&labels=icon+request&template=custom-icon-request.md&title=Icon%20Request%20%5Bname%20of%20fixture%5D).

---


### License

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].
I do this for fun, without charge, and to give back to the community. You may remix, tweak, and build upon this work non-commercially, as long as you credit the original author, provide a link to the license, and indicate if any changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use unless agreed. If you remix, transform or build upon the material, you must distribute your contributions under the same or compatible license as the original. 

