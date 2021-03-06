# Change Log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/) 
and this project adheres to [Semantic Versioning](http://semver.org/).

i.e. \<Major version\>.\<Minor version\>.\<Patch version\>

The namespace of the schema includes the major version, e.g. _event-logging:3_. This is to reflect the fact that a change to the major version number is a breaking change and thus a different namespace should be used. Similarly the filename of the schema as a release artifact will include the major version number to reflect a breaking change.

Minor and patch versions will be backwards compatible with other versions at the same major version number. The minor and patch version numbers are included in the _version_ and _id_ attributes of the _xs:schema_ element.

Minor version changes may included new optional elements or attributes. They may also include changes to such things as enumerations or patterns that are additive in nature.

Patch version changes will typically include cosmetic changes (e.g. _xs:documentation_ changes. 

## [Unreleased]
### Added

### Changed

## [v3.1.1] - 2017-07-17

### Changed

* Issue **#18** : Remove `pattern` from `VersionSimpleType` as this is trumped by the enumerations. Add past versions as enumerations.


## [v3.1.0] - 2017-07-12

### Added

* Issue **#16** : Add _Data_ element to _PrintSettings_ element

* Issue **#13** : Add _Group_ to the list of items an _Authenticate_ action can occur on

* Issue **#12** : Add _ElevatePrivilege_ and _Other_ to list of _Authenticate_ Actions

* Issue **#6** : Add _PauseJob_, _ResumeJob_, _FailedPrint_ and _Other_ to _PrintActionSimpleType_

* Issue **#4** : Extend _ObjectOutcomeComplexType_ to have _Data_ sub elements

### Changed

* Issue **#5** : Change certain instances of _xs:positiveInteger_ to _xs:nonNegativeInteger_ to allow zero values

## [v3.0.0] - 2016-10-31

### Added

* Intial open source release

[Unreleased]: https://github.com/gchq/event-logging-schema/compare/v3.1.1...HEAD
[v3.1.1]: https://github.com/gchq/event-logging-schema/compare/v3.1.0...v3.1.1
[v3.1.0]: https://github.com/gchq/event-logging-schema/compare/v3.0.0...v3.1.0
[v3.0.0]: https://github.com/gchq/event-logging-schema/compare/v3.0.0...v3.0.0
