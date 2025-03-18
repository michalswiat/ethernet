# 10BASE-T
10Mb/s Ethernet standard defined in IEEE 802.3.

## Modes
It can operate in half-duplex or full-duplex mode using twisted pair. Currently single port mode is widely used
in industrial area.

### Full duplex
[1] Widely used, separate pair for Tx and Rx

### Half duplex
[2] The Tx and Rx is done on the same pair. There is a need for collision detection.

[1] https://en.wikipedia.org/wiki/Duplex_(telecommunications)  
[2] https://en.wikipedia.org/wiki/Duplex_(telecommunications)  

## PHY encoding
In 10BASE-T manchester encoding is used on transimt and recevice. Bunch of filters and transformator needs to be used
to convert digital signal into ethernet standard.

## Example projects 

- ATtiny bit-banging 10BASE-T [3]
- FPGA bit-banging 10BASE-T [4]
- RPI bit-banging 10BASE-T [5]
- no CPU SPI to 10BASE-T [6] or whole NIC [7]

[3] https://hackaday.com/2014/08/29/bit-banging-ethernet-on-an-attiny85/  
[4] https://hackaday.com/2016/01/02/fpga-to-ethernet-direct/  
[5] https://hackaday.com/2022/08/26/bit-banged-ethernet-on-the-raspberry-pi-pico/  
[6] https://qdiv.dev/posts/eth-to-spi/  
[7] https://qdiv.dev/posts/eth2/  

## About the Ethernet

- brief history [8]
- basic and some more [9] (more than one article)
- sth about cabels [10]
- hostory of old NIC card [11]

[8] https://hackaday.com/2020/10/19/ethernet-at-40-from-a-napkin-sketch-to-multi-gigabit-links/  
[9] https://hackaday.com/2024/02/12/ethernet-for-hackers-the-very-basics/  
[10] https://hackaday.com/tag/10base2/  
[11] https://hackaday.com/2021/04/24/was-novells-ne2000-really-that-bad/  

## Few devices which support for 10BASE-T

It is PHY, or PHY and MAC. A lot of implementation details in datasheet.

PHY:
- DP83848 (TI, single port) [12]
- ADIN1100 (Analig device, single port) [13]
- TLK100 (TI, single port) [14]
- KSZ8081 (Microchip, half/full) [15]

PHY and MAC:
- DP83816 (TI/National semiductor, full-duplex) [16]
- ENC28J60 (Microchip, half/full) [17]
- LAN950x (Microchip, full) Ethernet to USB [18]
- LAN9514 (Microchip, full) Ethernet to USB [19]

[12] https://www.ti.com/lit/ds/symlink/dp83848-ep.pdf?HQS=dis-mous-null-mousermode-dsf-pf-null-wwe&DCM=yes&ref_url=https%3A%2F%2Fwww.mouser.pl%2F&distId=26  
[13] https://www.mouser.pl/datasheet/2/609/adin1100-2295795.pdf  
[14] https://www.ti.com/lit/ds/symlink/tlk100.pdf?ts=1742316405544&ref_url=https%253A%252F%252Fwww.google.com%252F  
[15] https://download.kamami.pl/p564299-ksz8081rnbca-tr.pdf  
[16] https://www.ti.com/lit/ds/symlink/dp83816ex.pdf?ts=1742326777465&ref_url=https%253A%252F%252Fwww.google.com%252F  
[17] https://download.kamami.pl/p26270-enc28j60.pdf  
[18] https://download.kamami.pl/p566167-LAN950x.pdf  
[19] https://download.kamami.pl/p565621-00002306A.pdf  
