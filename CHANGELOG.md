# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

- [Oban] - Execution errors are stored as a jsonb array for each job. Each error
  is stored, not just the most recent one. Error entries contains these keys:
  - `at` The utc timestamp when the error occurred at
  - `attempt` The attempt number when the error ocurred
  - `error` A formatted error message and stacktrace

## [0.1.0] - 2019-03-10

- [Oban] Initial release with base functionality.

[Unreleased]: https://github.com/sorentwo/oban/compare/v0.1.0...HEAD
[0.1.0]: https://github.com/sorentwo/oban/compare/0ac3cc8...v0.1.0