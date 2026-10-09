# IAP/Odoo Fin Utils

## Original Repo

[RIGR's repo](https://github.com/RicGR98/odoo-iap-chrome-extension)

## Overview

This Chrome extension adds a popup on Odoo instances to ease the switching of
config parameters and IAP/Odoo Fin accounts.

## Installation

1. Download the sources by clicking on `Code` on the right
2. Unzip them in the directory of your choice
3. Go to [chrome://extensions/](chrome://extensions/)
4. Activate the Developer mode (top right corner)
5. Click on Load unpacked (top left corner)
6. Select the folder you've chosen
7. Pin the extension in your toolbar if you wish so

[Installation video](https://drive.google.com/file/d/1rkqsS9CAYlhJ_DvOjivTZw8cY9fpguRo/view?usp=sharing)

## Usage

On an Odoo instance, click the extension icon to open the popup.  If you're logged in
and have the necessary rights, the popup will display two columns: one for the config
parameters, and the other for the IAP accounts.

For each, you will have a card showing the name of the key, its current value, and
some buttons to easily switch between different values. If the current value is the same
as one of the buttons, it will be highlighted in purple. A delete button is also available.

## Settings

By default, there already are some keys and some options for each key. You can click on
Extension Settings to tailor the extension to your needs. From the settings, you can
manage your keys and their possible options. Each option is made of a short name that will
be displayed on the popup (i.e. "prod"), and a value that will be used (e.g. https://iap.odoo.com).

You can show/hide each key (to avoid deleting it completely), as well as show/hide the entire
Config Parameters or IAP Accounts sections.

By default that's the IAP settings, if needed here is the Odoo Fin ones:

```
{
    "account_online_synchronization.proxy_mode": {
        "Internal": "internal",
        "Production": "production",
        "Sandbox": "sandbox",
        "show": true
    },
    "database.uuid": {
        "IAP Skip": "skip_check_subscription",
        "show": true
    }
}
```
