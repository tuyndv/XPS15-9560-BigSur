# XPS15 9560 BigSur

> XPS15 9560 Hackintosh OpenCore Config.

## Configuration

- CPU：Intel I7 7700HQ
- RAM：16G(8G\*2) 2400MHz DDR4
- HardDisk：PM961 NVMe SAMSUNG 1024GB
- WIFI：Intel® Wi-Fi 6 AX200
- Screen：4K(touch)

## What's not Working

1. Fingerprint sensor
2. Discrete graphic card, since macOS doesn't support Optimus technolog
3. ~~SD Card Reader~~
4. ~~USB Type-C Hotplug~~
5. Everything else works well
6. Known bug: The Refresh-Rate is only 48Hz at 4K resolution

## Installation

If the tracpad doesn't work during installation, please plug a wired mouse or a wireless mouse projector before the installation. After the installation completes, open `Terminal.app` and type `sudo kextcache -i /`. Wait for the process ending and restart the device. Enjoy your trackpad!

## Warning

1. Don't turn on `FileValue Encryption`！！！
2. Before using `OpenCore`, please make sure you have disabled `CFGlock`! If you don't disable `CFGLock`, you need change values of `AppleXcpmCfgLock` and `IgnoreInvalidFlexRatio` must be `True` or you will boot failure.