# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0]

### Added

- Ability to add labels to deployments/pods:
  The deployment.labels map is applied to the deployment and the pods

- Ability supply additional command line arguments to pypiserver:
  The pypiserver.extraArgs list is added to the pypiserver startup command

### Changed

- Default appVersion (version of pypiserver) is now 1.3.0

### Removed

## [1.0.1]

### Added

- Bug fix: Setting fsGroup to 1000 in case of enabled persistence
  (due to possibly missing write permissions as volumes are mounted as root owned folder by docker)

### Changed

### Removed
