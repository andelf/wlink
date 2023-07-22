# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- Support WCH-LinkW, a CH32V208 flasher with wireless connection
- Support WCH-Link firmware 2.9, some raw commands are changed
- Support Flash protect and unprotect (#14)
- Fix stuck for CH5xx devices, due to unsppported read ram rom split command
- Add `--chip` option to specify chip type
- Check probe type when doing mode-switch
- Add support for CH32X035
- Add support for CH59X

### Fixed

- Constraint regs for riscv32ec variant
- Wrong 0x0c command interpretation, this should be a set chip speed command

### Changed

- Refine error messages

## [0.0.4] - 2023-07-01

### Added

- Add `mode-switch` subcommand to switch between RV mode and DAP mode (#3)
- Add `hex`, `ihex` and `elf` format support for `flash` subcommand

### Fixed

- Fix communication parity error of abstractcs register (#16)
- Do not halt when read register

### Changed

- Refine attach chip logic, more robust now
- Refine docs

## [0.0.3] - 2023-03-01

### Added

- Everything just works