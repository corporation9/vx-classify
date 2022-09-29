vx-classify
==========

vx-classify is a simple tool that converts the hex Bluetooth Class of Device (CoD) code into human-readable output. CoDs are used to uniquely identify the capabilities of Bluetooth devices, and allow for an easier way to identify them when pairing or managing them. Unfortunately, these codes are not very descriptive and are not easily understood by humans. vx-classify converts these codes into a more readable format and provides some useful information about the device.

The CoD is a six-byte identifier that identifies the class of device, or type of peripheral, that a Bluetooth device reports itself to be. A CoD can match up with any number of peripheral types, but matching up these CoDs to their specific device types requires additional information from the user—this is where vx-classify comes in.


Run it like this:

    $ ./vx-classify 38010c 0x5a020c 240404
    0x38010c: Computer (Laptop): Audio, Object Transfer, Capturing
    0x5a020c: Phone (Smartphone): Telephony, Object Transfer, Capturing, Networking
    0x240404: Audio/Video (Wearable Headset Device): Audio, Rendering

Data Source
-----------

Class of Device data is maintained by the Bluetooth SIG on the
[Baseband Assigned Numbers](https://www.bluetooth.org/en-us/specification/assigned-numbers/baseband)
page.

