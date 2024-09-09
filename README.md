# Toshiba Tecra 500/510 series HDD adapter

This adapter converts the Toshiba Tecra 500/510 series laptop's proprietary HDD connector, to a standard 2.5" IDE 44-pin HDD connector. You can use normal 2.5" HDD up to 17mm thickness in the Toshiba Tecra 500/510 laptops (but keep in mind that the laptop BIOS does not support HDD larger than a certain size, I think it is 10GB? Just a disclaimer).

I built a couple of extra adapters and offered them for sale on [Tindie](https://www.tindie.com/products/35777/).

This design was inspired by the discussions in [this vogons post](https://www.vogons.org/viewtopic.php?f=46&t=83221). Thanks for all the previous contributors! If you have any suggestions to this adapter, you can reply to that post on vogons.

If you want to build this adapter yourself, keep in mind that the most difficult thing is to find a seller that sells this proprietary connector (that is, for a small quantity, at a reasonable price, e.g. \< $6). So buy the connector first before ordering the PCB, try your luck on Taobao, Aliexpress,eBay, Mouser etc. The IDE receptacle is a standard 2x22p, 2mm-pitch pin socket, you can buy it pretty easily. 

You can use any of the following model:

Use without modifying:

| Manufacturer | Model | Note | Datasheet |
| :---- | :---- | :---- | :---- |
| KEL | 8913-050-178S-A (or \-A-F) | Through-Hole, straight version | [8900-SERIES](https://www.bce.it/wp-content/uploads/2019/06/KEL-8900-SERIES\_BCE.pdf) |
| KEL | 8913-050-178MS-A | SMT version | [8900MS-SERIES](https://www.bce.it/wp-content/uploads/2019/06/KEL-8900MS-SERIES\_BCE.pdf) |
| KEL | 8911-050-178S-A | Through-Hole, straight version | [8900-SERIES](https://www.bce.it/wp-content/uploads/2019/06/KEL-8900-SERIES\_BCE.pdf) |

Use after dremeling off the flanges on both ends:

| Manufacturer | Model | Note | Datasheet |
| :---- | :---- | :---- | :---- |
| KEL | 8931E-050-178S-F | Through-Hole, straight version | [8925 series](https://www.kel.jp/files/topics/490\_ext\_19\_en\_0.pdf) |
| KEL | 8930E-050-178S-F | SMT version | [8925 series](https://www.kel.jp/files/topics/490\_ext\_19\_en\_0.pdf) |
| 3M | P50LE-050P1-R1-DA | Through-Hole, straight version | [P50LE series](https://multimedia.3m.com/mws/media/218453O/3mtm-050-in-low-profile-plug-050-strt-ra-smt-ts1148.pdf) |
| 3M | P50LE-050P1-SML-DA | SMT version | [P50LE series](https://multimedia.3m.com/mws/media/218453O/3mtm-050-in-low-profile-plug-050-strt-ra-smt-ts1148.pdf) |

(BTW, the laptop side's connector seems to be KEL 8901-050-177S-A)

I have provided the PCB design for both Through-hole and SMT versions in the `pcb/` folder. You can use the Gerber file to order PCBs from your selected PCB factory. Choose the version (Through-hole vs. SMT) based on the connector type you have bought. The SMT soldering would be more difficult by hand, a hotair station is recommended. The PCB is designed using LCEDA (an online PCB drawing tool), I'll pulicize the LCEDA project when it is stable.

I've also included a 3d-printed HDD caddy design. The stl file is at the `3d_print/` folder. The 3d model is designed using Tinkercad. You can remix it [here](https://www.tinkercad.com/things/9fCpsQH187o-toshiba-tecra-510cdt-hdd-caddy) if you want. Print using PETG for better heat resistance, because HDD becomes hot when operating.

## Building tips

It is recommended to trim the pins flush to the PCB *BEFORE* soldering the through-hole components to the PCB, so that they do not extrude too high on the other side. Use a piece of electrical tape to cover the solder pads after soldering, to avoid accidental short with the metal frame of the laptop.

## Gallery

EDA design

![eda](/images/eda.jpg)

Parts

![parts](/images/parts.jpg)

Assembled

![assembled](/images/assembled.jpg)

PC side

![pc_side](/images/pc_side.jpg)

HDD side

![hdd_side](/images/hdd_side.jpg)

Solder points insulated.

![solder_pad_insulated_1](/images/solder_pad_insulated_1.jpg)

![solder_pad_insulated_2](/images/solder_pad_insulated_2.jpg)





