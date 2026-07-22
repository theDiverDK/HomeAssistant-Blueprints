# Home Assistant Blueprints

A personal collection of Home Assistant automation blueprints for common smart-home devices and routines. Each blueprint is a YAML file that can be imported into a Home Assistant installation and configured through the UI.

## Blueprints

| Blueprint | Purpose |
| --- | --- |
| [`danfoss_ally/window_open_pause_heating.yaml`](danfoss_ally/window_open_pause_heating.yaml) | Pauses Danfoss Ally heating through Zigbee2MQTT while selected window or door sensors are open, then resumes it after they close. |
| [`ikea_e1743_light_control/control.yaml`](ikea_e1743_light_control/control.yaml) | Controls lights with an IKEA E1743 remote. |
| [`inform_when_not_in_use/inform_when_not_in_use.yaml`](inform_when_not_in_use/inform_when_not_in_use.yaml) | Sends a notification when configured devices are not in use. |
| [`sonoff_motion_sensor/control.yaml`](sonoff_motion_sensor/control.yaml) | Uses a Sonoff motion sensor in an automation. |

## Import a blueprint

1. In Home Assistant, go to **Settings → Automations & scenes → Blueprints**.
2. Select **Import Blueprint**.
3. Paste the URL of the desired YAML file from this repository.
4. Create an automation from the imported blueprint and choose the entities for your installation.

## Requirements

Requirements vary by blueprint. Read the input descriptions in the YAML before importing. The Danfoss Ally and IKEA E1743 blueprints are designed for entities exposed through Zigbee2MQTT.

## Notes

Test automations with a single device first. Entity names, MQTT integrations, and device capabilities differ between Home Assistant installations.
