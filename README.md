Overview
========
This directory stores a comprehensive theme for Eduardo, Lektorium's platform based on Open edX.

The directory tree is organized to mostly mimic the directory structure of the
edX codebase so that it's easy to tell where the files will end up upon deploy.
The only exception is "common" directory containing files used both by cms and lms.

Enabling theme
===============
- Create directory `/edx/app/edxapp/themes/edx-platform/`
- Clone this repo
- Enable theme in `lms.env.json` and `cms.env.json` located in `/edx/app/edxapp/`:
    ENABLE_COMPREHENSIVE_THEMING: true
    COMPREHENSIVE_THEME_DIRS: ["/edx/app/edxapp/themes/edx-platform"],
    COMPREHENSIVE_THEME_LOCALE_PATHS: ["/edx/app/edxapp/themes/edx-platform/<your-theme>/conf/locale"]
    DEFAULT_SITE_THEME: "<your-theme>"
- Update lms/cms assets and restart the edxapp to enable the theme.

License
=======

The code in this repo is licensed under the Apache 2.0 License.
See [LICENSE.txt](LICENSE.txt) for more info.
