# Changelog

## v0.1.9-dev
* Changed: Fixes sporadic error on startup with power factor https://github.com/mr-manuel/venus-os_dbus-mqtt-grid/issues/40

## v0.1.8
* Changed: Fix missing frequency in config file https://github.com/mr-manuel/venus-os_dbus-mqtt-grid/issues/38
* Changed: Fix restart issue
* Changed: Fix typo https://github.com/mr-manuel/venus-os_dbus-mqtt-grid/issues/40

## v0.1.7
⚠️ This version is required for Venus OS v3.60~27 or later, but it is also compatible with older versions.
* Added: Device type `heatpump`
* Added: Filter power values out of range
* Added: paho-mqtt module to driver
* Added: Power factor
* Added: Shelly Gen2+ device support
* Changed: Broker port missing on reconnect
* Changed: Default device instance is now `100`
* Changed: Fixed service not starting sometimes

## v0.1.6
* Added: Set device type to `grid`, `genset` or `acload`
* Changed: Add VRM ID to MQTT client name
* Changed: Fix registration to dbus https://github.com/victronenergy/velib_python/commit/494f9aef38f46d6cfcddd8b1242336a0a3a79563

## v0.1.5
* Added: Error handling
* Changed: Fixed problems when timeout was set to `0`
* Changed: Handling when voltage=0 is provided and no current

## v0.1.4
* Added: Tasmota support with https://github.com/mr-manuel/venus-os_dbus-mqtt-grid/pull/8 by @randomname32
* Added: Timeout on driver startup. Prevents problems, if the MQTT broker is not reachable on driver startup

## v0.1.3
* Changed: Fix crash when rounding none value
* Changed: Fixed a typo

## v0.1.2
* Added: Frequency
* Added: Show to which broker and port the connection was made when logging is set to INFO
* Added: Try to reconnect every 15 seconds to MQTT broker, if connection is closed abnormally
* Changed: Improved error handling and output

## v0.1.1
* Added: Timeout in order to disconnect the grid meter, if no new MQTT message is received after x seconds (configurable in `config.ini`)

## v0.1.0
* Added: Device name can be changed in the `config.ini`
* Added: Device instance can be changed in the `config.ini`
* Added: How to create multiple instances in `README.md`
* Changed: Topic variable name in `config.ini`

## v0.0.2
* Added: Set logging level in `config.default.ini`
* Changed: Logging levels of different messages for clearer output
* Changed: Optimized log output for faster troubleshooting

## v0.0.1
Initial release
