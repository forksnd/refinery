# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.6.0]
### Changed
 - Only maps with opensauce headers will have their tags treated as OS_V4 on extraction now.
 - Fix "Queue all maps" button only queuing maps from the current selected engine.

## [2.5.1]
### Changed
 - Update build config for Python 3.9.

## [2.5.0]
### Added
 - Add button to queue all maps for extraction.
 - Add button to deprotect all loaded maps.

### Changed
 - Changed some action button names to be shorter and hopefully more clear.

## [2.4.1]
### Changed
 - (Linux) Fix directories not being sorted separately from tags.
 - Display pointers as HEX.
 - Don't tell people to run as admin when no tags were extracted.
 - Hopefully sped up tag sorting.
 - Name first column in hierarchy view 'name'.
 - Remove fallback icon and about image locations.
 - Fix missing license in distributions.
 - Default setting for generating compressed vertices is now True.

## [2.4.0]
### Added
 - Added \_\_main\_\_ so Refinery can be executed using `python -m refinery` or just `refinery` on some systems.

## [2.3.2]
### Changed
 - Fix readme potentially breaking setup.

## [2.3.1]
### Add
 - Project is now automatically built for pypi.

## [2.3.0] Into the GPLv3
Something that is very important to us is collaboration and the ability to share knowledge. Since this library is just to help mod some games, we've decided that switching to GPLv3 is the right thing to do for us to avoid any future loss of knowledge.

### Added
 - Add report bug button.
 - Michelle to the authors!
 - This changelog!

### Changed
 - All valid Halo 1 map types are now selected by default instead of having to click a few buttons to also see opensauce maps.
 - Config is now saved in current_working_directory/mek_config on Windows. And ~/.local/share/mek/ on Linux.
 - Data extraction mode can be entered without loading a map first now.
 - Fix a bunch of issues relating to different path separators between map files and the filesystem.
 - Fix sounds extracting incorrectly during data extraction.
 - Fix tag class deprotection failing on scenario tag.
 - Fix valid classes for explorers being set wrong if not in data extraction mode.
 - Make numerous path handling changes to support POSIX systems.
 - Refactor a bunch of the Refinery core.
 - Use kdialog whenever available instead of default tkinter filepicker.
 - Use pathlib Path objects where applicable to ease compatibility with multiple operating systems.
 - Various changes to work with new reclaimer codebase.
 - **THIS PROJECT IS NOW LICENSED UNDER THE GNU General Public License version 3**

### Removed
 - **REMOVED SUPPORT FOR VERSIONS OF PYTHON BELOW 3.5**
