## BlitzWolf VC-1 reverse engineering info

### The PCB

The robot's electronics looks to be desinged by the [Slamtec](https://wiki.slamtec.com).


#### SOM

SLAMWARE Core Lite Module B1M4

More information could be found on the [Slamtec's wiki page](https://wiki.slamtec.com/pages/viewpage.action?pageId=7929902)

CPU: 
RAM: PoP (package on package)
Flash: 32 MB SPI flash
Ethernet: 

#### Base board

CPU: STM32F103VET6


#### Lidar

RoboPeak RPLidar (Classical slip ring + rubberband driven with DC motor)

#### Software

You can find a [SPI flash dump](readout.bin) in the repository from a dead unit I purchased second hand.

With [Binwalk](https://github.com/ReFirmLabs/binwalk) managed to extract multiple JFFS2 partitions which had been extracted with [jefferson](https://github.com/sviehb/jefferson)

You can find the extracted 
