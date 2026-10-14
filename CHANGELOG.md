# Changelog

All notable changes to this integration are documented in this file. The format
follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and the project
uses [semantic versioning](https://semver.org/).

Describe each change under `## [Unreleased]` as you make it. The Release
workflow moves that section under the version it ships, and the section becomes
the notes of the version's GitHub Release.

## [Unreleased]

### Fixed

- Docs and the placeholder of the payload: a device value comes from the
  variable list (`{{0.0.last_value}}` after a "Get device value" action), not
  `{{device.<name>.temperature}}`, which Gladys does not know.

## [0.1.1] - 2026-10-13

### Added

- Scene actions "Trigger an IFTTT event" (event name, value1..value3) and
  "Trigger an IFTTT event (JSON)" (event name, JSON object), through the
  IFTTT Webhooks service.
- Scene trigger "IFTTT event received": an applet calls the inbound webhook
  relayed by Gladys Plus (JSON, form or query string), with an optional
  shared secret.
- Dashboard widget "IFTTT button".
- "Send a test event" button, which also shows the inbound URL.

[Unreleased]: https://github.com/LM1LC3N7/gladys-ifttt/compare/v0.1.1...HEAD
[0.1.1]: https://github.com/LM1LC3N7/gladys-ifttt/releases/tag/v0.1.1
