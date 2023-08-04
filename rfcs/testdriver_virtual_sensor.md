# RFC _<PR_number>_: Add virtual sensor support to testdriver.js

## Summary

Add testdriver.js support for [Generic Sensor API](https://w3c.github.io/sensors/), by supporting [create_virtual_sensor](https://w3c.github.io/sensors/#create-mock-sensor-command), [update_virtual_sensor](https://w3c.github.io/sensors/#update-mock-sensor-reading-command), [remove_virtual_sensor](https://w3c.github.io/sensors/#delete-mock-sensor-command) and [get_virtual_sensor_information](https://w3c.github.io/sensors/#get-mock-sensor-command).

## Details

Proposed `create_virtual_sensor` command creates a new mock sensor.

Proposed `update_virtual_sensor` command updates a given type of mock sensor's reading.

Proposed `remove_virtual_sensor` command deletes a given type of mock sensor.

Proposed `get_virtual_sensor_information` command retrieves information about a given type of mock sensor.

These commands allows full end-to-end testing of Generic Sensors API.

## Risks

This increases the API surface of testdriver.js, so it's more code to maintain
or reason about.
