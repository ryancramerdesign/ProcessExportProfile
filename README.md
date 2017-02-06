# Profile Exporter for ProcessWire 2.5+

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
- System files in /site/ (ready.php, init.php, finished.php)

Site profiles do not include users or files not associated with pages (i.e. cache 
files, log files, etc.). Essentially, a site profile is meant to be a version of
a site you can share with others, that contains no confidential data like
user or password information. 

## How to use

Usage instructions are provided directly in the module when using it. After 
installing, go to Setup > Export Site Profile and it will guide you through the 
rest. 

## Requirements

This version of the profile exporter requires ProcessWire 2.5 or newer. If you 
need a profile exporter for an earlier version of ProcessWire, grab the 
[legacy branch](https://github.com/ryancramerdesign/ProcessExportProfile/tree/legacy) of this module. 

---

Copyright 2017 by Ryan Cramer

