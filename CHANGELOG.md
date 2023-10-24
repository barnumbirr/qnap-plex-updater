# Changelog

All notable changes to this project will be documented in this file.

This file format is loosely based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).\
This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### New
### Changes
### Deprecated
### Removed
### Fixes
### Security

## [1.0.1] - 24-10-2023

### Fixes

- fix default value for `${LOCAL_PLEX_VERSION}`

## [1.0.0] - 30-10-2022

### New

- use `-n / --notify` to output QTS/QuTS notice board notification on successful install

### Fixes

- set default value for `${LOCAL_PLEX_VERSION}`

## [0.3.2] - 24-06-2022

### New

- Add 'Prerequisites' section to `README`

### Fixes

- Fix path in `README` usage instructions (Closes: #2)
- Replace BASH parameter expansion with good ol' trusty `awk` (Closes: #1)

## [0.3.1] - 07-06-2022

### Fixes

- Stop PMS to prevent script being killed

## [0.3.0] - 06-06-2022

### New

- Specify package download directory using `-d/--directory <path>`

## [0.2.0] - 03-06-2022

### New

- `AARCH` and `REGEX_PLEX_VERSION` variables

### Changes

- Return `$AARCH` in Plex Media Server version

### Fixes

- Fix `[[ ]]` string comparisons

## [0.1.0] - 31-05-2022

Initial release.
