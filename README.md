# Media Player Lights Sync

_AppDaemon App that synchronizes the color of RGB lights with the thumbnail of a media player in Home Assistant._[span_0](start_span)[span_0](end_span)

[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs) [![](https://img.shields.io/github/release/jonathangibson98/media-lights-sync/all.svg?style=for-the-badge)](https://github.com/jonathangibson98/media-lights-sync/releases) ![downloads-latest](https://img.shields.io/github/downloads/jonathangibson98/media-lights-sync/total?style=for-the-badge)[span_1](start_span)[span_1](end_span)

[![Tests](https://github.com/jonathangibson98/media-lights-sync/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/jonathangibson98/media-lights-sync/actions/workflows/tests.yaml)[span_2](start_span)[span_2](end_span)

<a href="https://www.buymeacoffee.com/ericmatte" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>[span_3](start_span)[span_3](end_span)

<img src="https://github.com/jonathangibson98/media-lights-sync/raw/master/examples/example-1.jpg" alt="Example 1" width="400"> <img src="https://github.com/jonathangibson98/media-lights-sync/raw/master/examples/example-2.jpg" alt="Example 1" width="400">[span_4](start_span)[span_4](end_span)

## Features

- Realtime RGB lights color synchronization with the thumbnail of a media player[span_5](start_span)[span_5](end_span)
- Extract most relevant colors from a picture and assign them to lights[span_6](start_span)[span_6](end_span)
- Always creates great matching moody ambiances[span_7](start_span)[span_7](end_span)
- Change all configured lights color at the same time using multithreading[span_8](start_span)[span_8](end_span)
- Prevent lights synchronization based on a state condition from your Home Assistant[span_9](start_span)[span_9](end_span)

## Installation

Use [HACS](https://hacs.xyz/) or download the `media_lights_sync` directory from inside the `apps` directory here to your local `apps` directory, then add the configuration to enable the `media_lights_sync` module[span_10](start_span)[span_10](end_span).

## Prerequisites

In order for this app to work, you need to add `py3-pillow` and `Pillow` to the config of your AppDaemon 4 Supervisor add-on[span_11](start_span)[span_11](end_span):

```yaml
system_packages:
  - py3-pillow
python_packages:
  - Pillow
init_commands: []
log_level: info
