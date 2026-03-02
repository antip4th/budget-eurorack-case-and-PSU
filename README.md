# budget-eurorack-case-and-PSU
This repo contains all files to build your own budget 84HP Eurorack case with intrgrated PSU and an optional filter PCB.
Ok, it is not really a case, as in "enclosure", because it is not enclosed, but it is still a fairly inexpensive solution to house your modules, compared to other cases.

The buld features two MeanWell PSUs, each of which supplies up to 3A in theory, which should be more than enough for a 84HP case. Only +-12 V supplies, no +5 V.

BOM Case:
|Part  |Quantity  |Price  (Feb. 2026)  | Link |
|------|----------|--------------------|------|
| Mean Well RS-35-12 PSU | 2 | 13.36 € | [DigiKey](https://www.digikey.de/en/products/detail/mean-well-usa-inc/RS-35-12/7706181) |
| Doepfer Bus board V6 | 1 | 40 € | [Schneidersladen](https://schneidersladen.de/en/doepfer-a-100-bus-board-v6) |
| 84HP eurorack rails with edge | 2 | 9 € | [Schneidersladen](https://schneidersladen.de/en/divers-sb-rail-19-with-lip) |
| 84 HP eurorack rails without edge | 1 | 10 € | [Schneidersladen](https://schneidersladen.de/en/divers-sb-rail-19-without-lip) |
| M3 slider nuts or threaded strips | 1 | 8 - 10 € | [Nuts - Schneidersladen](https://schneidersladen.de/en/frap-tools-sliding-nuts-100-pcs) |
| | | | [Threaded strips - Schneidersladen](https://schneidersladen.de/en/divers-threaded-strip-with-m3-threads-84hp) |
| M5x25 or M5x20 socket head screws | 6 | Included with rails if you order from Schneidersladen | [Amazon](https://a.co/d/07VXTLld) |
| | | ~ 8.00 € otherwise | |
| M3x6 socket head screw | 6 | | | 
| M3x5 button head screw | 2-4 | | |
| AC Cold appliances built-in plug | 1 | ~ 8 € | [Amazon](https://amzn.eu/d/06RYOiwI) |
| 0.75 mm²/18 AWG silicone cable | 1 m | 13 € | [Amazon](https://amzn.eu/d/0fPG9uPr) |
| Insulated cable lugs | 1 | 7 € | [Amazon](https://amzn.eu/d/0cKYAwAh) |
| Fork wire terminals | 1 | 7 € | [Amazon](https://amzn.eu/d/0jiY2vDV) |
| 3D-printed parts | | 3 | |
| SUM | | ~ 150 € worst case | |  

In total, this is quite affordable for an Eurorack case, with busboard and PSUs included. And the total price includes some excess materials, like excess cables and screws etc.  
To dampen some of the PSU switching noise, I designed a custom filter PCB. It offers one pi-filter per PSU and it removes the switching voltage spikes on the power rails.

BOM Filter PCB:
