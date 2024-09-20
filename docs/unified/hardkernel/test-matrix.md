# Test matrix

## About

The test matrix is used to determine the scope of tests which the DUT is
subjected from before the release of the new binary compatible with
Hardkernel devices.

=== "Hardkernel ODROID H4+"
    ## Module: Dasharo compatibility

    | No. | Supported test suite                  | Test suite ID | Supported test cases                 |
    |:---:|:--------------------------------------|:-------------:|:-------------------------------------|
    | 1.  | [Custom boot order][CBO]              | CBO           | CBO001.002                           |
    | 2.  | [Custom Boot Keys][CBK]               | CBK           | All                                  |
    | 3.  | [Custom logo][CLG]                    | CLG           | All                                  |
    | 4.  | [USB HID and MSC Support][USB]        | USB           | USB001.0001, USB001.002, USB002.001, USB002.002|
    | 5.  | [Custom network boot entries][CNB]    | CNB           | CNB001.002                           |
    | 6.  | [UEFI compatible interface][EFI]      | EFI           | EFI001.001                           |
    | 7.  | [UEFI Shell][USH]                     | USH           | All                                  |
    | 8.  | [NVMe support][NVM]                   | NVM           | NVM001.001, NVM001.002               |
    | 9.  | [Network boot][PXE]                   | PXE           | All                                  |
    | 10. | [Display ports][DSP]                  | DSP           | DSP002.001, DSP003.001               |
    | 11. | [Audio subsystem][AUD]                | AUD           | AUD007.001, AUD008.001               |
    | 12. | [Sleep mode][SUSP]                    | SUSP          | SUSP001.001, SUSP002.001, SUSP003.001, SUSP005.001|
    | 13. | [SMBIOS verification][DMI]            | DMI           | All                                  |
    | 14. | [eMMC support][MMC]                  | MMC           | All                                  |
    | 15. | [SATA support][SATA]                  |               | All                                  |
    | 16. | [Sign of life][SOL]                   | SOL           | All                                  |
    | 17. | [Persistent Boot Splash][LCM]         | LCM           | All                                  |
    | 18. | [Debian Stable and Ubuntu LTS support][LBT] | LBT     | LBT003.001, LBT003.002, LBT004.001, LBT004.002|
    | 19. | [Power state after power fail][PSF]    | PSF           | All                                  |
    | 20. | [Dasharo Tools Suite][DTS]            | DTS           | DTS001.001, DTS002.001, DTS003.001, DTS004.001, DTS005.001, DTS006.001 |
    | 21. | [Reset to defaults][RTD]              | RTD           | RTD001.001, RTD002.001, RTD003.001, RTD004.001, RTD006.001 |
    | 22. | [Ethernet interface][NET]             | NET           | All                                  |
    | 23. | [Dasharo Configuration Utility][NET]  | DCU           | DCU001.001, DCU002.001, DCU003.001   |
    | 24. | [ESP scanning][ESP]                   | ESP           | All                                  |
    | 25. | [Network Boot Utilities][NBT]          | NBT           | All                                  |
    | 26. | [USB detection][UDT]                  | UDT           | All                                  |
    | 27. | [USB booting][UBT]                    | UBT           | All                                  |
    | 28. | [Setup Menu information][SET]         | SET           | All                                  |
    | 29. | [Ubuntu booting performance test][BUB]| BUB           | All                                  |
    | 30. | [CPU status][CPU]                     | CPU           | CPU001.001, CPU002.001, CPU003.001, CPU004.001|
    | 31. | [Auto boot time-out][BMM]             | BMM           | All                                  |

    [CBO]: .
    [CBK]: ../../unified-test-documentation/dasharo-compatibility/303-custom-boot-menu-key.md
    [CLG]: ../../unified-test-documentation/dasharo-compatibility/304-custom-logo.md
    [USB]: ../../unified-test-documentation/dasharo-compatibility/306-usb-hid-and-msc-support.md
    [CNB]: ../../unified-test-documentation/dasharo-compatibility/30A-custom-network-boot-entries.md
    [EFI]: ../../unified-test-documentation/dasharo-compatibility/30M-uefi-compatible-interface.md
    [USH]: ../../unified-test-documentation/dasharo-compatibility/30P-uefi-shell.md
    [NVM]: .
    [PXE]: ../../unified-test-documentation/dasharo-compatibility/315-network-boot.md
    [DSP]: ../../unified-test-documentation/dasharo-compatibility/31E-display-ports-and-lcd.md
    [AUD]: ../../unified-test-documentation/dasharo-compatibility/31F-audio-subsystem.md
    [SUSP]: .
    [DMI]: ../../unified-test-documentation/dasharo-compatibility/31L-smbios.md
    [MMC]: .
    [SATA]: .
    [SOL]: .
    [LCM]: .
    [LBT]: ../../unified-test-documentation/dasharo-compatibility/308-debian-stable-and-ubuntu-lts-support.md
    [PSF]: .
    [DTS]: ../../unified-test-documentation/dasharo-compatibility/326-dasharo-tools-suite.md
    [RTD]: .
    [NET]: .
    [DCU]: .
    [ESP]: .
    [NBT]: ../../unified-test-documentation/dasharo-compatibility/315b-netboot-utilities.md
    [UDT]: ../../unified-test-documentation/dasharo-compatibility/31O-usb-detect.md
    [UBT]: ../../unified-test-documentation/dasharo-compatibility/31N-usb-boot.md
    [SET]: .
    [BUB]: .
    [CPU]: ../../unified-test-documentation/dasharo-compatibility/31T-cpu-status.md
    [BMM]: .

<!--
    ## Module: Dasharo security

    | No. | Supported test suite                  | Test suite ID | Supported test cases                 |
    |:----|:--------------------------------------|:-------------:|:-------------------------------------|
    | 1.  | [Secure Boot support][SBO]            | SBO           | All                                  |
    | 2.  | [BIOS lock support][BLS]              | BLS           | All                                  |
    | 3.  | [SMM BIOS write protection][SMM]      | SMM           | All                                  |
    | 4.  | [UEFI Setup password][PSW]            | PSW           | All                                  |
    | 5.  | [Network stack enable/disable][NBA]   | NBA           | All                                  |
    | 6.  | [USB stack enable/disable][USS]       | USS           | All                                  |

    [SBO]: ../../unified-test-documentation/dasharo-security/206-secure-boot.md
    [BLS]: ../../unified-test-documentation/dasharo-security/20J-bios-lock-support.md
    [SMM]: ../../unified-test-documentation/dasharo-security/20O-SMM-bios-write-protection.md
    [PSW]: ../../unified-test-documentation/dasharo-security/20R-uefi-setup-password.md
    [NBA]: ../../unified-test-documentation/dasharo-security/20T-network-boot.md
    [USS]: ../../unified-test-documentation/dasharo-security/20S-usb-stack.md

    ## Module: Dasharo performance

    | No. | Supported test suite                  | Test suite ID | Supported test cases                 |
    |:----|:--------------------------------------|:-------------:|:-------------------------------------|
    | 1.  | [coreboot bring up time measurement][CBMEM] | CBMEM         | All                            |
    | 2.  | [CPU temperature measure][CPT]        | CPT           | All                                  |
    | 3.  | [CPU frequency measure][CPF]          | CPF           | Without CPU003.XXX and CPU005.XXX    |
    | 4.  | [Platform stability][STB]             | STB           | All                                  |

    [CBMEM]: ../../unified-test-documentation/dasharo-performance/400-coreboot-boot-measure.md
    [CPT]: ../../unified-test-documentation/dasharo-performance/401-cpu-temperature.md
    [CPF]: ../../unified-test-documentation/dasharo-performance/402-cpu-frequency.md
    [STB]: ../../unified-test-documentation/dasharo-performance/404-platform-stability.md
    [BUB]: ../../unified-test-documentation/dasharo-performance/407-ubuntu-booting-performance-test.md
    [BDE]: ../../unified-test-documentation/dasharo-performance/408-debian-booting-performance-test.md
-->
