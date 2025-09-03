##############################################################################
Overview
##############################################################################

To boot Raspberry Pi 5 from an NVMe SSD, two core tasks need to be accomplished:

**1、Flash the Raspberry Pi's operating system image onto the NVMe SSD.**

2、Configure the boot order of Raspberry Pi to give priority to SSD. (Optional)

Analysis
**********************

1.	First of all, make sure you can enter the Raspberry Pi OS via SD card or U drive.

2.	After booting the Raspberry Pi, you can use it to flash the OS image directly onto the NVMe SSD. Alternatively, you can purchase an NVMe SSD to USB adapter and flash the image using USB on Windows or macOS, much like you would for an SD card or USB drive.

3.	With this analysis in mind, we can systematically carry out the necessary steps.
 
Raspberry Pi models manufactured at different times might not boot up in the same way as described, but that's okay; just follow our guide to proceed.

There are various ways to flash the Raspberry Pi OS to SSD, each requiring different hardware tools.

.. table::
    :align: center
    :width: 80%
    :class: zebra

    +------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------+
    | Ways |                                                                          Flashing Methods                                                                           |                        Requirements                         |
    +======+=====================================================================================================================================================================+=============================================================+
    | 1    | Use Raspberry Pi to flash the OS. This requires that you can successfully boot up the Raspberry Pi via SD card or U disk. (Recommended, described in this tutorial) | An SD card or a U disk that can access the Raspberry Pi OS. |
    +------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------+
    | 2    | Purchase an NVMe SSD to USB adapter and flash the image just like you would with an SD card or USB drive.                                                           | NVME SSD to USB adapter (need to be bought separately)      |
    +------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------+
    | 3    | If there are spare M.2 NVME interface on the motherboard of your PC, you can insert the SSD to it to flash the OS.                                                  | PC with M.2 NVME interface                                  |
    +------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------+

Caution: Incompatible SSDs
***********************************

The recognition and reading/writing of the NVME SSD are handled by the drivers of the Raspberry Pi 5. The 4-Slot SSD Adapter Board or 2-Slot SSD Adapter Board serves to connect and power the SSD. If you find that your SSD is not recognized or readable/writeable by the Pi 5, please try to find the drivers suitable for your SSD and install them on the Raspberry Pi, or replace the SSD, or purchase our Adapter kit that comes with an SSD.