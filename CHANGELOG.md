# Changelog

## [0.4.4] - 2019-27-04

### Fix

 - mixins
   - shadow
     - Fix colors

## [0.4.3] - 2019-26-04

### Fix

 - global
   - color
     - Re-enable the color mixin

  - utilities
    - Import now the mixin to be able to work even if not imported by the user

## [0.4.2] - 2019-24-04

### Fix

 - utilities
   - color
     - Ctrl variable existence

## [0.4.1] - 2019-24-04

### Added

 - utilities
   - color
     - contrast-content

## [0.4.0] - 2019-24-04

### Added

 - utilities
   - customize-bg
   - color

### Removed (BREAKING CHANGE)

 - mixins
   - color
     - Utilities logic

## [0.3.6] - 2019-24-04

### Changed (Contain BUG)
  - mixins
    - color

## [0.3.4] - 2019-04-02

### Changed

 - color
   - Remove auto contrast

## [0.3.3] - 2019-04-02

### Changed

 - reset
   - Remove pointer

## [0.3.2] - 2019-03-26

### Changed

- color
  - Let the user set tint, shad, contrast and trans color directly

## [0.3.0] - 2019-03-02

### Added

- Utilities
  - customize-row

### Changed

- mixins
  - Every mixins inside mixins folder

### Deleted

- Global
  - Readme

## [0.2.8] - 2019-02-21

### Added

- Colors
  - bg now have his contrast as default color

## [0.2.7] - 2019-02-14

### Added

- Browser
  - @include chrome mixin

### Changed

- Browser
  - IE works now from version 6+ (was 9+)

## [0.2.5] - 2019-02-13

### Added

- Color
  - afterNBefore class (for ::after and ::before colors)

### Changed

- Color
  - Colors map is now us-colors (so we can use bootstrap at the same time)

## [0.2.2] - 2019-02-12

### Added

- Color
  - contrast
  - tint
  - shade

## [0.2.0] - 2019-02-11

### Changed

- Grid
  - Separated in to folder
    - Grid: Contain similar as bootstrap mixin
    - Browser: Contain browser specific mixin

### Remove

- Grid
  - "not" features for grid mixin

### Added

- Grid
  - [grid]Only and [grid]Up mixin
  - xs
  - xxl (up to 1'500px)

## [0.1.1] - 2019-02-08

### Added

- Mixins/animation

  - spin

- Helpers/reset
  - reset margin bottom to 0

## [0.1.0] - 2019-02-06

### Added

- Mixins

  - color
  - grid
  - shadow
  - animation

- Helpers
  - reset
