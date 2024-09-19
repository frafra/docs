# Dasharo firmware building guide

## Intro

This guide shows how to build Dasharo firmware for Hardkernel devices.


## Requirements

- Docker
    + follow [Install Docker Engine on Ubuntu](https://docs.docker.com/engine/install/ubuntu/)
    + follow [Post-installation steps for Linux](https://docs.docker.com/engine/install/linux-postinstall/)
- Git
    + `sudo apt-get install git`

## Building

To build Dasharo firmware image, first clone the coreboot repository:
    ```bash
    git clone https://github.com/Dasharo/coreboot.git
    ```
then follow the steps below:

=== "Odroid H4+"

    1. Checkout to the device's branch:
            ```bash
            cd coreboot
            git checkout hardkernel_odroid_h4/release
            ```

    To build a specific version replace `hardkernel_odroid_h4/release` with
    `hardkernel_odroid_h4_v0.9.x` where `x` is the version number.

    2. Checkout submodules:

    ```bash
    git submodule update --init --checkout
    ```
    3. Build the firmware:

    ```bash
    ./build.sh odroid_h4
    ```

    The resulting coreboot image will be placed in the coreboot directory as
    `hardkernel_odroid_h4.rom`.
