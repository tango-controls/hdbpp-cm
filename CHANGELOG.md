# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [2.0.0] - 2020-05-13

### Added
* New CMake build system that can download libhdbpp when requested
* Clang integration

### Changed
* Small refactoring and code modernization to get rid of some clang warnings.
* Remove libhdbpp dependency.
* Updated README for new build system
* Observe new namespace in libhdbpp
* Changed libhdbpp includes to new path (hdb++) and new split header files
* Project now links directly to given libhdbpp soname major version
* Made compatible with new libhdbpp (namespace, function and path changes)

### Fixed

* Fix potential crash in HdbConfigurationManager::add_domain [#6](https://github.com/tango-controls-hdbpp/hdbpp-cm/issues/6)

## [1.0.0] - 2017-09-28

### Added

* CHANGELOG.md file.
* Debian Package build files under debian/

### Changed

* Makefile: Added install rules, clean up paths etc
* Makefile: Cleaned up the linkage (removed unneeded libraries, libzmq, libCOS)
* Cleaned up some unused variable warnings
* libhdb++ include paths to match new install location.
* Updated README.md.

### Removed

* libhdbpp submodule. This now has to be installed manually.
