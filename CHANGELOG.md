# Changelog

## [3.1.1] -- 2023-04-13

* updated dependencies:
  * mypy
  * pytest
  * pytest-cov
  * wheel
* Debian:
  * added htmlcov and .mypy_cache to extended-diff-ignore
  * bump debhelper from 11 -> 13
  * use debhelper-compat
  * use standards-version 4.6.2

## [3.1.0] -- 2022-09-07

* added type hints and mypy --strict to test suite
* updated dependencies:
  * flake8
  * pytest
  * twine

## [3.0.1] - 2022-06-26

* bumped version (no changes)

## [3.0.0] - 2022-05-31

* removed python 3.6 support
* added dependabot
* updated makefile

## [2.2.0] - 2020-10-30

* Allow for missing .env file -- in this case the command will be executed
  without setting any environment variables. The previous behaviour was to
  fail with a FileNotFoundError
* Migrated from TravisCI to github actions. We test now on Linux, Mac and
  Windows x all supported Python versions!
* Fixed tests under windows, where NamedTemporaryFile cannot be opened twice.
* refactored __main__.py into cli.py and wrapped argparsing into dedicated
  function
* bumped minimal Python version to 3.6
* Added 3.8, 3.9 to travis tests
* Cleaned up Makefile
* Added twine to dev-dependencies

## [2.1.0] - 2020-10-27

* make sure child process terminates when dotenv terminates
* measure coverage for tests as well
* skip coverage report for files w/ complete coverage
* use twine for uploading to pypi

## [2.0.1] - 2019-09-07

* Version bump for Debian source-only upload

## [2.0.0] - 2019-08-03

* Differentiate single vs double quotes

## [1.3.0] - 2019-05-11

* Support for lines starting with `export`
* Support for empty values

## [1.2.0] - 2019-05-10

* Fixed newlines
* Added more tests


## [1.1.0] - 2019-04-28

* Added Bash completion and provide it via sdist and Debian package


## [1.0.2] - 2019-04-14

* Debian package
* Fixed Travis-CI pipeline and added tests for py37


## [1.0.0] - 2018-10-14

* Initial Release
