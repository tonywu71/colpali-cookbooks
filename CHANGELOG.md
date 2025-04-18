# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog],
and this project adheres to [Semantic Versioning].

## [Unreleased]

### Added

- Add ruff linter/formatter CI job.

### Changed

- Fix broken GitHub-rendered notebooks.

## [0.4.0] - 2024-12-17

### Added

- Add cookbook for using the 🤗 transformers-native implementation of ColPali

## [0.3.1] - 2024-11-17

### Changed

- Change the example query in the E2E RAG cookbook

## [0.3.0] - 2024-11-17

### Added

- Add cookbook for E2E RAG with ColQwen2 and adapter hot-swapping

## [0.2.1] - 2024-11-11

### Changed

- Load example image from Git URL if no image path is provided in similarity map cookbooks

### Fixed

- Add missing `interpretability` optional deps for similarity map cookbooks

## [0.2.0] - 2024-10-12

### Added

- Add a similarity map generation notebook for ColQwen2
- Use `colpali-engine>=0.3.2` instead of `vidore-benchmark` in the ColPali similarity map notebook

### Changed

- Improve the similarity map generation notebook for ColPali

## [0.1.0] - 2024-10-11 - Initial Release

### Added

- Add similarity map generation notebook for ColPali
- Add fine-tuning notebook for ColPali

<!-- Links -->
[keep a changelog]: https://keepachangelog.com/en/1.0.0/
[semantic versioning]: https://semver.org/spec/v2.0.0.html
