## BeagleV Starlight RISC-V Fedora image
This is a respin of Fedora 33 to support the [StarFive JH7100 SoC](https://github.com/starfive-tech/beaglev_doc/blob/main/JH7100%20Data%20Sheet%20V01.01.04-EN%20(4-21-2021).pdf) (RV64GC) and [BeagleV Starlight board](https://github.com/beagleboard/beaglev-starlight).  Find more details in the [BeagleV Starlight getting started guide](https://wiki.seeedstudio.com/BeagleV-Getting-Started/).  Please open issues regarding the Fedora image in [this repository](https://github.com/starfive-tech/beaglev_fedora/issues).

### Download the latest image: 
* **2021-July-27:** [Fedora-riscv64-developer-xfce-with-esp-Rawhide-20210727.n.0-sda.raw.xz](http://fedora.starfivetech.com/pub/downloads/BeagleV-release/Fedora-riscv64-developer-xfce-with-esp-Rawhide-20210727.n.0-sda.raw.xz)
  * [sha256sum](https://beagleboard.org/~pdp7/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210707.n.0-sda.raw.zst.sha256sum): `sha256sum: 02ba0418d93b87ab6988b67b06850cf847791bdc13408643119684806ede0016`
  * Changes:
    * using the latest 5.14.0-rc3+ kernel from GitHub - [starfive-tech/linux](https://github.com/starfive-tech/linux/commits/beaglev)
    * WI-FI [brcmfmac] should work now


### Past images:
* **2021-July-7:** [Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210707.n.0-sda.raw.zst](https://files.beagle.cc/file/beagleboard-public-2021/images/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210707.n.0-sda.raw.zst)
  * [sha256sum](https://beagleboard.org/~pdp7/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210707.n.0-sda.raw.zst.sha256sum): `sha256sum: 239f439125afce187c34b530490e6e3d095bf98ee6ef03b6d212842f1a4dba32`
* **2021-June-18:** [Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210618.n.0-sda.raw.zst](https://files.beagle.cc/file/beagleboard-public-2021/images/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210618.n.0-sda.raw.zst)
  * [sha256sum](https://files.beagle.cc/file/beagleboard-public-2021/images/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210618.n.0-sda.raw.zst.sha256sum): `849b75dd5ccdc7a4a05d7ebf218394b4d3261fa177ec8559a513ba5a6a63703d`
* **2021-May-16:** [Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210516233526.n.0-sda.raw.zst](https://files.beagle.cc/file/beagleboard-public-2021/images/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210516233526.n.0-sda.raw.zst)
  * [sha256sum](https://files.beagle.cc/file/beagleboard-public-2021/images/Fedora-riscv64-vic7100-xfce-dev-Rawhide-20210516233526.n.0-sda.raw.zst.sha256sum): `ab916cf46efc57c034aba8f79018a3af70a67d121126cbec271cdc12cdf64f05`
  * Note: [supports XFCE desktop on HDMI](https://github.com/starfive-tech/Fedora_on_StarFive/issues/22#issuecomment-841719888)
* **2021-April-19:** [Fedora-riscv64-vic7100-dev-raw-image-Rawhide-20210419121453.n.0-sda.raw.zst](https://files.beagle.cc/file/beagleboard-public-2021/images/Fedora-riscv64-vic7100-dev-raw-image-Rawhide-20210419121453.n.0-sda.raw.zst)
  * [sha256sum](https://files.beagle.cc/file/beagleboard-public-2021/images/Fedora-riscv64-vic7100-dev-raw-image-Rawhide-20210419121453.n.0-sda.raw.zst.sha256sum): `e3d0df18d2eeb913aafabbb975c7a8803fdae333643a946b20607060e18df0db`
