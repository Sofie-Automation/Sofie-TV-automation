---
description: Source Code for the Sofie System
---

# Applications & Libraries

## Main Application

The Sofie TV Automation system consists of the [**Sofie Server Core**](https://github.com/Sofie-Automation/sofie-core) which is the core application that serves the web GUI and handles the core logic.

## Gateways

Together with the _Server Core_ there are several _gateways_ which are separate applications, but which connect to _Server Core_ and are managed from within the Core's web UI.

- \*\*\*\*[**Input Gateway**](https://github.com/Sofie-Automation/sofie-input-gateway) **\(Work in progress\)**
- [**MOS Gateway**](https://github.com/nrkno/tv-automation-mos-gateway) \*\*\*\*Connects Sofie to a newsroom system and ingests rundowns via the [MOS protocol](http://mosprotocol.com/).
- [**Spreadsheet Gateway**](https://github.com/SuperFlyTV/spreadsheet-gateway) \*\*\*\*Connects Sofie to a Google-Drive folder and ingests rundowns from spreadsheets.
- [**Playout Gateway**](https://github.com/nrkno/tv-automation-playout-gateway) \*\*\*\*Handles the playout from Sofie. Connects to and controls a multitude of devices, such as vision mixers, graphics, light controllers, audio mixers etc..
- \*\*\*\*[**Quantel Gateway**](https://github.com/Sofie-Automation/sofie-quantel-gateway) \*\*\*\*CORBA to REST gateway for Quantel/ISA playback.

## Libraries

There are a number of libraries used in the Sofie ecosystem:

- [**ATEM Connection**](https://github.com/Sofie-Automation/sofie-atem-connection) \*\*\*\*Library for communicating with Blackmagic Design ATEM mixers
- [**ATEM State**](https://github.com/Sofie-Automation/sofie-atem-state) Used in TSR to tracks the state of ATEM:s and generate commands to control them.
- [**CasparCG Connection**](https://github.com/SuperFlyTV/casparcg-connection) \***\*developed by \*\***[_SuperFly.tv_](https://github.com/SuperFlyTV) \*\*\*\*Library to connect and interact with CasparCG Servers.
- [**CasparCG State**](https://github.com/superflytv/casparcg-state) \***\*developed by \*\***[_SuperFly.tv_](https://github.com/SuperFlyTV) \*\*\*\*Used in TSR to tracks the state of CasparCG Servers and generate commands to control them.
- [**Ember+ Connection**](https://github.com/Sofie-Automation/sofie-emberplus-connection) \*\*\*\*Library to communicate with _Ember+_ control protocol
- [**HyperDeck Connection**](https://github.com/Sofie-Automation/sofie-hyperdeck-connection) Library for connecting to Blackmagic Design Hyperdeck recorders.
- [**MOS Connection**](https://github.com/Sofie-Automation/sofie-mos-connection) \*\*\*\*A [_MOS protocol_](http://mosprotocol.com/) library for acting as a MOS device and connecting to an newsroom control system.
- \*\*\*\*[**Quantel Gateway Client**](https://github.com/Sofie-Automation/sofie-quantel-gateway-client) An interface that talks to the Quantel-Gateway application.
- [**SuperFly-Timeline**](https://github.com/SuperFlyTV/supertimeline) \***\*developed by \*\***[_SuperFly.tv_](https://github.com/SuperFlyTV) \*\*\*\*Resolver and rules for placing objects on a virtual timeline.
- [**ThreadedClass** ](https://github.com/nytamin/threadedClass)developed by \*\*\*\*[_Nytamin_](https://github.com/nytamin) Used in TSR to spawn device controllers in separate processes.
- [**Timeline State Resolver**](https://github.com/Sofie-Automation/sofie-timeline-state-resolver) \(TSR\) \***\*The main driver in **Playout Gateway,** handles connections to playout-devices and sends commands based on a **Timeline** received from **Core\*\*.

There are also a few typings-only libraries that define interfaces between applications:

- \*\*\*\*[**Blueprints integration**](https://www.npmjs.com/package/@sofie-automation/blueprints-integration) Defines the interface between [**Blueprints** ](dictionary.md#blueprints)and [**Sofie Core**](dictionary.md#sofie-core).
- [**Server Core Integration**](https://www.npmjs.com/package/@sofie-automation/server-core-integration) \*\*\*\*Used to connect to the [Sofie Server Core](https://github.com/Sofie-Automation/sofie-core) by the Gateways.
- [**Timeline State Resolver types**](https://www.npmjs.com/package/timeline-state-resolver-types) Defines the interface between [**Blueprints**](dictionary.md#blueprints) \***\*and the timeline that will be fed into **TSR\*\* for playout.

## Other Sofie-related Repositories

- [**CasparCG Server** \(NRK fork\)](https://github.com/nrkno/sofie-casparcg-server) Sofie-specific fork of CasparCG Server.
- [**CasparCG Launcher**](https://github.com/Sofie-Automation/sofie-casparcg-launcher) Launcher, controller, and logger for CasparCG Server.
- [**CasparCG Media Scanner** \(NRK fork\)](https://github.com/nrkno/sofie-casparcg-server) Sofie-specific fork of CasparCG Server 2.2 Media Scanner.
- [**Package Manager**](https://github.com/Sofie-Automation/sofie-package-manager) \*\*\*\*Handles media transfer and media file management for pulling new files and deleting expired files on playout devices.
- \*\*\*\*[**Quantel Browser plugin**](https://github.com/Sofie-Automation/sofie-quantel-browser-plugin) MOS-compatible Quantel video clip browser for use with Sofie.
- \*\*\*\*[**Sisyfos Audio Controller**](https://github.com/nrkno/sofie-sisyfos-audio-controller) \***\*developed by \*\***[_olzzon_](https://github.com/olzzon/)
