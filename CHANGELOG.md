# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.3.0] - 2026-02-11

### Added

- Functional options pattern for Prometheus `MonitoringService` (`NewMonitoringServiceWithOptions`)
- `WithRegistry` option to use an external `*prometheus.Registry` instead of the global default
- `WithRegisterer` option for lower-level registerer injection
- `WithListenAddress`, `WithRegion`, `WithLogger` options
- Graceful HTTP server shutdown in `MonitoringService.Shutdown()`
- HTTP server timeouts (read, idle) for Slowloris protection
- Tolerance for duplicate metric registration (`AlreadyRegisteredError`)
- Prometheus metrics example (`examples/prometheus-metrics/`)

## [0.2.1] - 2026-02-11

### Fixed

- Integer overflow in MaxRecords int to int32 conversion (polling-shard-consumer.go)

## [0.2.0] - 2026-02-11

### Added

- Redis-backed checkpointer as an alternative to DynamoDB
- Changelog version bump check in GitHub Actions CI

## [0.1.0] - 2026-02-11

### Changed

- Fork from vmware/vmware-go-kcl-v2
- Update module path to github.com/ODudek/go-kcl
- Bump minimum Go version to 1.21
- Upgrade AWS SDK and dependencies
