# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.0.0] - 2021-09-03

### Added
- Support for Kubernetes 1.22.0
- Support for Helm APIVersion v2

### Removed
- Support for Kubernetes <=1.19.0
- Dependency to a deprecated postgresql chart
- Dependecy to a deprecated mysql chart
- Deployment of a database, you should now rely on sqlite or an external database
