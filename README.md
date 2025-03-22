# lora-antenna-notes
Antenna tests for LoRa radios

Antennas are tested for SWR with a calibrated [NanoVNA](https://meshmap.net/) on a wooden table approximately 36 inches off the ground to reduce reflections and ~24 inches from any metal objects. These are not incredibly scientific testing practices, and the NanoVNA is not a professional piece of test equipment, but the testing results here should be reasonable enough for hobbyists to make decisions and compare/contrast antennas and people have reported the NanoVNA to be within 95-98% accurate.

## SWR

We really concern outselves here with good SWR (Standing Wave Ratio) which essentially means how efficient the transmission is. The more efficient, the more power is actually being radiated and the further the signal goes. An ideal-but-not-obtainable SWR is 1.0, which means all the power is effectively radiated efficiently. This is really considered a theoretical case and only used for reference. Practical SWRs are as follows:

* SWR < 1.5 Great
* SWR < 2.0 Good
* SWR < 2.5 Bad
* SWR < 3 AVOID (could cause radio damage)

I personally like to use antennas with < 2.0 SWR.

## Gain

A lot of people assume the higher gain of an antenna the better, but this is not true. To put it into simple terms:

* A gain of 1 dBi is a bit like a sphere around the antenna, with the signal radiating equally in every direction.
* A gain of 3 dBi has the signal coming out at a 120 degree angle, creating a bit of a donut shape.
* A gain of 6 dBi has the signal coming out at a 60 degree angle, creating slightly flatter but wider donut
* A gain of 9 dbI has the signal coming out at a 30 degree angle, creating an even flatter and wider donut
* Higher gains often cause really strange and undesirable radiation patterns, having lobes shoot off in strange directions.

The tradeoff is that lower dBi antennas will radiate power in more directions but at an overall lower distance. 3 dBi antennas may be good for a dense city while 6 dBi antennas may be good for a more suburban setting, and 9 dBi antennas are better for a very flat environment.

## 915MHz Test Results Summary

### Portable Antennas

| Brand | Model | Gain (dBi) | Antenna Dimensions | Price | SWR | Suggested For Use? (Y/N) |
| --- | --- | --- | --- | --- | --- | --- |
| ALFA | [ARS-9096RP](https://www.alfa.com.tw/products/ars-9096rp?variant=39338137190472) | 5 | 431.8mm (L) x 12.954mm (W) | [$12.00](https://store.rokland.com/products/alfa-network-ars-9096rp-5-dbi-indoor-antenna-for-helium-hotspots) | [1.364](images/ALFA-ARS-9096RP.png) | ✔️ Yes |
| ALFA | [ARS-915P](https://www.alfa.com.tw/products/ars-915p?variant=36473964855368) | 2 | 195mm (L) x 13.3mm (W) | [$11.97](https://store.rokland.com/products/alfa-network-ars-915pr-2-dbi-sma-male-915-mhz-antenna-with-90-elbow-for-t-beam-t-echo-lora32) | [1.295](images/ALFA-ARS-915P.png) | ✔️ Yes |
| Linx | [ANT-916-CW-HWR-SMA](https://www.te.com/commerce/DocumentDelivery/DDEController?Action=srchrtrv&DocNm=ANT-916-CW-HWR-ccc&DocType=Data+Sheet&DocLang=English&DocFormat=pdf&PartCntxt=ANT-916-CW-HWR-SMA) | 1.2 | 142mm (L) x 10mm (W) | [$12.55](https://www.digikey.com/en/products/detail/te-connectivity-linx/ANT-916-CW-HWR-SMA/1139580) | [1.362](images/LINX-ANT-916-CW-HWR-SMA.png) | ✔️ Yes |
| Linx | [ANT-916-CW-RCL-SMA](https://www.te.com/commerce/DocumentDelivery/DDEController?Action=srchrtrv&DocNm=ant-916-cw-rcl-ccc&DocType=Data+Sheet&DocLang=English&DocFormat=pdf&PartCntxt=ANT-916-CW-RCL-SMAA) | 4.2 | 97.7mm (L) x 18.6mm (W) | [$7.87](https://www.digikey.com/en/products/detail/te-connectivity-linx/ANT-916-CW-RCL-SMA/13147742) | [1.988](images/LINX-ANT-916-CW-RCL-SMA.png) | ✔️ Yes |
| Linx | [ANT-916-CW-RCS-SMA](https://www.te.com/commerce/DocumentDelivery/DDEController?Action=srchrtrv&DocNm=CW-RCS_Series&DocType=Data+Sheet&DocLang=English&DocFormat=pdf&PartCntxt=ANT-916-CW-RCS-SMA) | 4.8 | 54mm (L) x 17.4mm (W) | [$7.62](https://www.digikey.com/en/products/detail/te-connectivity-linx/ANT-916-CW-RCS-SMA/1663028) | ??? | ✔️ Yes |
| Rabbit Labs | [HG 915mhz](https://rabbit-labs.com/product/cc1101-modules-compatible-antennas-by-rabbit-labs/?v=0b3b97fa6688) | 3.5 | 199.898mm (L) x 12.7mm (W) | [$6.25](https://www.amazon.com/Generic-Rabbit-Labs-Connector-Compatible-Meshtastic/dp/B0D19JJBKZ/) | [1.673](images/RABBIT-LABS-HG915.png) | ✔️ Yes |
| Unknown | [Station G2 Antenna](https://shop.uniteng.com/product/meshtastic-mesh-device-station-edition/) | ??? | 195mm (L) x 13.3mm (W) | N/A | [1.872](images/STATION_G2_GENERIC.png) | ✔️ Yes |

### Fixed (Base) Antennas

| Brand | Model | Gain (dBi) | Pattern | Antenna Dimensions | Price | SWR | Suggested For Use? (Y/N) |
| --- | --- | --- | --- | --- | --- | --- | --- |
| ALFA | [AOA-8696-3ACM](https://www.alfa.com.tw/products/aoa-8696-3acm) | 3 | Omni | 600mm (L) x 20mm (W) | [$28.97](https://store.rokland.com/products/3-dbi-n-male-alfa-fiberglass-outdoor-antenna-bracket-mount-for-usa-eu-868-960-mhz-rak-bobcat-sensecap?srsltid=AfmBOoqnaHDhYku-znnVuunnKX8-50KOt0wpSsPHS-IqIgA8Jjw3lHoe) | [1.416](images/ALFA-AOA-915-5ACM.png) | ✔️ Yes |
| ALFA | [AOA-915-5ACM](https://www.alfa.com.tw/products/aoa-915-5acm?variant=36473963020360) | 5 | Omni | 182mm (L) x 20mm (W) | [$16.97](https://store.rokland.com/products/alfa-aoa-915-5acm-5-dbi-omni-outdoor-915mhz-802-11ah-mini-antenna-for-lora-halow-application) | [1.268](images/ALFA-AOA-8686-3ACM.png) | ✔️ Yes |
| Rokland | [4 dBi 698-960MHz](https://store.rokland.com/products/4-dbi-helium-hotspot-fiberglass-outdoor-antenna-bracket-mount-for-rak-bobcat-nebra-sensecap) | 4 | Omni | 342.9mm (L) x 25.4mm (W) | [$19.97](https://store.rokland.com/products/4-dbi-helium-hotspot-fiberglass-outdoor-antenna-bracket-mount-for-rak-bobcat-nebra-sensecap) | [1.509](images/ROKLAND-698-960-4DBI.png) | ✔️ Yes |
| Rokland | [5.8 dBi 915MHz](https://store.rokland.com/products/5-8-dbi-n-male-omni-outdoor-915-mhz-antenna-large-profile-32-height-for-helium-rak-miner-2-nebra-indoor-bobcat) | 5.8 | Omni | 787.4mm (L) x 25.4mm (W) | [$39.97](https://store.rokland.com/products/5-8-dbi-n-male-omni-outdoor-915-mhz-antenna-large-profile-32-height-for-helium-rak-miner-2-nebra-indoor-bobcat) | 1.25 | ✔️ Yes |

