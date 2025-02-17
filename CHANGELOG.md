<!-- Keep a Changelog guide -> https://keepachangelog.com -->

# excalidraw-jetbrains-plugin Changelog

## [Unreleased]
### New
- Toggle between light and dark separated from the current theme by @michael-pratt, see [#92](https://github.com/bric3/excalidraw-jetbrains-plugin/pull/92) 

### Changed
- New plugin icon, matching the new excalidraw icon
- Upgraded excalidraw to version 0.16.0
- Opens Excalidraw editor rather than JSON by @michael-pratt, see [#93](https://github.com/bric3/excalidraw-jetbrains-plugin/pull/93) 

## [0.3.2] - 2021-09-14
### New
- This version is the first public release of the excalidraw integration.
  
  This version supports the edition of `.excalidraw`, and embedded excalidraw
  in `svg` and `png` image files. This plugin is engineered to be able to work 
  offline, consequently online collaboration is not supported.
  
  Contributions are welcome: Excalidraw library support, plugin settings, switch 
  to [excalidraw.com](https://excalidraw.com) (thus enabling collaboration), etc.
  Please check out the [project](https://github.com/bric3/excalidraw-jetbrains-plugin).

## [0.3.2-eap] - 2021-09-11
### Fixed
- Incorrect editor selected in split panes ([#11](https://github.com/bric3/excalidraw-jetbrains-plugin/issues/13))

## [0.3.1-eap] - 2021-08-12
### Fixed
- Fixed compatibility issue with 2021.1.x

## [0.3.0-eap] - 2021-08-11
### Added
- SVG and PNG exports are now saved with an embedded scene (always on) ([#11](https://github.com/bric3/excalidraw-jetbrains-plugin/issues/11))
- SVG and PNG files an embedded scene are recognized and can be loaded in the editor ([#12](https://github.com/bric3/excalidraw-jetbrains-plugin/issues/12))
- Modified excalidraw files marker if _Mark Modified (*)_ is ticked (in _Preferences | Editor | General | Editor Tabs_)

### Changed
- The Excalidraw webapp is now written in typescript
- The Excalidraw webapp now inline sourcemaps to enable 
  debugging within the JCEF DevTools, this was impossible due to a bug in chromium
  (see [#7](https://github.com/bric3/excalidraw-jetbrains-plugin/issues/7))
- Refactored how editor are auto-saved, now using IntelliJ's built-in mechanism.

## [0.2.0-eap] - 2021-07-01
### Added
- Save drawing to SVG or PNG (without the Excalidraw scene metadata) ([#3](https://github.com/bric3/excalidraw-jetbrains-plugin/issues/3))
- Options when saving to image (background color, dark mode, watermark) ([#9](https://github.com/bric3/excalidraw-jetbrains-plugin/issues/9))
- Options to display the grid or to toggle the zen mode ([#8](https://github.com/bric3/excalidraw-jetbrains-plugin/issues/8))

### Fixed
- Fixed a bug that prevented to open JSON files, the code is trying to identify Excalidraw JSON files (#5)

## [0.1.0-eap] - 2021-06-25
### Added
- Initial support of Excalidraw integration in JetBrains IDEs :
  create, open (with autosave) `.excalidraw` (json) files.