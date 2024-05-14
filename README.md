# audioreach-conf

## Introduction
This repository aims to host configuration files read by various AudioReach components for different vendor/chipset/board.

## Directory structure

Configuration files for vendor/chip/board to follow below structure:
```
├── <vendor specific dir>
    ├── kvh2xml.h
    └── <chip specific dir>
        ├── chip config files
        └── <board specific dir>
            ├── board config files
```
### File description
* kvh2xml.h: Defines key-values used in ACDB data file.

## Build instructions

Instructions to use audioreach-conf on OpenEmbedded system will be updated soon.

## License
audioreach-conf is licensed under the BSD-3-Clause-Clear. Check out the [LICENSE](LICENSE) for more details.