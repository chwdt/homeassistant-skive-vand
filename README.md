## A [homeassistant](https://www.home-assistant.io) [automation](https://www.home-assistant.io/docs/automation/) to read smart meter data from Skive Vand

This automation reads smart meter data from [Skive Vand](https://skivevand.bdforsyning.dk/)

The automation creates three sensors for `water_volume`, `water_temperature`, and `water_volume_backflow` and two binary_sensors for `leakage_alarm` and `burst_alarm`.

# Installation

Install `skive_vand.yaml` in [homeassistant/packages](https://www.home-assistant.io/docs/configuration/packages/) and add `skive_vand_username` and `skive_vand_password` in your `secrets.yaml`.

Add the following to your configuration.yaml, if you don't already have this:

```
homeassistant:
  packages: !include_dir_named packages
```
