# Peblar EV charger component for Home Assistant

Custom component to support Easee EV chargers and equalizers.

The status sensor is the default sensor and has the following values

```
disconnected
awaiting_start
charging
ready_to_charge
completed
error
```
## Installation

### Git installation

1. Make sure you have git installed on your machine.
2. Navigate to you home assistant configuration folder.
3. Create a `custom_components` folder of it does not exist, navigate down into it after creation.
4. Execute the following command: `git clone https://github.com/0xf-group/hass-peblar peblar`
5. Run `bash links.sh`

## Configuration

Configuration is done through in Configuration > Integrations where you first configure it and then set the options for what you want to monitor.

## Debug logging
A full debug log can be enabled by entering following into `configuration.yaml` and restarting Home Assistant
```yaml
logger:
  default: info
  logs:
    custom_components.peblar: debug
```
