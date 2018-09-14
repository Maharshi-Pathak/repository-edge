# Community Hass.io Add-ons: Network UPS Tools

[![Release][release-shield]][release] ![Project Stage][project-stage-shield] ![Project Maintenance][maintenance-shield]

[![Discord][discord-shield]][discord] [![Community Forum][forum-shield]][forum]

[![Buy me a coffee][buymeacoffee-shield]][buymeacoffee]

A Network UPS Tools daemon to allow you to easily manage battery backup (UPS)
devices connected to your Hass.io machine.

## About

The primary goal of the Network UPS Tools (NUT) project is to provide support
for Power Devices, such as Uninterruptible Power Supplies, Power Distribution
Units, Automatic Transfer Switch, Power Supply Units and Solar Controllers.

NUT provides many control and monitoring [features][nut-features], with a
uniform control and management interface.

More than 140 different manufacturers, and several thousands models
are [compatible][nut-compatible].

The Network UPS Tools (NUT) project is the combined effort of
many [individuals and companies][nut-acknowledgements].

Be sure to add a NUT Sensor to your `configuration.yaml` after starting the
add-on:

```yaml
sensor:
  - platform: nut
    name: "CyberPower 1500"
    host: a0d7b954-nut
    username: nutty
    password: changeme
    resources:
      - battery.charge
      - battery.runtime
      - ups.load
      - ups.status
```

For more information on how to configure the NUT Sensor in Home Assistant
see the [NUT Sensor documentation][nut-sensor-docs].

[Click here for the full documentation][docs]

## WARNING! THIS IS AN EDGE VERSION!

This Hass.io Add-ons repository contains edge builds of add-ons. Edge builds
add-ons are based upon the latest development version.

- They may not work at all.
- They might stop working at any time.
- They could have a negative impact on your system.

This repository was created for:

- Anybody willing to test.
- Anybody interested in trying out upcoming add-ons or add-on features.
- Developers.

If you are more interested in stable releases of our add-ons:

<https://github.com/hassio-addons/repository>

[project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
[forum-shield]: https://img.shields.io/badge/community-forum-brightgreen.svg
[forum]: https://community.home-assistant.io/t/community-hass-io-add-on-network-ups-tools/68516
[discord-shield]: https://img.shields.io/discord/478094546522079232.svg
[discord]: https://discord.me/hassioaddons
[maintenance-shield]: https://img.shields.io/maintenance/yes/2018.svg
[release-shield]: https://img.shields.io/badge/version-65d0b03-blue.svg
[release]: https://github.com/hassio-addons/addon-nut/tree/65d0b03
[docs]: https://github.com/hassio-addons/addon-nut/blob/65d0b03/README.md
[buymeacoffee-shield]: https://www.buymeacoffee.com/assets/img/guidelines/download-assets-sm-2.svg
[buymeacoffee]: https://www.buymeacoffee.com/dale3h