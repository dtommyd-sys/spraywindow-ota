# spraywindow-ota
Over-the-air firmware channel for the Spray Window glance device (LilyGO T-Display-S3).
- `version.txt` — integer build number the device compares to its own FW_VERSION.
- `spraywindow.bin` — firmware the device pulls when version.txt is higher. Contains NO wifi credentials (those live in the chip's NVS).
Push an update: bump FW_VERSION, compile the clean build, replace spraywindow.bin, set version.txt, push. Devices self-flash within ~30 min.
