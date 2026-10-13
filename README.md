# tinyblock

A TinyGo port of [M-Abozaid/esp32-c3-adblock](https://github.com/M-Abozaid/esp32-c3-adblock).
It turns a roughly $2 ESP32-C3 into a network-wide DNS sinkhole: blocked domains
resolve to 0.0.0.0, and everything else is forwarded to your upstream resolver.

The blocklist is stored as compact hashes in flash and binary-searched, so it
fits on a 4 MB board with no PSRAM.

Licensed under MIT. Original C++ project by M-Abozaid.
