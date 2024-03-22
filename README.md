# Profile Exporter for ProcessWire 3.x

This module exports an installable site profile of your site. It essentially enables 
you take any site and create files that the ProcessWire installer will recognize 
when installing a new copy of ProcessWire. This is the tool that is used to export
all of the ProcessWire core site profiles. 

## About site profiles

Site profiles exported by this tool include the following:

- The site database (but no caches and users)
- Files associated with pages (/site/assets/files/)
- Configuration file (/site/config.php), but no DB connection info
- Template files and related assets (/site/templates/*)
- Installed site modules (/site/modules/), except for this one
- Installed custom Page classes (/site/classes/), when used
- System files in /site/ (ready.php, init.php, finished.php, etc.)

Site profiles do not include users or files not associated with pages (i.e. cache 
files, log files, etc.). Essentially, a site profile is meant to be a version of
a site you can share with others, that contains no confidential data like
user or password information. 

## How to use

Usage instructions are provided directly in the module when using it. After 
installing, go to "Setup > Export Site Profile" and it will guide you through the 
rest. 

### Using a custom install/finish.php file

ProcessWire 3.0.191+ supports a /site/install/finish.php file in the site profile
which is a plain PHP file that has access to most site API variables and can 
perform any finishing touches on the site. It is called after the installer finishes 
but before it deletes installer assets and displays the final status messages to the user. 

After exporting a site profile, feel free to modify the default install/finish.php 
file to suit your needs. 

---

Copyright 2024 by Ryan Cramer