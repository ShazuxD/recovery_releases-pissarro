### TWRP / OFOX (PISSARRO)

# Flashing Instructions

[**Download the latest release here!**](https://github.com/ShazuxD/recovery_releases-pissarro/releases/)

## TWRP

1. Download the TWRP image from the latest release.
2. Flash TWRP using the following command:

   ```bash
   fastboot flash boot twrp_3.7.1_pissarro.img
   ```

3. Reboot into recovery:

   ```bash
   fastboot reboot recovery
   ```

## Notes

- **Custom ROMs:** Do not permanently install TWRP/OFOX on custom ROMs, as this may cause a bootloop, possibly due to LK or `vbmeta` issues.
- **HyperOS:** Permanent installation is supported on HyperOS. Follow the instructions below carefully.
- Always make sure you have the correct boot image for your current ROM or kernel before proceeding.

## Permanently Installing TWRP on HyperOS

1. Make sure you have the stock HyperOS `boot.img` or a compatible custom kernel.
2. Flash the TWRP image:

   ```bash
   fastboot flash boot twrp_3.7.1_pissarro.img
   ```

3. Reboot directly into TWRP recovery:

   ```bash
   fastboot reboot recovery
   ```

4. In TWRP, flash the stock HyperOS `boot.img` to the appropriate boot slot.

5. Open the TWRP settings menu and select **Flash Current TWRP** to install TWRP permanently.

### Alternative Method: Using a Custom Kernel

Instead of flashing the stock `boot.img`, you can flash a compatible custom kernel ZIP through TWRP. In this case, **skip the Flash Current TWRP step** if instructed by the kernel's installation procedure.

Once finished, reboot your device.

## Flashing ROMs

Always follow the appropriate flashing guide for the ROM you intend to install. Make sure to verify compatibility and follow all instructions carefully to avoid bootloops or other issues.
