# Changelog

## [8.0.0] - 2025-05-05
### Breaking change
- Dropped support of Python 3.8.
### Added
- Testing for Python 3.11, 3.12, and 3.13.
### Fixed
- Large paylod for ntfy notifier.
  Thanks to [wunter8](https://github.com/wunter8) in [PR#146](https://github.com/kibitzr/kibitzr/pull/146).

## [7.0.6] - 2024-01-05
### Added
- Support for ntfy notifier.
  Thanks to [wunter8](https://github.com/wunter8) in [PR#141](https://github.com/kibitzr/kibitzr/pull/141).

## [7.0.5] - 2023-03-29
### Fixed
- Restore CHANGELOG markup conversion

## [7.0.4] - 2023-03-29
### Fixed
- Update usage for the new version of telegram bot.
  Thanks to [Pan Luo](https://github.com/xcompass) in [PR#139](https://github.com/kibitzr/kibitzr/pull/139)

## [7.0.3] - 2023-03-23
### Fixed
- Update import path for the new version of telegram bot.
  [Issue#138](https://github.com/kibitzr/kibitzr/issues/138)

## [7.0.2] - 2023-02-24
### Added
- Support for Twilio notifier.
  Thanks to [Colin Unger](https://github.com/lockshaw) in [PR#137](https://github.com/kibitzr/kibitzr/pull/137)

## [7.0.1] - 2023-02-24
### Added
- Support for Discord webhook notifier.
  Thanks to [Iwa](https://github.com/mcrozz) in [PR#136](https://github.com/kibitzr/kibitzr/pull/136)

## [7.0.0] - 2022-07-19
### Removed
- Python 3.6 and 3.7 support.

### Added
- Python 3.10 support

## [6.2.1] - 2022-05-07
### Fixed
- Python version requirement (3.6+) for the package.

## [6.2.0] - 2022-05-07
### Changed
- SMTP notifier will not try to authenticate when either user or password is missing from configuration.
  Thanks to [QJKX](https://github.com/QJKX) in [PR#122](https://github.com/kibitzr/kibitzr/pull/122)

## [6.1.0] - 2022-01-28
### Added
- `kibitzr reload` command to pick up configuration changes without restart by [fi-do](https://github.com/fi-do) in [PR#115](https://github.com/kibitzr/kibitzr/pull/115)

## [6.0.2] - 2021-12-05
- Update docker image

## [6.0.1] - 2021-10-11
### Added
- [Gotify notifier](https://kibitzr.readthedocs.io/en/latest/gotify.html) by [egvimo](https://github.com/egvimo) in [PR#108](for://github.com/kibitzr/kibitzr/pull/108)

## [6.0.0] - 2019-08-06
### Removed
- Support for Python 2.6, 3.4

### Added
- Support for Python 3.7

## [5.4.4] - 2019-08-06
### Fixed
- skip handling of unsupported SIGUSR1 under Windows #73.

### Added
- provide context for `{{ env }}` dictionary in all Jinja templates.

## [5.4.3] - 2019-06-07
### Fixed
- Fixed `xpath` in Jinja transform for attribute and namespace access (#81 thanks to @mstarzyk).

## [5.4.2] - 2018-12-27
### Changed
- Better support for dynamic forms filling. Check only first form field for accessibility.
- Changed `bash` to `shell` in docs and added alias.

## [5.4.1] - 2018-11-27
### Changed
- Replaced option `verify_cert` with `verify-cert` for consistency.

## [5.4.0] - 2018-10-20
### Added
- Schedule option (#71 thanks to @cescobarresi).
- Option to omit HTTPS certificate verification in simple fetcher (#72 thanks to @cescobarresi).

## [5.3.5] - 2018-10-02
### Added
- Telegram notifier option `split-on` (#70 thanks to @cescobarresi).
### Changed
- Fixed `xpath` transform for attribute and namespace access (#68 thanks to @cescobarresi).

## [5.3.4] - 2018-09-28
### Added
- `xpath-all` transform (#67 thanks to @cescobarresi).

## [5.3.3] - 2018-08-24
### Added
- [undocumented] `before_start` extension interface.

## [5.3.2] - 2018-08-16
### Changed
- Made custom Jinja filters ignore None values.
- convert lxml to defusedxml in transformer/html.py (#61 thanks to @unit-00).

## [5.3.1] - 2018-07-06
### Added
- [undocumented] CLI extension interface.

## [5.3.0.alpha] - 2018-05-06
### Added
- [undocumented] fetcher extension interface.

## [5.2.0] - 2018-05-06
### Changed
- `kibitzr firefox` now prompts for Return to save profile.
- Firefox profile directory path moved to capabilities in the new version.

## [5.1.1] - 2018-04-19
### Added
- `kibitzr stash` command to show stash contents.

## [5.1.0] - 2018-04-10

### Added
- kibitzr clean command to delete changes history (#13 thanks to @attilanagy).
- Jinja filters: int and float.

## [5.0.0] - 2017-12-16
### Changed
- Dropped support for Firefox < 56 (using -headless instead of XVFB).

## [4.0.10] - 2017-08-28
### Changed
- Fix #47: Xpath transform encodes content to UTF-8 before parsing (X|HT)ML.

## [4.0.9] - 2017-08-21
### Fixed
- Allow SMTP without authentication.
### Changed
- Use local SMTP server by default.

## [4.0.8] - 2017-08-02
### Fixed
- Fixed xpath selector transform.

## [4.0.7] - 2017-06-29
### Fixed
- Fixed interruption exit code (1).

## [4.0.6] - 2017-06-28
### Fixed
- Exit(2) when receiving SIGTERM/SIGINT.

## [4.0.5] - 2017-06-14
### Fixed
- Exit(1) Kibitzr when Firefox goes funny business.

## [4.0.4] - 2017-06-07
### Changed
- Firefox fetcher: Implicitly wait 2 seconds for selects.
- Firefox fetcher: Resize window before each fetch.
### Fixed
- bash transform: Skip execution for empty content.

## [4.0.3] - 2017-05-25
### Added
- Changes style "new" - show only current content if it changed.
### Fixed
- text filter in Jinja templates.
- Adapted list of requirements for Windows.

## [4.0.2] - 2017-05-21
### Added
- Explicit telegram imprinting.
### Fixed
- Dynamically import only what's needed in checks.
- Better Windows support.
- Support for non-ascii URLs.

## [4.0.1] - 2017-05-10
### Added
- Credentials extensions through entry points (for kibitzr-keyring).

## [4.0.0] - 2017-05-08
### Added
- `kibitzr init` - create sample configuration files.
### Changed
- Changed kibitzr CLI commands structure (`kibitzr run` instead of `kibitzr`).

## [3.1.8] - 2017-05-08
### Fixed
- Unspecified period caused error (introduced in 3.1.4).

## [3.1.7] - 2017-05-06
### Fixed
- Gracefull shutdown on SIGTERM (as on SIGINT).

## [3.1.6] - 2017-05-05
### Fixed
- Jinja transform.
### Added
- CHANGELOG to PyPI page.

## [3.1.4] - 2017-05-04
### Changed
- human-readable period.

## [3.1.3] - 2017-05-01
### Fixed
- Bash and Python transforms parameter (dis)order.
- Skip Bash transform if input is empty.
### Changed
- Requests fetcher uses caching.

## [3.1.0] - 2017-05-01
### Added
- Jinja transform.
### Removed
- cut and sort transforms (superseded by bash).

## [3.0.11] - 2017-04-30
### Added
- Browser form filling shorthand.

## [3.0.10] - 2017-04-29
### Added
- Bash transform.
### Fixed
- jq transform input encoding.

## [3.0.9] - 2017-04-25
### Fixed
- Firefox fetcher: retry 3 times on stale element exception.
- Persistent Firefox: Ignore all exceptions when closing.

## [3.0.8] - 2017-04-24
### Added
- Transformer css-all selector which returns all elements instead of first.
- Python transformer.
### Changed
- Missing check name autopopulated from URL or autogenerated.

## [3.0.7] - 2017-04-19
### Added
- Zapier notifier.

## [3.0.6] - 2017-04-19
### Added
- Telegram notifier.

## [3.0.3] - 2017-04-18
### Added
- Persistent firefox profile [undocumented].

## [3.0.2] - 2017-04-18
### Added
- Short form for SMTP notifier #11.
### Fixed
- Weird BS4 misbehaviour in CSS selector.

## [3.0.1] - 2017-04-07
### Fixed
- Exit if no checks defined.
- Better credentials reloading.

## [3.0.0] - 2017-04-04
### Changed
- Switched to selenium >3 and Firefox >48.

## [2.7.4] - 2017-04-01
### Changed
- Closing FireFox tab after it was fetched to reduce idle CPU.

## [2.7.3] - 2017-03-31
### Added
- Started CHANGELOG.
- script.python fetcher.
