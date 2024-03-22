# ProcessExportProfile changelog

## v5.0.0

- Added support for updating an existing profile. When an existing profile 
  is present, it will let you know and give you an "Update" button you can 
  click to re-export the entire profile in 1 click, using all the settings 
  from the existing profile. Requires using the "server directory" option.
 
- Added support for previewing an existing profile. It shows you what the 
  profile looks like from the ProcessWire installer (screenshot, etc.)

- Fixed issue with the ZIP profiles where they could omit status files like 
  /site/ready.php and /site/init.php. 
 
- Various other minor fixes and updates. 

## v4.0.1

- Added the ability to support a finish.php file that is called after the 
  installer finishes. Use this to make any final adjustments to the profile 
  following installation. See the README file for more details on this. 
  Requires ProcessWire 3.0.191+.

## Earlier versions

- See the commit log at:
  <https://github.com/ryancramerdesign/ProcessExportProfile/commits/master/>