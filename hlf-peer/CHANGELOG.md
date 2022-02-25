# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [5.1.0] - 2022-02-17

### Added
- Added `FABRIC_LOGGING_SPEC` to env through configmap which is the preferred mechanism for logging : https://hyperledger-fabric.readthedocs.io/en/release-2.2/logging-control.html#logging-specification
- Added annotations to services

## [5.0.0] - 2021-10-13

### Changed
- Allows configuring couchdb without hlf-couchdb chart with `couchdbService` and `couchdbPort`


## [4.0.1] - 2021-09-09

### Added
- Support for 1.19.x pre-releases

## [4.0.0] - 2021-09-06

### Added
- Support for Kubernetes 1.22.0
- Support for Helm APIVersion v2

### Removed
- Support for Kubernetes <=1.19.0

## [3.2.0]

### Added
- `couchdbInstance` is necessary for the connection with the peer

## [3.1.0]

### Added
- `pullImageSecret` is added to be able to pull image from a private registry

## [3.0.0]

### Breaking changes
- `couchdbSecret` replaces `couchdbInstance` to make the value explicit
