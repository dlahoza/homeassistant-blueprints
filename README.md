# Home Assistant Blueprints

Home Assistant blueprints to automate common tasks in my smart home.

This repository collects compact, reusable automation blueprints you can import into Home Assistant. Each blueprint is designed to be self-contained and configurable via the Home Assistant Blueprint UI.

---

## Blueprints

Below are the blueprints included in this repository. Click the "Add to Home Assistant" button to import a blueprint directly into your Home Assistant instance.

### Automatic Heating
Turn on heating when any thermostat is heating or any binary sensor is on. The idea is to control a central heating system based on the state of multiple thermostats and sensors around the house. For example, turn on the heating for the floor if any room thermostat is calling for heat.

- File: `automatic-heating.yaml`
- Description: Turn on heating when any thermostat is heating or any binary sensor is on.

[![Add Automatic Heating](https://img.shields.io/badge/Add%20to%20Home%20Assistant-blue?logo=home-assistant&style=for-the-badge)](https://raw.githubusercontent.com/dlahoza/homeassistant-blueprints/main/automatic-heating.yaml)

---

### Controller → Follower Climate Control
It's made to turn off TRVs when AC is on in the room.

- File: `control-climates.yaml`
- Description: If any controller climate is ON (hvac_mode != 'off'), all follower climates are turned OFF. If all controller climates are OFF, follower climates are turned ON (optionally sets follower HVAC mode).

[![Add Controller → Follower Climate Control](https://img.shields.io/badge/Add%20to%20Home%20Assistant-blue?logo=home-assistant&style=for-the-badge)](https://raw.githubusercontent.com/dlahoza/homeassistant-blueprints/main/control-climates.yaml)

---

### Link On/Off State of Multiple Devices
Sync the on/off state between a group of entities so that when one changes, the others follow. So you can link follower switches to a main switch with syncing their states. Buttons, lights, or any other switchable entities can be linked together.

- File: `link_multiple_devices.yaml`
- Description: Sync switch devices state across multiple entities.

[![Add Link Devices](https://img.shields.io/badge/Add%20to%20Home%20Assistant-blue?logo=home-assistant&style=for-the-badge)](https://raw.githubusercontent.com/dlahoza/homeassistant-blueprints/main/link_multiple_devices.yaml)

---

## Usage

1. Click any "Add to Home Assistant" button above (it opens the raw YAML URL). In Home Assistant, go to Settings → Automations & Scenes → Blueprints → Import blueprint, and paste the URL.
2. Configure inputs and save the automation created from the blueprint.

## Contributing
Contributions welcome — please open an issue or pull request with improvements, new blueprints, or bug fixes.

## License
This repository is available under the MIT License. See the `LICENSE` file for details.
