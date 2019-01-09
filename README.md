# EVB-KSZ9477
EVB-KSZ9477 Repository

To Build

1. Create the source tree
$ git clone https://github.com/nconnolly/EVB-KSZ9477.git
Or download the zip file from the following location and extract them on to your working folder.
https://github.com/Microchip-Ethernet/EVB-KSZ9477
2. Change directory to KSZ folder
$ cd EVB-KSZ9477/KSZ
3 . Export KSZ_HOME variable to KSZ folder
$ export KSZ_HOME=`pwd`
4. Change directory to Atmel_SOC_SAMA5D3/buildroot
$ cd Atmel_SOC_SAMA5D3/buildroot
5. Decide whether you need NAND flash image or SD card image
If you need NAND flash image:
$ make atmel_sama5d3_xplained_ksz9897_defconfig
If you choose SD card image:
$ make atmel_sama5d3_xplained_ksz9897_mmc_defconfig
6. Build
$ make clean all
7. The images will be created @
$KSZ_HOME/Atmel_SOC_SAMA5D3/buildroot/output/images
