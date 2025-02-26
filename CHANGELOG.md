# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [v0.7.2](https://github.com/livebook-dev/livebook/tree/v0.7.2) (2022-10-26)

### Added

- Options to view and delete secrets in the session sidebar ([#1473](https://github.com/livebook-dev/livebook/pull/1473))
- Option to change the default file system in settings ([#1450](https://github.com/livebook-dev/livebook/pull/1450))

### Changed

- Improved CLI configuration for Attached runtime to support short node name without hostname ([#1474](https://github.com/livebook-dev/livebook/pull/1474))

### Fixed

- Relative URLs in HTML elements in Markdown ([#1491](https://github.com/livebook-dev/livebook/pull/1491))
- Units in byte formatting when showing memory usage ([#1494](https://github.com/livebook-dev/livebook/pull/1494))
- Fixed vendoring OTP in the desktop app ([#1495](https://github.com/livebook-dev/livebook/pull/1495))

## [v0.7.1](https://github.com/livebook-dev/livebook/tree/v0.7.1) (2022-10-09)

### Fixed

- Fixed editing Mermaid graphs in Markdown cells ([#1471](https://github.com/livebook-dev/livebook/pull/1471))

## [v0.7.0](https://github.com/livebook-dev/livebook/tree/v0.7.0) (2022-10-07)

### Added

- Added <kbd>Shift</kbd> + <kbd>Enter</kbd> (<kbd>⇧</kbd> + <kbd>↵</kbd>) for evaluating a cell and advancing to the next one ([#1294](https://github.com/livebook-dev/livebook/pull/1294))
- Support for composite outputs - tabs and grid ([#1326](https://github.com/livebook-dev/livebook/pull/1326) and [#1375](https://github.com/livebook-dev/livebook/pull/1375))
- Support for anchor links in notebook-relative navigation ([#1327](https://github.com/livebook-dev/livebook/pull/1327))
- Support for uploading SVG images in Markdown cells ([#1341](https://github.com/livebook-dev/livebook/pull/1341))
- Secrets management ([#1348](https://github.com/livebook-dev/livebook/pull/1348), [#1406](https://github.com/livebook-dev/livebook/pull/1406) and [#1441](https://github.com/livebook-dev/livebook/pull/1441))
- Completion for bitstring modifiers ([#1291](https://github.com/livebook-dev/livebook/pull/1291))
- Ability to configure global environment variables on the settings page ([#1387](https://github.com/livebook-dev/livebook/pull/1387) and [#1409](https://github.com/livebook-dev/livebook/pull/1409))
- Support for uploading files to the file system navigator via drag-and-drop ([#1422](https://github.com/livebook-dev/livebook/pull/1422))
- Universal desktop build for Mac and automated nightly builds

### Changed

- Redesigned the homepage sidebar ([#1325](https://github.com/livebook-dev/livebook/pull/1325))
- Package search to always list the exact match first ([#1355](https://github.com/livebook-dev/livebook/pull/1355))
- Renamed the Explore section to Learn ([#1424](https://github.com/livebook-dev/livebook/pull/1424))
- Reduced the number of clicks necessary to save a notebook ([#1458](https://github.com/livebook-dev/livebook/pull/1458))

### Removed

- Removed Mix standalone runtime in favour of the new `Mix.install/2` options, see [#1345](https://github.com/livebook-dev/livebook/pull/1345) to learn more ([#1370](https://github.com/livebook-dev/livebook/pull/1370))

### Fixed

- Fixed the "evaluate all" shortcut to work when a cells is evaluating ([#1334](https://github.com/livebook-dev/livebook/pull/1334))
- Source corruption when adding dependencies on Windows ([#1337](https://github.com/livebook-dev/livebook/pull/1337))
- Failure when changing file system from S3 to local ([#1377](https://github.com/livebook-dev/livebook/pull/1377))
- Evaluator to wait for garbage collected processes to terminate before next evaluation ([#1385](https://github.com/livebook-dev/livebook/pull/1385))
- Fixed unnecessary vertical whitespace in Mermaid graphs ([#1415](https://github.com/livebook-dev/livebook/pull/1415))
- Started ignoring non-Livebook logs in the Attached runtime ([#1451](https://github.com/livebook-dev/livebook/pull/1451))

## [v0.6.3](https://github.com/livebook-dev/livebook/tree/v0.6.3) (2022-07-13)

### Fixed

- Crashes when editing user profile on the homepage ([#1268](https://github.com/livebook-dev/livebook/pull/1268))
- Input change to be reflected immediately when clicking a button ([#1269](https://github.com/livebook-dev/livebook/pull/1269))
- JS outputs and smart cells when waking up from hibernation ([#1270](https://github.com/livebook-dev/livebook/pull/1270))

## [v0.6.2](https://github.com/livebook-dev/livebook/tree/v0.6.2) (2022-06-30)

### Added

- Session sidebar toggle on mobile ([#1183](https://github.com/livebook-dev/livebook/pull/1183))
- Support for configuring a custom iframe URL ([#1200](https://github.com/livebook-dev/livebook/pull/1200))
- Link to Hexdocs in on-hover docs ([#1221](https://github.com/livebook-dev/livebook/pull/1221))
- Capturing logs from processes outside Livebook supervision ([#1235](https://github.com/livebook-dev/livebook/pull/1235))
- Support HTML and CSS highlighting in Markdown cells ([#1244](https://github.com/livebook-dev/livebook/pull/1244) and [#1246](https://github.com/livebook-dev/livebook/pull/1246))
- MapLibre introductory notebook ([#1250](https://github.com/livebook-dev/livebook/pull/1250))
- Support for SQLite, Google BigQuery and AWS Athena under the well-known cells ([#1256](https://github.com/livebook-dev/livebook/pull/1256))

### Changed

- Default Livebook home path for Docker to `/data` ([#1191](https://github.com/livebook-dev/livebook/pull/1191))
- Mac app to run in the background ([#1199](https://github.com/livebook-dev/livebook/pull/1199))

### Fixed

- Memory monitoring to show the correct amount of free memory available on the system ([#1179](https://github.com/livebook-dev/livebook/pull/1179))
- Livebook access URL when running `livebook server` with custom `--ip` ([#1181](https://github.com/livebook-dev/livebook/pull/1181))
- Smart cell evaluation button in forked notebooks ([#1185](https://github.com/livebook-dev/livebook/pull/1185))
- Relative links in Markdown output ([#1189](https://github.com/livebook-dev/livebook/pull/1189))
- Docker startup when specifying `--user` ([#1193](https://github.com/livebook-dev/livebook/pull/1193))
- Support for `target="_blank"` links inside JS outputs and smart cells ([#1203](https://github.com/livebook-dev/livebook/pull/1203))
- Context menu in the file system component ([#1205](https://github.com/livebook-dev/livebook/pull/1205))
- Copying content with math syntax ([#1225](https://github.com/livebook-dev/livebook/pull/1225))
- Windows absolute paths when configuring Mix runtime via CLI ([#1242](https://github.com/livebook-dev/livebook/pull/1242))

## [v0.6.1](https://github.com/livebook-dev/livebook/tree/v0.6.1) (2022-05-06)

### Changed

- Stopped ignoring mouse events on crash ([#1168](https://github.com/livebook-dev/livebook/pull/1168))

### Fixed

- Added iframes to the Hex archive ([#1174](https://github.com/livebook-dev/livebook/pull/1174))

## [v0.6.0](https://github.com/livebook-dev/livebook/tree/v0.6.0) (2022-05-03)

### Added

- Code error highlighting on formatting and evaluation ([#948](https://github.com/livebook-dev/livebook/pull/948))
- Bulk actions in the sessions list ([#939](https://github.com/livebook-dev/livebook/pull/939))
- Support for opening files and URLs via `livebook server` args ([#947](https://github.com/livebook-dev/livebook/pull/947), [#969](https://github.com/livebook-dev/livebook/pull/969) and [#960](https://github.com/livebook-dev/livebook/pull/960))
- Persistent user configuration ([#937](https://github.com/livebook-dev/livebook/pull/937), [#1002](https://github.com/livebook-dev/livebook/pull/1002) and [#1017](https://github.com/livebook-dev/livebook/pull/1017))
- Word wrapping toggle to the editor ([#961](https://github.com/livebook-dev/livebook/pull/961))
- Option to download notebook source from the sessions list ([#980](https://github.com/livebook-dev/livebook/pull/980))
- Support for binary payloads in JS outputs ([#982](https://github.com/livebook-dev/livebook/pull/982))
- Introduced smart cells ([#1029](https://github.com/livebook-dev/livebook/pull/1029), [#1030](https://github.com/livebook-dev/livebook/pull/1030), [#1041](https://github.com/livebook-dev/livebook/pull/1041), [#1048](https://github.com/livebook-dev/livebook/pull/1048), [#1050](https://github.com/livebook-dev/livebook/pull/1050))
- Confirmation modals ([#1033](https://github.com/livebook-dev/livebook/pull/1033))
- Introduced desktop app packaging for Windows ([#1032](https://github.com/livebook-dev/livebook/pull/1032))
- Autosave path configuration on the settings page ([#1019](https://github.com/livebook-dev/livebook/pull/1019))
- Support for forcing SSL connection ([#1064](https://github.com/livebook-dev/livebook/pull/1064))
- Introduced a setup cell ([#1075](https://github.com/livebook-dev/livebook/pull/1075))
- Added cell insert buttons for a list of predefined smart cells ([#1078](https://github.com/livebook-dev/livebook/pull/1078) and [#1090](https://github.com/livebook-dev/livebook/pull/1090))
- UI for searching and adding new dependencies ([#1081](https://github.com/livebook-dev/livebook/pull/1081))
- An option for wrapping words in all Markdown editors ([#1107](https://github.com/livebook-dev/livebook/pull/1107))
- Support for `mix run` flags in the Mix runtime ([#1108](https://github.com/livebook-dev/livebook/pull/1108))
- Introduced code zen ([#1115](https://github.com/livebook-dev/livebook/pull/1115))
- Optional instance information when running in the cloud ([#1116](https://github.com/livebook-dev/livebook/pull/1116))
- Warning when running in the cloud and system memory is low ([#1122](https://github.com/livebook-dev/livebook/pull/1122))
- Notification when a new Livebook version is available ([#1121](https://github.com/livebook-dev/livebook/pull/1121))
- Insert button for Markdown cell with a Mermaid diagram ([#1134](https://github.com/livebook-dev/livebook/pull/1134))
- Taskbar icon for the desktop app ([#1119](https://github.com/livebook-dev/livebook/pull/1119))
- Notebook discussing Smart cells ([#1141](https://github.com/livebook-dev/livebook/pull/1141))

### Changed

- Notebook export file name to match notebook file or title ([#870](https://github.com/livebook-dev/livebook/pull/870))
- Switched importing to opening files in the desktop app ([#995](https://github.com/livebook-dev/livebook/pull/995))
- Renamed Elixir cell to Code cell ([#1035](https://github.com/livebook-dev/livebook/pull/1035))
- Use the first cell in viewport as the default for j/k navigation ([#1054](https://github.com/livebook-dev/livebook/pull/1054))
- Limit standard output to last 1000 lines ([#1063](https://github.com/livebook-dev/livebook/pull/1063))
- Restructured cell insert buttons ([#1073](https://github.com/livebook-dev/livebook/pull/1073))
- Allowed inserting images without specifying name in Markdown cells ([#1083](https://github.com/livebook-dev/livebook/pull/1083))
- Unified authentication to always redirect to the initial URL ([#1104](https://github.com/livebook-dev/livebook/pull/1104) and [#1112](https://github.com/livebook-dev/livebook/pull/1112))
- Erase outputs action to clear cell indicators ([#1160](https://github.com/livebook-dev/livebook/pull/1160))

### Removed

- `--open` and `--open-new` CLI flag to `livebook server` in favour of args ([#969](https://github.com/livebook-dev/livebook/pull/969) and [#960](https://github.com/livebook-dev/livebook/pull/960))
- `--autosave-path` in favour of `--data-path` ([#963](https://github.com/livebook-dev/livebook/pull/963))
- Disabled font ligatures in Markdown code blocks ([#1072](https://github.com/livebook-dev/livebook/pull/1072))
- Embedded runtime under the default configuration ([#1084](https://github.com/livebook-dev/livebook/pull/1084))

### Fixed

- Properly handle Cloud Storage S3 API operation responses ([#956](https://github.com/livebook-dev/livebook/pull/956))
- Access to cookies and other browser APIs inside JS output iframe ([#968](https://github.com/livebook-dev/livebook/pull/968), [#985](https://github.com/livebook-dev/livebook/pull/985) and [#989](https://github.com/livebook-dev/livebook/pull/989))
- Improved accessibility ([#979](https://github.com/livebook-dev/livebook/pull/979), [#1009](https://github.com/livebook-dev/livebook/pull/1009), [#1007](https://github.com/livebook-dev/livebook/pull/1007) and [#1010](https://github.com/livebook-dev/livebook/pull/1010))
- Editor input in Chrome when waking up from Windows hibernation ([#1018](https://github.com/livebook-dev/livebook/pull/1018))
- Improved input performance with multiple Mermaid diagrams in a Markdown cell ([#1023](https://github.com/livebook-dev/livebook/pull/1023))
- Opening browser from the CLI when running in WSL ([#1074](https://github.com/livebook-dev/livebook/pull/1074))

## [v0.5.2](https://github.com/livebook-dev/livebook/tree/v0.5.2) (2022-01-27)

### Added

- Allowed Livebook port to be set to 0 for a random port ([#906](https://github.com/livebook-dev/livebook/pull/906))
- Added memory usage information to runtime panel and sessions list ([#898](https://github.com/livebook-dev/livebook/pull/898), [#917](https://github.com/livebook-dev/livebook/pull/917) and [#918](https://github.com/livebook-dev/livebook/pull/918))
- Added support for font-awesome in mermaid.js diagrams ([#913](https://github.com/livebook-dev/livebook/pull/913))
- Support for reopening the desktop app ([#928](https://github.com/livebook-dev/livebook/pull/928))
- Added a warning when copying to clipboard fails ([#922](https://github.com/livebook-dev/livebook/pull/922))

### Changed

- App icon on macOS to look more native ([#924](https://github.com/livebook-dev/livebook/pull/924))
- Improved errors formatting ([#926](https://github.com/livebook-dev/livebook/pull/926))
- Improved intellisense to work while code is evaluating ([#941](https://github.com/livebook-dev/livebook/pull/941))
- Updated the release to run in interactive mode, hence using less memory ([#944](https://github.com/livebook-dev/livebook/pull/944))
- Updated the release to use a random cookie on every startup ([#944](https://github.com/livebook-dev/livebook/pull/944))

### Fixed

- Favicon rendering in Safari ([#920](https://github.com/livebook-dev/livebook/pull/920))
- Fixed code evaluation in the desktop app to work without Elixir installed globally ([929](https://github.com/livebook-dev/livebook/pull/929))
- Fixed line break support in Mermaid diagram definition ([932](https://github.com/livebook-dev/livebook/pull/932))
- Improved error handling in case of erroneous implementations of the `Inspect` protocol ([934](https://github.com/livebook-dev/livebook/pull/934))
- Fixed image insertion in Markdown cells when the image name includes special characters ([945](https://github.com/livebook-dev/livebook/pull/945))

## [v0.5.1](https://github.com/livebook-dev/livebook/tree/v0.5.1) (2022-01-20)

### Changed

- Changed the file system root path to $HOME in the desktop app ([#887](https://github.com/livebook-dev/livebook/pull/887))

### Fixed

- Loading JavaScript widgets when running behind a domain ([#902](https://github.com/livebook-dev/livebook/pull/902))

## [v0.5.0](https://github.com/livebook-dev/livebook/tree/v0.5.0) (2022-01-19)

### Added

- Support for input forms ([#790](https://github.com/livebook-dev/livebook/pull/790))
- Completion for struct keys ([#793](https://github.com/livebook-dev/livebook/pull/793))
- Support for custom JavaScript widgets ([#826](https://github.com/livebook-dev/livebook/pull/826))
- Introduced a dedicated Explore subsection for Kino guides ([#830](https://github.com/livebook-dev/livebook/pull/830))
- Added notebook name to page title ([#844](https://github.com/livebook-dev/livebook/pull/844))
- Added `@deprecated` and `@since` documentation metadata on mouse over ([#852](https://github.com/livebook-dev/livebook/pull/852))
- Added Livebook and Elixir version information to the Settings page ([#851](https://github.com/livebook-dev/livebook/pull/851))
- Added shutdown button to the sidebar ([#862](https://github.com/livebook-dev/livebook/pull/862))
- An option to increase the font size in the editor ([#860](https://github.com/livebook-dev/livebook/pull/860))
- An option to use a high-contrast editor theme ([#868](https://github.com/livebook-dev/livebook/pull/868) and [#871](https://github.com/livebook-dev/livebook/pull/871))
- Support for rendering mermaid.js graphs in Markdown cells ([#816](https://github.com/livebook-dev/livebook/pull/816))
- Introduced desktop app packaging for macOS ([#865](https://github.com/livebook-dev/livebook/pull/865))

### Changed

- Removed confirmation step when deleting an empty section ([#829](https://github.com/livebook-dev/livebook/pull/829))
- Applied several design improvements ([#858](https://github.com/livebook-dev/livebook/pull/858), [#859](https://github.com/livebook-dev/livebook/pull/859) and [#882](https://github.com/livebook-dev/livebook/pull/882))
- Changed the color scheme in text outputs to improve contrast ([#864](https://github.com/livebook-dev/livebook/pull/858) and [#859](https://github.com/livebook-dev/livebook/pull/864))
- Reworked Kino guides in the Explore section ([#879](https://github.com/livebook-dev/livebook/pull/858) and [#859](https://github.com/livebook-dev/livebook/pull/879))

### Fixed

- Disallowed saving notebooks with empty file name ([#823](https://github.com/livebook-dev/livebook/pull/823))
- Fixed unexpected focus behaviour in large editors ([#831](https://github.com/livebook-dev/livebook/pull/831))
- Fixed Escape key to exit multi-cursor mode ([#833](https://github.com/livebook-dev/livebook/pull/833))
- Improved error reports when reconnecting Mix runtime fails ([#837](https://github.com/livebook-dev/livebook/pull/837))
- Fixed code blocks in Markdown to use monospaced font for all characters ([#855](https://github.com/livebook-dev/livebook/pull/855))

## [v0.4.1](https://github.com/livebook-dev/livebook/tree/v0.4.1) (2021-12-09)

### Added

- Added <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Enter</kbd> (<kbd>⌘</kbd> + <kbd>⇧</kbd> + <kbd>↵</kbd>) for evaluating current and all outdated cells ([#766](https://github.com/livebook-dev/livebook/pull/766))

### Changed

- Disabled word suggestions on Elixir cells ([#763](https://github.com/livebook-dev/livebook/pull/763))

### Fixed

- Fixed error on back navigation after closing a session ([#769](https://github.com/livebook-dev/livebook/pull/769))
- Fixed disappearing indentation when pasting code into the editor ([#779](https://github.com/livebook-dev/livebook/pull/779))

## [v0.4.0](https://github.com/livebook-dev/livebook/tree/v0.4.0) (2021-12-05)

### Added

- Support for file scheme when importing notebook from URL ([#706](https://github.com/livebook-dev/livebook/pull/706))
- Support for rendering UI controls, such as buttons and keyboard ([#710](https://github.com/livebook-dev/livebook/pull/710))
- Added Pong notebook to the explore section to showcase controls ([#729](https://github.com/livebook-dev/livebook/pull/729))
- Improved function completion to insert parentheses ([#693](https://github.com/livebook-dev/livebook/pull/693))
- Added user-specific intellisense configuration ([#693](https://github.com/livebook-dev/livebook/pull/693))
- Added signature completion ([#640](https://github.com/livebook-dev/livebook/pull/640))
- Added automatic persistence for unsaved notebooks ([#736](https://github.com/livebook-dev/livebook/pull/736))
- Support XML and JSON highlighting in Markdown cells ([#743](https://github.com/livebook-dev/livebook/pull/743))

### Changed

- Restructured j/k navigation to support headlines ([#707](https://github.com/livebook-dev/livebook/pull/707))
- Migrated inputs to Kino ([#714](https://github.com/livebook-dev/livebook/pull/714))

### Removed

- Removed input cells in favour of `Kino.Input`, see [#714](https://github.com/livebook-dev/livebook/pull/714) for more details

### Fixed

- Fixed evaluation timer reset on page refresh ([#732](https://github.com/livebook-dev/livebook/pull/732))
- Fixed alignment of long names in the sections panel ([#734](https://github.com/livebook-dev/livebook/pull/734))
- Fixed timeout when importing a notebook with Vega-Lite output ([#741](https://github.com/livebook-dev/livebook/issues/741))

## [v0.3.2](https://github.com/livebook-dev/livebook/tree/v0.3.2) (2021-11-10)

### Added

- An option to clear evaluation outputs ([#661](https://github.com/livebook-dev/livebook/pull/661))
- Evaluation indicators to the sections side panel ([#657](https://github.com/livebook-dev/livebook/pull/657))
- Support for importing a notebook via file upload ([#665](https://github.com/livebook-dev/livebook/pull/665))
- Show/hide button to password inputs ([#664](https://github.com/livebook-dev/livebook/pull/664))
- Improved new directory creation under high latency ([#674](https://github.com/livebook-dev/livebook/pull/674))
- Enabled persisting static Vega-Lite plot to Live Markdown ([#676](https://github.com/livebook-dev/livebook/pull/676))
- Support for animable frame output ([#688](https://github.com/livebook-dev/livebook/pull/688))
- An option to amplify cell outputs ([#689](https://github.com/livebook-dev/livebook/pull/689))
- Included CMake in the Docker image ([#694](https://github.com/livebook-dev/livebook/pull/694))
- Environment variable for disabling token auth ([#696](https://github.com/livebook-dev/livebook/pull/696))

### Changed

- Redesigned save to file modal ([#663](https://github.com/livebook-dev/livebook/pull/663))
- Moved current runtime information into a new side panel ([#692](https://github.com/livebook-dev/livebook/pull/692))

### Fixed

- Rendering math with KaTeX that uses SVGs ([#684](https://github.com/livebook-dev/livebook/pull/684))

## [v0.3.1](https://github.com/livebook-dev/livebook/tree/v0.3.1) (2021-10-27)

### Added

- Introduced automatically reevaluating cells ([#637](https://github.com/livebook-dev/livebook/pull/637))

### Changed

- Changed color for aborted and queued cell status ([#620](https://github.com/livebook-dev/livebook/pull/620))
- Improved Markdown rendering of task and nested lists ([#623](https://github.com/livebook-dev/livebook/pull/623) and [#623](https://github.com/livebook-dev/livebook/pull/631))

### Fixed

- Connecting to an empty S3 bucket ([#646](https://github.com/livebook-dev/livebook/pull/623) and [#623](https://github.com/livebook-dev/livebook/pull/646))
- Importing notebooks served with `application/octet-stream` content type ([#650](https://github.com/livebook-dev/livebook/pull/623) and [#623](https://github.com/livebook-dev/livebook/pull/650))

### Removed

- Removed the keyboard shortcut for "Evaluate cells below" ([#621](https://github.com/livebook-dev/livebook/pull/621))
- Removed reactive inputs in favour of automatically reevaluating cells ([#649](https://github.com/livebook-dev/livebook/pull/649))

## [v0.3.0](https://github.com/livebook-dev/livebook/tree/v0.3.0) (2021-10-19)

### Added

- Introduced file system abstraction and an S3 support ([#492](https://github.com/livebook-dev/livebook/pull/492))
- Added support for configuring file systems using env variables ([#498](https://github.com/livebook-dev/livebook/pull/498))
- Added a keyboard shortcut for triggering on-hover docs ([#508](https://github.com/livebook-dev/livebook/pull/508))
- Added `--open-new` CLI flag to `livebook server` ([#529](https://github.com/livebook-dev/livebook/pull/529))
- Nx introductory notebook ([#528](https://github.com/livebook-dev/livebook/pull/528))
- Display creation date of a session in home ([#593](https://github.com/livebook-dev/livebook/pull/593))
- Dynamic favicon reflecting session state ([#594](https://github.com/livebook-dev/livebook/pull/594))

### Changed

- Improved intellisense to handle structs and sigils ([#513](https://github.com/livebook-dev/livebook/pull/513))
- Create new notebooks with an already focused code cell ([#527](https://github.com/livebook-dev/livebook/pull/527))
- Switched base Docker image from alpine to debian-slim ([#552](https://github.com/livebook-dev/livebook/pull/552))
- Update matching brackets style ([#595](https://github.com/livebook-dev/livebook/pull/595))

### Fixed

- Improved Markdown and math integration by migrating to remark ([#495](https://github.com/livebook-dev/livebook/pull/495))
- Improved the evaluator process to not consume user-submitted messages from inbox ([#502](https://github.com/livebook-dev/livebook/pull/502))
- Improved sections panel UI to better handle numerous sections or long section names ([#534](https://github.com/livebook-dev/livebook/pull/534) and [#537](https://github.com/livebook-dev/livebook/pull/537))
- Fixed branching section evaluation when the parent section is empty ([#560](https://github.com/livebook-dev/livebook/pull/560))
- Fixed ANSI support to handle multi-code escape sequences ([#569](https://github.com/livebook-dev/livebook/pull/569))

## [v0.2.3](https://github.com/livebook-dev/livebook/tree/v0.2.3) (2021-08-12)

### Added

- Added UI for directory creation ([#424](https://github.com/livebook-dev/livebook/pull/424))
- Added UI for file deletion and renaming ([#426](https://github.com/livebook-dev/livebook/pull/426))
- Listing Livebook version on dashboard home
- Support for relative navigation between notebooks ([#441](https://github.com/livebook-dev/livebook/pull/441) and [#445](https://github.com/livebook-dev/livebook/pull/445))
- Introduced branching sections ([#449](https://github.com/livebook-dev/livebook/pull/449))
- Range (slider) input ([#435](https://github.com/livebook-dev/livebook/pull/435) and [#440](https://github.com/livebook-dev/livebook/pull/440))
- Select input ([#448](https://github.com/livebook-dev/livebook/pull/448))
- Checkbox input ([#461](https://github.com/livebook-dev/livebook/pull/461))
- Showing full documentation when hovering over an identifier ([#453](https://github.com/livebook-dev/livebook/pull/453))
- Added notebook source preview and export ([#457](https://github.com/livebook-dev/livebook/pull/457))
- Added Elixir source export ([#476](https://github.com/livebook-dev/livebook/pull/476))
- Added option to export and persist Live Markdown with output ([#483](https://github.com/livebook-dev/livebook/pull/483) and [#485](https://github.com/livebook-dev/livebook/pull/485))

### Changed

- Merge undo stack for collaborative editing ([#433](https://github.com/livebook-dev/livebook/pull/433))
- Restructured remote node processes to allow for multiple connections ([#434](https://github.com/livebook-dev/livebook/pull/434))

### Fixed

- Fixed editor font size on MacOS

## [v0.2.2](https://github.com/livebook-dev/livebook/tree/v0.2.2) (2021-07-01)

### Added

- Support for configuring Attached as the default runtime ([#397](https://github.com/livebook-dev/livebook/pull/397))
- Textarea input ([#382](https://github.com/livebook-dev/livebook/pull/382))
- Color input ([#410](https://github.com/livebook-dev/livebook/pull/410))
- Support for markdown output ([#404](https://github.com/livebook-dev/livebook/pull/404))
- Introduced cells bin for restoring deleted cells ([#414](https://github.com/livebook-dev/livebook/pull/414))
- Added code formatting integration to Elixir cells ([#416](https://github.com/livebook-dev/livebook/pull/416))
- Added `--open` CLI flag to `livebook server` ([#417](https://github.com/livebook-dev/livebook/pull/417))
- Suggest restarting runtime on Mix.install error and add restart shortcut ([#418](https://github.com/livebook-dev/livebook/pull/418))
- Documented editor shortcuts and added basic view ([#419](https://github.com/livebook-dev/livebook/pull/419))

### Changed

- Improved section management ([#411](https://github.com/livebook-dev/livebook/pull/411))
- Highlight matching brackets only in insert mode ([#421](https://github.com/livebook-dev/livebook/pull/421))

## [v0.2.1](https://github.com/livebook-dev/livebook/tree/v0.2.1) (2021-06-24)

### Added

- Showing the evaluation time next to the cell indicator ([#366](https://github.com/livebook-dev/livebook/pull/366))
- Showing a ticking timer while cell is evaluating ([#374](https://github.com/livebook-dev/livebook/pull/374))
- Added a section on evaluation vs compilation to the Elixir notebook ([#376](https://github.com/livebook-dev/livebook/pull/376))
- Support for image output ([#380](https://github.com/livebook-dev/livebook/pull/380))
- Introduced reactive inputs ([#389](https://github.com/livebook-dev/livebook/pull/389))
- Added copy to clipboard button to virtualized output ([#393](https://github.com/livebook-dev/livebook/pull/393))

## [v0.2.0](https://github.com/livebook-dev/livebook/tree/v0.2.0) (2021-06-17)

Next milestone, see [New in Livebook v0.2 by José Valim](https://www.youtube.com/watch?v=MOTEgF-wIEI).

### Added

- Introduced an Explore section ([#310](https://github.com/livebook-dev/livebook/pull/310))
- Notebook about the unique features behind Elixir and Livebook ([#314](https://github.com/livebook-dev/livebook/pull/314))
- Portal guide ([#328](https://github.com/livebook-dev/livebook/pull/318))
- VegaLite introductory notebook ([#335](https://github.com/livebook-dev/livebook/pull/335))
- Kino introductory notebook ([#364](https://github.com/livebook-dev/livebook/pull/364))
- Notebook on VM introspection ([#346](https://github.com/livebook-dev/livebook/pull/346))
- Show an informative message on completion when there is no runtime ([#316](https://github.com/livebook-dev/livebook/pull/316))
- Support for inputs ([#328](https://github.com/livebook-dev/livebook/pull/328))
- Numeric input ([#352](https://github.com/livebook-dev/livebook/pull/352))
- Password input ([#357](https://github.com/livebook-dev/livebook/pull/357))
- Support for Mix runtime as the default one ([#334](https://github.com/livebook-dev/livebook/pull/334))
- Dynamic table output ([#356](https://github.com/livebook-dev/livebook/pull/356))

## [v0.1.2](https://github.com/livebook-dev/livebook/tree/v0.1.2) (2021-06-01)

### Added

- Capture and show logger output ([#298](https://github.com/livebook-dev/livebook/pull/298))
- Support for dynamic Vega-Lite graphics ([#306](https://github.com/livebook-dev/livebook/pull/306) and [#309](https://github.com/livebook-dev/livebook/pull/309))

## [v0.1.1](https://github.com/livebook-dev/livebook/tree/v0.1.1) (2021-05-24)

### Added

- Support for plots rendering via [`VegaLite`](https://github.com/elixir-nx/vega_lite) ([#287](https://github.com/livebook-dev/livebook/pull/287))

### Changed

- Improved path selector to properly handle text editing in the middle ([#283](https://github.com/livebook-dev/livebook/pull/283))
- Made section anchor links deterministic ([#288](https://github.com/livebook-dev/livebook/pull/288))

## [v0.1.0](https://github.com/livebook-dev/livebook/tree/v0.1.0) (2021-05-19)

Initial release, see [Livebook's announcement by José Valim](https://www.youtube.com/watch?v=RKvqc-UEe34).
