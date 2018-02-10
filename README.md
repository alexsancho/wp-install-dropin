# WP Dropin: Better install.php
[![Build Status](https://travis-ci.org/alexsancho/wp-install-dropin.svg?branch=master)](https://travis-ci.org/alexsancho/wp-install-dropin)

This `install.php` dropin doesn't install bloat from default install.php and sets a few opionated wp options.

It doesn't send you an email after installing new WordPress either.

## Current options
- Set empty page as Front page
- Don't use any widgets
- Use empty blog description ( if someone forgets to change that )
- Use `/%postname%/` permalink
- Don't install any articles

## Installation
You can copy `install.php` to your `wp-content` folder. Just plug&play.

OR you can use composer so that you can automatically update it too. Put these in your composer.json:
```json
{
    "require": {
        "alexsancho/wp-install-dropin": "^1.0"
    },
    "extra": {
        "dropin-paths": {
            "htdocs/wp-content/": ["type:wordpress-dropin"]
        }
    }
}
```
