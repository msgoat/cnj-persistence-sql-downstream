# Changelog
All notable changes to `cnj-persistence-sql-downstream` will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [2.1.0] - 2023-08-24
### Added
- added explicit dependency to CloudTrain Maven repository to POM to simplify local builds
- allowed anonymous read access to CloudTrain Maven repository to simplify local builds
- added global docker-compose.yml file to simplify local execution
### Changed
- improved documentation in README.md
- upgraded cnj-common-security-oidc-spring to 2.2.0
- upgraded cnj-common-observability-spring to 1.1.0
- added support of static OpenAPI specification files accessible via URI `openapi`

## [2.0.0] - 2023-06-05
### Changed
- moved to new AWS CodeBuild build pipeline
- moved to new CloudTrain EKS cluster
- upgraded everything

## [1.1.0] - 2022-09-09
### Added
### Changed
- re-released after repo split
- renamed to cnj-persistence-sql-downstream (dropping the `-spring` suffix) to be more consistent with other showcases
- added cnj-common-observability-spring to have request/response tracing
