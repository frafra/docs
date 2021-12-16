# Dasharo Compatibility: Network Boot

## Test cases

### PXE001.001 iPXE network boot

**Test description**

This test aims to verify that the DUT is capable of network booting and logging
into `Debian` from an iPXE server.

**Test configuration data**

1. `BOOT_MENU_KEY` = `ESC`
2. `BOOT_MENU_STRING` = `Press ESC for boot menu`

**Test setup**

1. Proceed with the [Generic test setup: firmware](generic-test-setup.md#firmware).

**Test steps**

1. Power on the DUT.
2. Wait for boot until `BOOT_MENU_STRING` appears.
3. Press `BOOT_MENU_KEY` to enter the boot menu.
4. Select the key with a proper number for `iPXE`.
5. Press `Ctrl+B` when prompted to stop iPXE from booting automatically.
6. Wait until `iPXE>` prompt appears.
7. Type in `dhcp` to obtain an IP address.
8. Type in `chain` and local iPXE address after a single space to load a network 
boot menu.
8. Select `Debian stable netboot 4.14.y` option below `iPXE boot menu` header.
9.  Wait for `debian login:`.
10. Type the `root` login.
11. Wait for `Password:`.
12. Type the proper password.
13. Wait for `root@debian:~#`.

**Expected result**

1. The iPXE application boots successfully.
2. iPXE obtains an IP address.
3. iPXE boots a `Debian` from the local network.