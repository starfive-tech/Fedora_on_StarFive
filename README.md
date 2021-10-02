## Starlight RISC-V Fedora image
This is a respin of Fedora 33 to support the [StarFive JH7100 SoC](https://github.com/starfive-tech/StarLight_Docs/blob/main/JH7100%20Data%20Sheet%20V01.01.04-EN%20(4-21-2021).pdf) (RV64GC) and Starlight SBC board.  Please open issues regarding the Fedora image in [this repository](https://github.com/starfive-tech/Fedora_on_StarFive/issues).

### Download the latest image: 
* **2021-September-27:** [Fedora-riscv64-developer-xfce-with-esp-Rawhide-20210927.n.1-sda.raw.zst](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/Fedora-riscv64-developer-xfce-with-esp-Rawhide-20210927.n.1-sda.raw.zst)
  * [sha256sum](https://fedora.starfivetech.com/pub/downloads/BeagleV-release/SHA256SUMS): `sha256sum: 9484901d1f743a0a11ebb56b174a4d281cf66e445281458ce6086044da805ff4`
  * Changes:
    * Using the latest 5.15.0-rc3+ kernel - [starfive-tech/linux](https://github.com/starfive-tech/linux/commits/starlight) with tag [linux_5.13_rc3_2021.10.01](https://github.com/starfive-tech/linux/tree/linux_5.13_rc3_2021.10.01)
    * Support Bluetooth module and load the correct firmware automatically - [issue#4](https://github.com/starfive-tech/Fedora_on_StarFive/issues/4)
    * Add DRM driver to support more HDMI displays - [issue#32](https://github.com/starfive-tech/Fedora_on_StarFive/issues/32)
    * Support grub to boot Fedora - [issue#3](https://github.com/starfive-tech/u-boot/issues/3)
    * Change NVDLA as a module 
* Notes: Please use the release [u-boot binary](https://github.com/starfive-tech/Fedora_on_StarFive/releases/tag/fw_payload_1001_starlight) to test this Fedora image

### Past images:
* **2021-August-22:** [Fedora-riscv64-developer-xfce-with-esp-Rawhide-20210822.n.0-sda.raw.zst](https://fedora.starfivetech.com/pub/downloads/image-history/BeagleV-release/Fedora-riscv64-developer-xfce-with-esp-Rawhide-20210822.n.0-sda.raw.zst)
  * [sha256sum](https://fedora.starfivetech.com/pub/downloads/image-history/BeagleV-release/SHA256SUMS): `sha256sum: 7078b9c19e1451136813a3a3409e4e90f4de44103cc302450cd8f236d6d8e2b2`
* **2021-July-27:** [Fedora-riscv64-developer-xfce-with-esp-Rawhide-20210727.n.0-sda.raw.xz](https://fedora.starfivetech.com/pub/downloads/image-history/BeagleV-release/Fedora-riscv64-developer-xfce-with-esp-Rawhide-20210727.n.0-sda.raw.xz)
  * [sha256sum](https://beagleboard.org/~pdp7/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210707.n.0-sda.raw.zst.sha256sum): `sha256sum: 02ba0418d93b87ab6988b67b06850cf847791bdc13408643119684806ede0016`
* **2021-July-7:** [Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210707.n.0-sda.raw.zst](https://files.beagle.cc/file/beagleboard-public-2021/images/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210707.n.0-sda.raw.zst)
  * [sha256sum](https://beagleboard.org/~pdp7/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210707.n.0-sda.raw.zst.sha256sum): `sha256sum: 239f439125afce187c34b530490e6e3d095bf98ee6ef03b6d212842f1a4dba32`
* **2021-June-18:** [Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210618.n.0-sda.raw.zst](https://files.beagle.cc/file/beagleboard-public-2021/images/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210618.n.0-sda.raw.zst)
  * [sha256sum](https://files.beagle.cc/file/beagleboard-public-2021/images/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210618.n.0-sda.raw.zst.sha256sum): `849b75dd5ccdc7a4a05d7ebf218394b4d3261fa177ec8559a513ba5a6a63703d`
* **2021-May-16:** [Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210516233526.n.0-sda.raw.zst](https://files.beagle.cc/file/beagleboard-public-2021/images/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210516233526.n.0-sda.raw.zst)
  * [sha256sum](https://files.beagle.cc/file/beagleboard-public-2021/images/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210516233526.n.0-sda.raw.zst.sha256sum): `ab916cf46efc57c034aba8f79018a3af70a67d121126cbec271cdc12cdf64f05`
  * Note: [supports XFCE desktop on HDMI](https://github.com/starfive-tech/Fedora_on_StarFive/issues/22#issuecomment-841719888)
* **2021-April-19:** [Fedora-riscv64-vic7100-dev-raw-image-Rawhide-20210419121453.n.0-sda.raw.zst](https://files.beagle.cc/file/beagleboard-public-2021/images/Fedora-riscv64-vic7100-dev-raw-image-Rawhide-20210419121453.n.0-sda.raw.zst)
  * [sha256sum](https://files.beagle.cc/file/beagleboard-public-2021/images/Fedora-riscv64-vic7100-dev-raw-image-Rawhide-20210419121453.n.0-sda.raw.zst.sha256sum): `e3d0df18d2eeb913aafabbb975c7a8803fdae333643a946b20607060e18df0db`
