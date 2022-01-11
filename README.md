## Starlight & VisionFive V1 RISC-V Fedora image
This is a respin of Fedora 33 to support the [StarFive JH7100 SoC](https://github.com/starfive-tech/JH7100_Docs/blob/main/JH7100%20Data%20Sheet%20V01.01.04-EN%20(4-21-2021).pdf) (RV64GC) and Starlight SBC board.  Please open issues regarding the Fedora image in [this repository](https://github.com/starfive-tech/Fedora_on_StarFive/issues).

### Download the latest image: 
**2021-December-26:** [Fedora-riscv64-jh7100-developer-xfce-Rawhide-20211226-214100.n.0-sda.raw.zst](https://fedora.starfivetech.com/pub/downloads/VisionFive-release/Fedora-riscv64-jh7100-developer-xfce-Rawhide-20211226-214100.n.0-sda.raw.zst)

* [sha256sum](https://fedora.starfivetech.com/pub/downloads/VisionFive-release/SHA256SUMS): `sha256sum: 94c73c967e12c80192d7bf25147badd9f0ee1738dc9800d1c502f376df5d5e2f`
* Changes:
  * Using the LTS kernel 5.15 with tag [linux-5.15.10](https://github.com/starfive-tech/linux/releases/tag/linux_5.15.10_devel_pwmdac);
  * Using the latest 5.16-rc6+ kernel - [starfive-tech/linux](https://github.com/starfive-tech/linux/tree/visionfive);
  * Support UVC camera using camorama application;
  * Support both of Starlight and VisionFive board;
  * Support ASLA driver and aplay audio files through the mini-jack on the board (only support 16kHz samplerate for now);
  * Fix kernel oops/crash issue by brcmfmac driver;
  * Fix the issue of not being able to switch some display resolutions;
* Issues:
  - Kernel panic when system booting with USB drive in rare case;
  - Real hot swap is not supported in case of HDMI is not connected before power-on;
  - Failed to open the Bilibili web page by firefox;


### Past images:
* **2021-November-29:** [Fedora-riscv64-jh7100-developer-xfce-Rawhide-20211129-184322.n.0-sda.raw.zst](https://fedora.starfivetech.com/pub/downloads/VisionFive-release/Fedora-riscv64-jh7100-developer-xfce-Rawhide-20211129-184322.n.0-sda.raw.zst)
  * [sha256sum](https://fedora.starfivetech.com/pub/downloads/VisionFive-release/SHA256SUMS): `sha256sum: 16e7a1e1e6445e6c04ac1bd7a7bbd36bb47a49d207560f6bcef0d6a614e4eac9`
  * Changes:
    * Using the 5.15.0 LTS kernel with RPM package;
    * Using the latest 5.16-rc2+ kernel - [starfive-tech/linux](https://github.com/starfive-tech/linux/tree/visionfive) with tag [linux_5.16_rc2_2021.11.27](https://github.com/starfive-tech/linux/releases/tag/linux_5.16_rc2_2021.11.27);
    * Support hardware watchdog;
    * Support both of Starlight and VisionFive board;
* **2021-October-27:** [Fedora-riscv64-jh7100-developer-xfce-Rawhide-20211027-130325.n.0-sda.raw.zst](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/Fedora-riscv64-jh7100-developer-xfce-Rawhide-20211027-130325.n.0-sda.raw.zst)
  * [sha256sum](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/SHA256SUMS): `sha256sum: c84fdf821c8e82c454da23d326cd6b8a91041e61748d5c51a8325e6ac3768dd9`
  * Changes:
    * Using the latest 5.15.0-rc7+ kernel - [starfive-tech/linux](https://github.com/starfive-tech/linux/commits/starlight) with tag [[linux_5.15_rc7_2021.10.28]](https://github.com/starfive-tech/linux/releases/tag/linux_5.15_rc7_2021.10.28)
    * Enable CONFIG_FRAMEBUFFER_CONSOLE;
    * Support Firefox browser;
    * Support podman;
* **2021-September-27:** [Fedora-riscv64-developer-xfce-with-esp-Rawhide-20210927.n.1-sda.raw.zst](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/Fedora-riscv64-developer-xfce-with-esp-Rawhide-20210927.n.1-sda.raw.zst)
  * [sha256sum](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/SHA256SUMS): `sha256sum: 9484901d1f743a0a11ebb56b174a4d281cf66e445281458ce6086044da805ff4`
  * Changes: 
    * Using the latest 5.15.0-rc3+ kernel - [starfive-tech/linux](https://github.com/starfive-tech/linux/commits/starlight) with tag [linux_5.13_rc3_2021.10.01](https://github.com/starfive-tech/linux/tree/linux_5.13_rc3_2021.10.01)
    * Support Bluetooth module and load the correct firmware automatically - [issue#4](https://github.com/starfive-tech/Fedora_on_StarFive/issues/4)
    * Add DRM driver to support more HDMI displays - [issue#32](https://github.com/starfive-tech/Fedora_on_StarFive/issues/32)
    * Support grub to boot Fedora - [issue#3](https://github.com/starfive-tech/u-boot/issues/3)
    * Change NVDLA as a module
* **2021-August-22:** [Fedora-riscv64-developer-xfce-with-esp-Rawhide-20210822.n.0-sda.raw.zst](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/Fedora-riscv64-developer-xfce-with-esp-Rawhide-20210822.n.0-sda.raw.zst)
  * [sha256sum](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/SHA256SUMS): `sha256sum: 7078b9c19e1451136813a3a3409e4e90f4de44103cc302450cd8f236d6d8e2b2`
  * Changes: 
    * Using the latest 5.14.0-rc6+ kernel
    * Fix the stability of some TF cards based on 50MHz frequency SDIO - [issue#23](https://github.com/starfive-tech/Fedora_on_StarFive/issues/23)
    * Support pinctrl driver
* **2021-July-27:** [Fedora-riscv64-developer-xfce-with-esp-Rawhide-20210727.n.0-sda.raw.xz](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/Fedora-riscv64-developer-xfce-with-esp-Rawhide-20210727.n.0-sda.raw.xz)
  * [sha256sum](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/SHA256SUMS): `sha256sum: 02ba0418d93b87ab6988b67b06850cf847791bdc13408643119684806ede0016`
  * Changes:
    * using the latest 5.14.0-rc3+ kernel
    * WI-FI [brcmfmac] should work now
* **2021-July-7:** [Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210707.n.0-sda.raw.zst](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210707.n.0-sda.raw.zst)
  * [sha256sum](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/SHA256SUMS): `sha256sum: 239f439125afce187c34b530490e6e3d095bf98ee6ef03b6d212842f1a4dba32`
  * Changes:
    * using the latest 5.13 kernel
    * USB3 devices should now work
    * enabled POWER_RESET_TPS65086 so reboot now works
* **2021-June-18:** [Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210618.n.0-sda.raw.zst](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210618.n.0-sda.raw.zst)
  * [sha256sum](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/SHA256SUMS): `849b75dd5ccdc7a4a05d7ebf218394b4d3261fa177ec8559a513ba5a6a63703d`
* **2021-May-16:** [Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210516233526.n.0-sda.raw.zst](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210516233526.n.0-sda.raw.zst)
  * [sha256sum](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/SHA256SUMS): `ab916cf46efc57c034aba8f79018a3af70a67d121126cbec271cdc12cdf64f05`
  * Note: [supports XFCE desktop on HDMI](https://github.com/starfive-tech/Fedora_on_StarFive/issues/22#issuecomment-841719888)
* **2021-April-19:** [Fedora-riscv64-vic7100-dev-raw-image-Rawhide-20210419121453.n.0-sda.raw.zst](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/Fedora-riscv64-vic7100-dev-raw-image-Rawhide-20210419121453.n.0-sda.raw.zst)
  * [sha256sum](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/SHA256SUMS): `e3d0df18d2eeb913aafabbb975c7a8803fdae333643a946b20607060e18df0db`
