[![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-no-red.svg)](https://bitbucket.org/lbesson/ansi-colors)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

# CardReaderProvider-NFC

An [CardReaderProvider](https://github.com/gematik/ref-CardReaderProvider-ApiKit.git) implementation that handles the
communication with the Apple Iphone NFC interface.

## Getting Started

CardReaderProvider-NFC requires Swift 5.1.

### Setup for integration:

-   **Carthage:** Put this in your `Cartfile`:

        github "gematik/ref-CardReaderProvider-NFC-iOS" ~> 1.0

### Setup for development

You will need [Bundler](https://bundler.io/), [XcodeGen](https://github.com/yonaskolb/XcodeGen), [Carthage](https://github.com/Carthage/Carthage)
and [fastlane](https://fastlane.tools) to conveniently use the established development environment.

1.  Update ruby gems necessary for build commands

        $ bundle install --path vendor/gems

2.  Checkout (and build) dependencies and generate the xcodeproject

        $ bundle exec fastlane setup

3.  Build the project

        $ bundle exec fastlane build_all [build_mac, build_ios]
