# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [3.1.0]

### Added
- Ability to provide external Secret with credentials

## [3.0.1]

### Changed
- Fixed incorrect podAnnotations indentation

## [3.0.0]

### Added
- Support for Kubernetes 1.22
- New value `ingress.pathType` to control how the ingress path should be interpreted by the underlying load balancer.
- New value `ingress.ingressClassName` that replaces the old ingress annotation used to select the ingressClass.

### Removed
- Support for Kubernetes versions prior to 1.19

### Changed
- Helm api version
## [2.2.1]

### Fixed
- Can now pass in empty `auth.actions` without pypiserver erroring

## [2.2.0]

### Changed

- Allowed configuration of user and group
- Allowed mountPropagation field configuration for a PV

## [2.1.0]

### Changed

- Changed apiVersion of Deployment from extensions/v1beta1 to apps/v1 (not considered a breaking change as it's availble since v1.9)
- Changed apiVersion of Ingress from extensions/v1beta1 to networking.k8s.io/v1beta1 (not considered a breaking change as it's availble since v1.14)
- Fixing continuous integration

## [2.0.0]

### Breaking Changes

- `podLabels` replaces `deployment.labels`

### Added

- Added `podAnnotations` and `podLabels` to deployment template
- Added `apiVersion` to `Chart.yaml`

### Changed

- Bumped application version to `1.3.2`
- Changed comment in `values.yaml`

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
