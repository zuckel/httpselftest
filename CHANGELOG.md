# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

<!-- Categories: Added, Changed, Deprecated, Removed, Fixed, Security -->

## [Unreleased]
- rework TestConfigs
### Changed
- implementing Servlets must now provide their configs as TestConfigs.Builder

## [0.3.3] - 2019-10-10
- don't flush writers early to prevent potential conflicts with e.g. Content-MD5 filters
- display presentation toggles only if there is more than one presentation

## [0.3.2] - 2019-09-05
- fixed query parameter handling on TestRequest (broken in 0.3.0 and 0.3.1)
- shade json-simple
- shade j2html
- render unhandled Throwables to html

## [0.3.1] - 2019-08-29
- added uncaught exception messages to JSON response
- added json presentation

## [0.3.0] - 2019-08-29
- added support for different request presentations
- added x-www-form-urlencoded presentation
- added hex response presentation
- added support for different response presentations

## [0.2.3] - 2019-05-02
- added support for unmodifiable test-provided parameters via `TestConfigs.fixed(..)`
- extended JSON response

## [0.2.2] - 2019-03-28
- fix artifact deployment to sonatype

## [0.2.1] - 2019-03-28
### Added
- Support SHA-256 for Basic auth. Use by prefixing credentials with `sha256|`, e.g. `selftest.credentials=sha256|a60ec1cf58f49cd2fab6d9e...`.

## [0.2.0] - 2019-02-22
### Added
- Dependency on Logback is now optional. Logging framework is configurable under `selftest.logger`, defaulting to logback.

## [0.1.0] - 2019-02-08
### Added
- First release
