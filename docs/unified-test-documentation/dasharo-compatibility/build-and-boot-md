# Dasharo Compatibility: Building from source on a newly installed OS works

## Test cases common documentation

**Test setup**

1. Proceed with the
   [Generic test setup: firmware](../generic-test-setup.md#firmware).

## BNO001.001 Build on a Newly installed OS (Ubuntu)

**Test description**

This test aims to verify that Dasharo is buildable on freshly installed Ubuntu.

**Test configuration data**

1. `FIRMWARE` = Dasharo
1. `OPERATING_SYSTEM` = Ubuntu

**Test steps**
1. If the Ubuntu on the device is not freshly installed, install a clean one.
Do not use the preseeds suggested in [Generic Test Setup](../generic-test-setup.md#os-installer)
. You can get a clean installer from [ubuntu.com](https://ubuntu.com/download).
1. Boot into Ubuntu
1. Build the Dasharo firmware for the DUT following the build instructions
from docs.dasharo.com for this device. For example [Novacustom building manual](../../unified/novacustom/building-manual.md)
in the case of testing on a Novacustom laptop.
1. Flash the built firmware on the device using the instructions for the device
from docs.dasharo.com. For example [Novacustom firmware update](../../unified/novacustom/firmware-update.md)
in the case of testing on a Novacustom laptop.

**Expected result**
The build process should result in creating a rom file, which will be
possible to flash onto the device.

## BNO001.002 Boot (Ubuntu)

**Test description**

This test aims to verify that Ubuntu Linux is bootable with the firmware built
using the instructions at docs.dasharo.com.

**Test configuration data**

1. `FIRMWARE` = Dasharo
1. `OPERATING_SYSTEM` = Ubuntu

**Test steps**
1. Power on the DUT.
1. Boot into Ubuntu.

**Expected result**
There was no message that the device booted from recovery.
The OS boots properly.

## BNO001.003 Boot (Windows)

**Test description**

This test aims to verify that Windows is bootable with the firmware built
using the instructions at docs.dasharo.com.

**Test configuration data**

1. `FIRMWARE` = Dasharo
1. `OPERATING_SYSTEM` = Windows

**Test steps**
1. Power on the DUT.
1. Boot into Windows.

**Expected result**
There was no message that the device booted from recovery.
The OS boots properly.
