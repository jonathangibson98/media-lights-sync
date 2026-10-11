# Media Player Lights Sync

_AppDaemon app that synchronizes the color of RGB lights with the thumbnail of a media player in Home Assistant._

[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs)
[![Release](https://img.shields.io/github/release/jonathangibson98/media-lights-sync/all.svg?style=for-the-badge)](https://github.com/jonathangibson98/media-lights-sync/releases)
[![Tests](https://github.com/jonathangibson98/media-lights-sync/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/jonathangibson98/media-lights-sync/actions/workflows/tests.yaml)

<img src="https://raw.githubusercontent.com/jonathangibson98/media-lights-sync/main/examples/example-1.jpg" alt="Example 1" width="400"> <img src="https://raw.githubusercontent.com/jonathangibson98/media-lights-sync/main/examples/example-2.jpg" alt="Example 2" width="400">

## Features

- Realtime RGB light color synchronization with the thumbnail of a media player
- Extracts the most relevant colors from a picture and assigns them to lights
- Always creates great matching moody ambiances
- Changes all configured lights at the same time using multithreading
- Prevents synchronization based on a state condition from your Home Assistant

## Installation

Use [HACS](https://hacs.xyz/), or download the `media_lights_sync` directory from inside the `apps` directory to your local `apps` directory. Then add the configuration to enable the `media_lights_sync` module.

## Prerequisites

For this app to work, add `py3-pillow` and `Pillow` to the config of your AppDaemon 4 Supervisor add-on:

```yaml
system_packages:
  - py3-pillow
python_packages:
  - Pillow
init_commands: []
log_level: info
```
