---
description: >-
  A release is made up from a collection of components and their versions that
  together make up the Sofie system.
---

# Releases

| Release                                                              | Status                                           |
| :------------------------------------------------------------------- | :----------------------------------------------- |
| Release 26                                                           | In Planning                                      |
| [Release 25](releases.md#release-25)                                 | In testing                                       |
| [Release 24](releases.md#release-24)                                 | _Released 2020-09-28 **Current stable version**_ |
| [Release 23](releases.md#release-23-skipped)                         | Skipped                                          |
| [Release 22](releases.md#release-22)                                 | Released 2020-08-17                              |
| [Release 21](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/17) | Skipped                                          |
| [Release 20](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/16) | _Released 2020-05-12_                            |
| [Release 19](releases.md#release-19)                                 | _Released 2020-03-31_                            |
| [Release 18](releases.md#release-18)                                 | _Released 2020-03-04_                            |
| [Release 17](releases.md#release-17)                                 | _Released 2020-01-24_                            |
| [Release 16](releases.md#release-16)                                 | _Released 2020-01-02_                            |
| \_\_[Release 15](releases.md#release-15)                             | _Released 2019-11-25_                            |
| [Release 14](releases.md#release-14)                                 | _Released 2019-11-06_                            |
| [Release 13](releases.md#release-13)                                 | _Released 2019-10-17_                            |
| [Release 12](releases.md#release-12)                                 | _Released 2019-09-11_                            |
| [Release 11](releases.md#release-11)                                 | _Released 2019-08-19_                            |
| [Release 10](releases.md#release-10)                                 | Released 2019-07-05                              |
| [Release 9](releases.md#release-9)                                   | Released 2019-05-16                              |
| [Release 8](releases.md#release-8)                                   | Released 2019-04-08                              |
| [Release 7](releases.md#release-7)                                   | Released 2019-03-15                              |

## _Release 25_

Release date: TBD

### Main Features

This release contains GUI performance improvements and a couple of extensions on the features introduced in [Release 24](releases.md#release-24).

See the [tracking issue on github](https://github.com/Sofie-Automation/sofie-core/pull/324) for details.

### Components

| Component                                                                                             | Version |
| :---------------------------------------------------------------------------------------------------- | :------ |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 1.13.0  |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 2.3.1   |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver)                     | 5.1.0   |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 1.11.0  |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 1.5.1   |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 1.2.1   |

## _Release 24_

Release date: 2020-09-28

### Main Features

- **Major performance improvements** Response times of 200-300 ms before have been reduced to about 100 ms, and some situations \(such as when adlibbing 100+ elements\) that was hurting before now have been greatly improved.
- **Adlib Actions** Adlibs now call a generic function in the blueprints, which can do various things \(think macros\).
- **Infinites Pieces** Introducing the new infinite types
  - OutOnRundownEnd, OutOnSegmentEnd Which follows the planned shows
  - OutOnSegmentChange, OutOnRundownChange Which follows the playhead
- **Routing** Output-layers can now be routed through RouteSets \(in the Settings/studio\), allowing an output to be mirrored to multiple output devices, switch between Main and Backup, or switch between which set of hardware to control.

### Notable features

- **Elastic APM tracing** Used by the developers to in detail trace performance reports in development and in prod.
- **Single-object timeline** Instead of an array of timeline-objects, a single object is now sent over the wire to the Playout Gateway, which increases responsiveness.
- **Accounts & security** \(opt-in through settings file\) Enable user accounts, log in and access control. Note that this is an experimental feature that might contain bugs.

_Note that when upgrading to this version, there are breaking changes from release 23._

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/20) for details.

### Components

| Component                                                                                             | Version                                      |
| :---------------------------------------------------------------------------------------------------- | :------------------------------------------- |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 1.12.0 _\(**Bugfix**: 1.12.1 - 2020/10/12\)_ |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 2.2.1                                        |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver)                     | 5.0.0                                        |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 1.10.1                                       |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 1.5.0                                        |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 1.2.1                                        |

## _Release 23 \(skipped\)_

Release date: _unreleased_

### Main Features

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/19) for details

## _Release 22_

Release date: 2020-08-17

Note: This is a big, BREAKING update, manual steps are required when upgrading.

### Main Features

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/18) for details

### Components

| Component                                                                                             | Version |
| :---------------------------------------------------------------------------------------------------- | :------ |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 1.10.0  |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | TBD     |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver)                     | 4.0.0   |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 1.9.0   |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 1.4.x   |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | -       |

## _Release 21 \(skipped\)_

Release date: _Unreleased_

### Main Features

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/17) for details

## _Release 20_

Release dates: 2020-05-12 \(1.8.0\), 2020-05-13 \(1.8.1\), 2020-05-27 \(1.8.2\)

### Main Features

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/16) for details

### Components

| Component                                                                                             | Version | Changelog                                                                                                                                   |
| :---------------------------------------------------------------------------------------------------- | :------ | :------------------------------------------------------------------------------------------------------------------------------------------ |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 1.8.2   | [Changelog](https://github.com/Sofie-Automation/sofie-core/blob/4c428983f4fba1fd366e52f71d523d707badb969/meteor/CHANGELOG.md)                          |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 1.11.0  | [Changelog](https://github.com/nrkno/tv-automation-sofie-blueprints-integration/blob/40c38a3805de5bc8794cf020c78fddc2eb674f9e/CHANGELOG.md) |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver)                     | 3.20.0  | [Changelog](https://github.com/nrkno/tv-automation-state-timeline-resolver/blob/cadcde8a54008e8b9597a2622c18487b53833b80/CHANGELOG.md)      |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 1.7.0   | [Changelog](https://github.com/nrkno/tv-automation-playout-gateway/blob/8807ca4250fb68629eb6c161522ccf984ac6fcf4/CHANGELOG.md)              |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 1.2.0   | Unchanged                                                                                                                                   |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 1.1.0   | Unchanged                                                                                                                                   |

## _Release 19_

Release date: 2020-03-31

### Main Features

- Gap parts: parts that fill space within a show that is to be filled by other parts during playback. \([nrkno/sofie-core\#198](https://github.com/Sofie-Automation/sofie-core/pull/198)\)
- Rundown playlists: break rundowns apart into rundowns and rundown playlists allowing effective continuous rundowns \([nrkno/sofie-core\#98](https://github.com/Sofie-Automation/sofie-core/pull/98)\) \(Contribution from TV 2\)
- First phase of Part Instances: a first step towards a more solid understanding of parts that are on-air and what is to be aired. \([nrkno/sofie-core\#150](https://github.com/Sofie-Automation/sofie-core/pull/150)\)

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/15) for details

### Components

| Component                                                                                             | Version | Changelog                                                                                                                 |
| :---------------------------------------------------------------------------------------------------- | :------ | :------------------------------------------------------------------------------------------------------------------------ |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 1.7.0   | [Changelog](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#170-0-2020-03-25)                         |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 1.10.0  | [Changelog](https://github.com/nrkno/tv-automation-sofie-blueprints-integration/blob/main/CHANGELOG.md#1100-2020-03-24) |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver-types)               | 3.19.0  | [Changelog](https://github.com/nrkno/tv-automation-state-timeline-resolver/blob/main/CHANGELOG.md#3190-2020-03-25)      |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 1.6.2   | [Changelog](https://github.com/nrkno/tv-automation-playout-gateway/blob/develop/CHANGELOG.md#160-2020-03-04)              |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 1.2.0   | [Changelog](https://github.com/nrkno/tv-automation-mos-gateway/blob/release19/CHANGELOG.md#120-0-2020-03-24)              |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 1.1.0   | N/A                                                                                                                       |

## _Release 18_

Release date: 2020-03-04

### Main Features

- [Improve UI performance](https://github.com/Sofie-Automation/sofie-core/pull/157)
- [Adlibs can state to always be queued](https://github.com/Sofie-Automation/sofie-core/pull/184) \(Contribution from TV 2\)
- [Segments can be hidden from the rundown and prompter views](https://github.com/Sofie-Automation/sofie-core/pull/174) \(Contribution from TV 2\)
- [Animated unfocused window border](https://github.com/Sofie-Automation/sofie-core/pull/192)
- Support action buttons \(eg Take\) in Dashboard layouts
- [ATEM media pool config UI](https://github.com/nrkno/tv-automation-playout-gateway/pull/57)

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/14) for details

### Components

| Component                                                                                             | Version | Changelog                                                                                                                |
| :---------------------------------------------------------------------------------------------------- | :------ | :----------------------------------------------------------------------------------------------------------------------- |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 1.6.0   | [Changelog](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#160-2020-03-04)                          |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 1.8.0   | [Changelog](https://github.com/nrkno/tv-automation-sofie-blueprints-integration/blob/main/CHANGELOG.md#180-2020-02-19) |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver-types)               | 3.18.0  | [Changelog](https://github.com/nrkno/tv-automation-state-timeline-resolver/blob/main/CHANGELOG.md#3180-2020-02-19)     |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 1.6.0   | [Changelog](https://github.com/nrkno/tv-automation-playout-gateway/blob/main/CHANGELOG.md#160-0-2020-02-19)            |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 1.1.0   | N/A                                                                                                                      |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 1.1.0   | N/A                                                                                                                      |

## _Release 17_

Release date: 2020-01-24

### Main Features

Notable features:

- Allow devices to provide a configuration manifest, thus decoupling the core from understanding the specifics of each of the devices. This will ease adding new features to the device modules.
- Allow blueprints to specify that a media object status for a given Piece should be ignored. Useful for static assets that may intentionally contain content otherwise considered problematic \(black frames, freeze frames, etc.\)
- Improve prompter performance
- Various bugfixes

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/13) for details

### Components

| Component                                                                                             | Version | Changelog                                                                                                                          |
| :---------------------------------------------------------------------------------------------------- | :------ | :--------------------------------------------------------------------------------------------------------------------------------- |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 1.5.0   | \_\_[_Changelog_](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#150-2020-01-24)\_\_                          |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 1.7.0   | \_\_[_Changelog_](https://github.com/nrkno/tv-automation-sofie-blueprints-integration/blob/main/CHANGELOG.md#170-2020-01-07)\_\_ |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver-types)               | 3.17.0  | \_\_[_Changelog_](https://github.com/nrkno/tv-automation-state-timeline-resolver/blob/main/CHANGELOG.md#3170-2020-01-08)\_\_     |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 1.5.0   | \_\_[_Changelog_](https://github.com/nrkno/tv-automation-playout-gateway/blob/main/CHANGELOG.md#150-2020-01-24)\_\_              |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 1.1.0   | \_\_[_Changelog_](https://github.com/nrkno/tv-automation-mos-gateway/blob/main/CHANGELOG.md#1190-2020-01-24)\_\_                 |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 1.1.0   | \_\_[_Changelog_](https://github.com/nrkno/tv-automation-media-management/blob/main/CHANGELOG.md#110-2020-01-24)\_\_             |

## _Release 16_

Release date: 2020-01-02

### Main Features

This release contains mainly bug fixes and code maintenance.

Notable features:

- **autorewind:** auto rewind leaving segment \([b88ea43](https://github.com/Sofie-Automation/sofie-core/commit/b88ea43)\)
- Invalid Reason information on invalid parts \([\#129](https://github.com/Sofie-Automation/sofie-core/issues/129)\) \([b4f5126](https://github.com/Sofie-Automation/sofie-core/commit/b4f5126)\)
- restart core from status view \([\#131](https://github.com/Sofie-Automation/sofie-core/issues/131)\) \([154f999](https://github.com/Sofie-Automation/sofie-core/commit/154f999)\)

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/11) for details

### Components

| Component                                                                                             | Version             | Changelog                                                                                                 |
| :---------------------------------------------------------------------------------------------------- | :------------------ | :-------------------------------------------------------------------------------------------------------- |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 1.4.1               | \_\_[_Changelog_](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#120-2019-11-06)\_\_ |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 1.5.0               |                                                                                                           |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver-types)               | 3.15.1              |                                                                                                           |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 1.4.0               |                                                                                                           |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 1.0.1 \(unchanged\) |                                                                                                           |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 1.0.2 \(unchanged\) |                                                                                                           |

## _Release 15_

Release date: 2019-11-25

### Main Features

This release contains mainly bug fixes and code maintenance.

Notable features:

- Basic Prompter, running in web window, controlled by Contour-Xpress, keyboard or mouse.
- Various bug fixes

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/10) for details

### Components

| Component                                                                                             | Version             | Changelog                                                                                                 |
| :---------------------------------------------------------------------------------------------------- | :------------------ | :-------------------------------------------------------------------------------------------------------- |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 1.3.0               | \_\_[_Changelog_](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#120-2019-11-06)\_\_ |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 1.2.1               |                                                                                                           |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver-types)               | 3.14.0              |                                                                                                           |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 1.3.0               |                                                                                                           |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 1.0.1 \(unchanged\) |                                                                                                           |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 1.0.2               |                                                                                                           |

## _Release 14_

Release date: 2019-11-06

### Main Features

This release contains mainly bug fixes and code maintenance.

Notable features:

- Add more unit-tests in Core \(code maintenance\)
- Playout Gateway now monitoring the Hyperdeck recording status. \(Raising the alarm if recording isn't working\)
- Streamdeck view \([more info in PR](https://github.com/Sofie-Automation/sofie-core/pull/106)\)
- Blueprint config parameter can now be a "table"

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/8) for details

### Components

| Component                                                                                             | Version             | Changelog                                                                                                 |
| :---------------------------------------------------------------------------------------------------- | :------------------ | :-------------------------------------------------------------------------------------------------------- |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 1.2.0               | \_\_[_Changelog_](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#120-2019-11-06)\_\_ |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 1.1.0               |                                                                                                           |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver-types)               | 3.13.1              |                                                                                                           |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 1.2.1 _\(patched\)_ |                                                                                                           |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 1.0.1               |                                                                                                           |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 1.0.1               |                                                                                                           |

## _Release 13_

Release date: 2019-10-17 _\(patched 2019-11-01\)_

### Main Features

This release features several bug fixes and a few features:

- Support for remote system messages management _Allowing an external manager to send out a system message to a whole fleet of Sofie-cores._
- Preview of HTML-graphics in the hover-scrub in GUI
- GUI: Errors and possible issues are highlighted in the settings pages
- GUI: Initial getting-started-tour in GUI \(activated by [/?help=1](http://localhost:3000/?help=1)\)
- GUI: Improved visualization of device hierarchy in status page
- GUI: Improved navigation and links between studio/showstyles and blueprints in settings
- User is now able to undo a Hold \(by pressing Shift+H\)
- User can now restart the Quantel-Gateway device

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/6) for details

### Components

| Component                                                                                             | Version            | Changelog                                                                                  |
| :---------------------------------------------------------------------------------------------------- | :----------------- | :----------------------------------------------------------------------------------------- |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 1.1.2 \(patched!\) | \_\_[_Changelog_](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md)\_\_ |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 1.1.0              |                                                                                            |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver-types)               | 3.12.0             |                                                                                            |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 1.1.0              |                                                                                            |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 1.0.0              |                                                                                            |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 1.0.1              |                                                                                            |

## _Release 12_

Release date: 2019-09-11

### Main Features

This release features many bug fixes and support for a few new playout devoces:

- Playout-gateway: Support for the Quantel video server, via the [Quantel Gateway](https://github.com/nrkno/tv-automation-quantel-gateway)
- Playout-gateway: Support for the [Sisyfos audio controller](https://github.com/olzzon/sisyfos-audio-controller)
- Playout-gateway: Generic TCP-controlled device
- Playout-gateway: Hyperdeck monitoring disk usage, and be able to format slots
- Core: Support for shotbox-like buttons in the shelf
- ..and fixes for many, many bugs introduced in R10 and R11.

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/5) for details

### Components

| Component                                                                                             | Version | Changelog                                                                                                 |
| :---------------------------------------------------------------------------------------------------- | :------ | :-------------------------------------------------------------------------------------------------------- |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 1.0.0   | \_\_[_Changelog_](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#100-2019-09-11)\_\_ |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 0.24.0  |                                                                                                           |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver-types)               | 3.8.3   |                                                                                                           |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 1.0.0   |                                                                                                           |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 1.0.0   |                                                                                                           |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 1.0.0   |                                                                                                           |

##

## _Release 11_

Release date: _2019-08-19_

### Main Features

This release is a maintenance release, with only minor features.

- Core: Blueprint.onGenerateTimeline improvements
- Core: REST API, a first version, allowing basic control of playout
- Playout-gateway: CommandError callback: report to Core when a command fails

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/4) for details

### Components

| Component                                                                                             | Version | Changelog                                                                                                  |
| :---------------------------------------------------------------------------------------------------- | :------ | :--------------------------------------------------------------------------------------------------------- |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 0.26.0  | \_\_[_Changelog_](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#0260-2019-08-19)\_\_ |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 0.24.1  |                                                                                                            |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver-types)               | 3.1.1   |                                                                                                            |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 0.21.0  |                                                                                                            |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 0.8.0   |                                                                                                            |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 0.2.1   |                                                                                                            |

## Release 10

Release date: _2019-07-05_

### Main Features

This release features a BIG refactoring and a lot of renamings. _Therefore, this release is NOT backwards compatible._

- **The Big Renaming** _A big refactoring and renaming of variables and data structures._

  _Some of the most prominent renamings are:_

  - _StudioInstallation -&gt; Studio_
  - _RunningOrder -&gt; Rundown_
  - _Segment \(unchanged\)_
  - _SegmentLine -&gt; Part_
  - _SegmentLineItem -&gt; Piece_

- **New ingest data pipeline** _\*\*This is a step on the way to support different types of sources of input data._
- **New Timeline** _This release also features the new_ [_Timeline_ ](https://www.npmjs.com/package/superfly-timeline)_\(version 7.0\), which gives better control and performance_
- **Unit tests & CI** _In order to achieve a safer development environment, higher code quality and catching bugs earlier, we've added Jest as test framework._

See the [tracking issue on github](https://github.com/Sofie-Automation/Sofie-TV-automation/issues/3) for details

### Components

| Component                                                                                             | Version | Changelog                                                                                          |
| :---------------------------------------------------------------------------------------------------- | :------ | :------------------------------------------------------------------------------------------------- |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 0.25.0  | [_Changelog_](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#0250-2019-07-05) |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 0.23.0  |                                                                                                    |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver-types)               | 3.0.1   |                                                                                                    |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 0.20.0  |                                                                                                    |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 0.8.0   |                                                                                                    |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 0.2.0   |                                                                                                    |

## Release 9

Release date: 2019-05-16

### Main Features

- **Take from anywhere** _Start playing from anywhere in a segmentLine, not just from the beginning of it_
- **Set In / Out points** _UI for editing in & out-points of video clips_
- **Prompter** _Teleprompter on a separate page \(se documentation in README\)_
- **Invalid SegmentLines** _If a segmentLine cannot be created proberly by the blueprint, it can no be set as "invalid", which prevents it from being played out_
- **System & studio blueprints** _The blueprints have now been split into system-, studio- & showStyle- blueprints_

### Components

| Component                                                                                             | Version                                                                                     | Changelog                                                                                          |
| :---------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 0.24.0                                                                                      | [_Changelog_](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#0240-2019-05-16) |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 0.19.0                                                                                      |                                                                                                    |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver-types)               | 2.2.0                                                                                       |                                                                                                    |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 0.19.1                                                                                      |                                                                                                    |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 0.7.0                                                                                       |                                                                                                    |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 0.1.8 \(no changes\)                                                                        |                                                                                                    |
| [CasparCG](https://github.com/nrkno/tv-automation-casparcg-server)                                    | [2.1.7_NRK](https://github.com/nrkno/tv-automation-casparcg-server/releases/tag/v2.1.7_NRK) |                                                                                                    |
| [CasparCG Media-Scanner](https://github.com/nrkno/tv-automation-media-scanner)                        | [1.5.3_NRK](https://github.com/nrkno/tv-automation-media-scanner/releases/tag/v1.5.3rc4)    |                                                                                                    |

## Release 8

Release date: 2019-04-08

### Main Features

- **Set In / Out points** _\(preliminary implementation\)_
- **Timeline vizualiser**

### Components

| Component                                                                                             | Version                                                                               | Changelog                                                                                          |
| :---------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 0.23.0                                                                                | [_Changelog_](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#0230-2019-04-08) |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 0.16.0                                                                                |                                                                                                    |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver-types)               | 2.0.1                                                                                 |                                                                                                    |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 0.18.0                                                                                |                                                                                                    |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 0.5.3                                                                                 |                                                                                                    |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | 0.1.8                                                                                 |                                                                                                    |
| [CasparCG Launcher](https://github.com/nrkno/tv-automation-casparcg-launcher)                         | [0.6.1](https://github.com/nrkno/tv-automation-casparcg-launcher/releases/tag/v0.6.1) |                                                                                                    |

## Release 7

Release date: 2019-03-15

### Components

| Component                                                                                             | Version                                                                                     | Changelog                                                                                          |
| :---------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| [Core](https://github.com/Sofie-Automation/sofie-core)                                                           | 0.22.0                                                                                      | [_Changelog_](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#0220-2019-03-15) |
| [Blueprints API \( Core \)](https://www.npmjs.com/package/tv-automation-sofie-blueprints-integration) | 0.13.0                                                                                      |                                                                                                    |
| [Blueprints API \( TSR \)](https://www.npmjs.com/package/timeline-state-resolver-types)               | 1.6.3                                                                                       |                                                                                                    |
| [Playout Gateway](https://github.com/nrkno/tv-automation-playout-gateway)                             | 0.17.0                                                                                      |                                                                                                    |
| [Mos Gateway](https://github.com/nrkno/tv-automation-mos-gateway)                                     | 0.5.2                                                                                       |                                                                                                    |
| [Media Manager](https://github.com/nrkno/tv-automation-media-management)                              | [r7rc1](https://github.com/nrkno/tv-automation-media-management/releases/tag/r7rc1)         |                                                                                                    |
| [CasparCG Launcher](https://github.com/nrkno/tv-automation-casparcg-launcher)                         | [0.6.0](https://github.com/nrkno/tv-automation-casparcg-launcher/releases/tag/v0.6.0)       |                                                                                                    |
| [CasparCG](https://github.com/nrkno/tv-automation-casparcg-server)                                    | [2.1.6_NRK](https://github.com/nrkno/tv-automation-casparcg-server/releases/tag/v2.1.6_NRK) |                                                                                                    |

## Release 6

_---This release was discarded due to stability issues and replaced by Release 7---_

See [Core changelog](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#0210-0-2019-02-05) for details

Core version: 0.21.0

## Release 5

Release date: 2019-02-05

See [Core changelog](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#0200-2019-02-05) for details

Core version: 0.20.0

## Release 4

Release date: 2018-12-17

See [Core changelog](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#0181-2018-12-11) for details

Core version: ~~0.18.1~~ patched by 0.19.0

## Release 3

Release date: 2018-11-15

See [Core changelog](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#0160-2018-10-26) for details

Core version: 0.17.0

## Release 2

Release date: 2018-10-26

See [Core changelog](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#0150-2018-10-16) for details

Core version: 0.16.0

## Release 1

Release date: 2018-09-07

See [Core changelog](https://github.com/Sofie-Automation/sofie-core/blob/main/meteor/CHANGELOG.md#0110-2018-09-07) for details

Core version: 0.11.0
