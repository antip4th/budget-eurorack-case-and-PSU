# budget-eurorack-case-and-PSU #
This repo contains all files to build your own budget 84HP Eurorack case with intrgrated bus board, PSU and an optional filter PCB.

The case features two MeanWell PSUs, each of which supplies up to 3 A in theory. This should be more than enough for a 84HP case. Only +-12 V supplies, no +5 V.

The cost is about 150 € max. Less, if you already have some cables and screws.
I found this was quite affordable for an Eurorack case, with busboard, PSU mounting screws etc. included.

To dampen some of the PSU switching noise, I designed a custom filter PCB. It offers one pi-filter per PSU and it removes the switching voltage spikes on the power rails.
Also works well on prototyping board instead of the PCB.

![Case front View](images/front.jpg)

## BOM Case ## 
|Part  |Quantity  |Price  (Feb. 2026)  | Link |
|------|----------|--------------------|------|
| Mean Well RS-35-12 PSU | 2 | 13.36 € | [DigiKey](https://www.digikey.de/en/products/detail/mean-well-usa-inc/RS-35-12/7706181) |
| Doepfer Bus board V6 | 1 | 40 € | [Schneidersladen](https://schneidersladen.de/en/doepfer-a-100-bus-board-v6) |
| 84HP eurorack rails with lip | 2 | 9 € | [Schneidersladen](https://schneidersladen.de/en/divers-sb-rail-19-with-lip) |
| 84 HP eurorack rails without lip | 1 | 10 € | [Schneidersladen](https://schneidersladen.de/en/divers-sb-rail-19-without-lip) |
| M3 slider nuts or threaded strips | 1 | 8 - 10 € | [Nuts - Schneidersladen](https://schneidersladen.de/en/frap-tools-sliding-nuts-100-pcs) |
| | | | [Threaded strips - Schneidersladen](https://schneidersladen.de/en/divers-threaded-strip-with-m3-threads-84hp) |
| Module Screws | 1 | 6 € | [Schneidersladen](https://schneidersladen.de/en/frap-tools-m3x6-philips-panhead-screws-silver-100-pieces) |
| M5x25 or M5x20 socket head screws | 6 | Included with rails if you order from Schneidersladen | [Amazon](https://a.co/d/07VXTLld) |
| | | ~ 8.00 € otherwise | |
| M3x6 socket head screw | 6 | | | 
| M3x5 button head screw | 2-8 | | |
| AC Cold appliances built-in plug | 1 | ~ 8 € | [Amazon](https://amzn.eu/d/06RYOiwI) |
| 0.75 mm²/18 AWG silicone cable | 1 m | 13 € | [Amazon](https://amzn.eu/d/0fPG9uPr) |
| Insulated cable lugs | 1 | 7 € | [Amazon](https://amzn.eu/d/0cKYAwAh) |
| Fork wire terminals | 1 | 7 € | [Amazon](https://amzn.eu/d/0jiY2vDV) |
| 3D-printed parts | | 3 | |
| SUM | | ~ 150 € worst case | |  

## BOM Filter PCB ##
|Part  |Quantity  |Price  (Feb. 2026)  | Link |
|------|----------|--------------------|------|
| Low ESR electrolytic caps 1000 µF | 4 | 0.5 € | [reichelt](https://www.reichelt.com/de/en/shop/product/elko_radial_1000_f_25_v_105_low_esr_12_5x20_mm_rm_5-166391?search=RAD%2520LXZ%252025%252F1K0B&)|
| Ceramic caps 100 nF | 4 | 0.1 € | [reichelt](https://www.reichelt.com/de/en/shop/product/smd_multilayer_ceramic_capacitor_100_n_10_-22889?search=X7R-G1206%2520100n&) |
| Ferrite core inductor 10 μΗ | 2 | 1 € | [reichelt](https://www.reichelt.com/de/en/shop/product/vertical_inductor_09hcp_ferrite_10_h-138644?country=de&CCTYPE=private&LANGUAGE=en) |
| Custom PCB or prototyping board | 1 | ~15 € if you have the PCB manufactured | |
| SUM | | ~ 20 € | |

## Build Instructions

> [!CAUTION]
> Only work with mains voltage, if you know what you are doing!

The build is pretty straight forward for the general structure. The rails with lip go in the front, the rail without lip goes in the back and is for mounting the bus board. The part `PSUBoxRib` needs to be printed twice (one part mirrored). 
The PSUs are mounted to the `PSUBoxBottom` part with the M3x5 screws. **Do not use longer screws for this, as the screws could touch the PCU PCB!** 
The PSU mounting parts (`PSUBoxLid`, `PSUBoxRib`) need to be placed on the rails before the side panels are attached.
