# Third-Party Notices

This inventory reflects the versions declared in `platformio.ini` and the
licenses identified in the corresponding locally installed package metadata
or license files. It is a dependency inventory, not a legal assessment of
commercial distribution. Keep the upstream license texts and notices with
redistributed source or binaries as required by each license.

## Firmware and UI dependencies

| Component | Version | Use | License identified | Upstream source |
|---|---:|---|---|---|
| Arduino-ESP32 framework | 2.0.17 (`framework-arduinoespressif32` package `4.20017.260907+sha.dcc1105b`) | ESP32 Arduino core and bundled libraries | LGPL-2.1-or-later (package metadata) | [espressif/arduino-esp32](https://github.com/espressif/arduino-esp32) |
| TFT_eSPI | 2.5.43 | TFT display and resistive touch support | Mixed notices in upstream `license.txt`: FreeBSD, BSD, and MIT-origin components | [Bodmer/TFT_eSPI](https://github.com/Bodmer/TFT_eSPI) |
| LVGL | 8.4.0 | Display UI | MIT | [lvgl/lvgl](https://github.com/lvgl/lvgl) |
| ESPAsyncWebServer | 3.12.1 | HTTP and WebSocket server | LGPL-3.0 | [ESP32Async/ESPAsyncWebServer](https://github.com/ESP32Async/ESPAsyncWebServer) |
| AsyncTCP | 3.5.0 | Asynchronous TCP transport | LGPL-3.0 | [ESP32Async/AsyncTCP](https://github.com/ESP32Async/AsyncTCP) |
| ArduinoJson | 7.4.3 | JSON serialization and parsing | MIT | [bblanchon/ArduinoJson](https://github.com/bblanchon/ArduinoJson) |
| NimBLE-Arduino | 2.5.1 | BLE GATT and OTA transport | Apache-2.0; bundled NimBLE and TinyCrypt components have their own upstream notices (Apache-2.0 and BSD-style, respectively) | [h2zero/NimBLE-Arduino](https://github.com/h2zero/NimBLE-Arduino) |
| autowp-mcp2515 | 1.3.1 | MCP2515 CAN controller | MIT | [autowp/arduino-mcp2515](https://github.com/autowp/arduino-mcp2515) |

The exact license files are distributed with the corresponding upstream
packages. The local PlatformIO metadata identifies the versions above; a
firmware release should retain the full applicable license texts and notices,
including the bundled-component notices.

## Test dependency

| Component | Version | Use | License identified | Upstream source |
|---|---:|---|---|---|
| Unity | PlatformIO-managed; not version-pinned in `platformio.ini` | Native unit tests | MIT | [ThrowTheSwitch/Unity](https://github.com/ThrowTheSwitch/Unity) |

## DBC data files

The repository audit lists 57 DBC files. Their source and license metadata
remain `unverified`; this notice does not assign authorship, provenance, or
permission to use them. Do not infer a license from a filename or vehicle
name. Resolve provenance and commercial-use decisions with the project owner
before redistribution; unknown files are retained rather than silently
removed.

## Scope

This file covers the declared firmware libraries, the Arduino-ESP32 framework,
and the native-test framework. It does not claim to enumerate every
transitive SDK, compiler, build-tool, or operating-system component. Their
package-provided notices must be reviewed separately before distributing
build environments or firmware binaries.
