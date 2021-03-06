Changelog
=========

Unreleased
----------
* Removed React dependency

2.6.0 - (January 4, 2018)
----------
* Log reduced nightwatch output when running in CI.

2.5.0 - (January 3, 2018)
----------
* Lock axe-core to version 2.5

2.4.0 - (December 12, 2017)
------------------
* Lock webpack-dev-server at latest version that supported IE10 (2.7.1)

2.3.0 - (November 30, 2017)
------------------
### Added
* Added WebpackDevServerService to webdriver.io services

### Updated
* Updated nightwatch to use WebpackDevServerService
* Updated tests to use WebpackDevServerService instead of 'wdio-static-server'

2.2.0 - (November 15, 2017)
------------------
### Changed
* Use path.join to allow for windows development
* Removed sauce labs config and install java 8 in a different way for travis ci
* Added webdriver.io testing utilities
* Update nightwatch to use docker

2.1.0 - (October 5, 2017)
------------------
### Changed
* Refactored dependencies to make webpack and nightwatch peer dependencies.

2.0.0 - (August 31, 2017)
------------------
### Changed
* Nighwatch configuration is now available via a single file which allowed for the removal of the testSetting module. Configuration can now be created  by providing the webpack configuration, test folders and (optional) port number to the nightwatchConfig function.

## Added
* Added responsive nightwatch test helper functions. Functions include 1. resizeTo and 2. screenWidth.
1. resizeTo: Allows for breakpoint specification within the test suite and handles browser resizing function to allow for test to be run across each breakpoint specified.
2. screenWidth: returns the screen width grabbing the breakpoint tag specified within the current test description.

### Removed
* Removed screenshot capabilities
* Removed sauce capabilities
* Removed spectre capabilties
* Removed nightwatch test scripts
* Removed default webpack configuration

1.2.2 - (July 14, 2017)
------------------
### Changes
* Update output of aggregated translations to be placed within the site package for testing

1.2.1 - (July 13, 2017)
------------------
### Changes
* Change permission to 755 on executable scripts

1.2.0 - (July 13, 2017)
------------------
### Changes
* Remove post-install script which caused installation failure

1.1.0 - (June 28, 2017)
------------------
### Dependency Additions/Updates
* The following changes removed any coupling to the terra-core repository. Additionally, default configuration was added to webpack and nightwatch setup to remove the need for any nightwatch testing configuration at package level for terra components.
* Added webpack.config.js and nightwatch.conf.js files. These provides a default test setup for the nightwatch scripts. The webpack config file assumes package-level testing with examples living within the 'repo_name'-site package.
* Updated "globals_path" in nightwatch.json to assume package-level testing.
* Updated README to include versioning and added more explanation regarding toolkit abilities.

1.0.0 - (June 28, 2017)
------------------
Initial stable release
