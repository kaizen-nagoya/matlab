Q1 Are there any CAN XL and Vehicle Ethernet switching IC?
A1 by ChatGPT
Yes — there are already several IC families and architectures emerging around both **CAN XL** and **Automotive Ethernet switching**, although fully integrated “CAN XL + Ethernet switch SoC” devices are still relatively rare in 2026.

## CAN XL ICs

### CAN XL Protocol Controllers / IP

The CAN XL standard is now formalized in ISO 11898-1:2024 and supports payloads up to 2048 bytes and data rates up to 20 Mbit/s. It was designed specifically to bridge the gap between CAN FD and Automotive Ethernet. ([ボッシュ自動車半導体とセンサー][1])

Key suppliers include:

* [Bosch CAN XL IP Modules](https://www.bosch-semiconductors.com/products/ip-modules/can-ip-modules/can-xl.html?utm_source=chatgpt.com)
* [NXP Semiconductors](https://www.nxp.com?utm_source=chatgpt.com)
* [Infineon Technologies](https://www.infineon.com?utm_source=chatgpt.com)
* [Renesas Electronics](https://www.renesas.com?utm_source=chatgpt.com)
* [Texas Instruments](https://www.ti.com?utm_source=chatgpt.com)
* [Microchip Technology](https://www.microchip.com?utm_source=chatgpt.com)

Typical device categories:

| Category              | Examples                       |
| --------------------- | ------------------------------ |
| CAN XL controller IP  | Bosch M_CAN XL evolution       |
| CAN XL transceiver    | Next-gen SIC XL PHYs           |
| MCU with CAN XL       | Upcoming automotive MCUs       |
| CAN XL bridge/gateway | Ethernet ↔ CAN XL gateway SoCs |

---

## Automotive Ethernet Switching ICs

This area is much more mature.

### NXP Automotive Ethernet Switches

One of the best-known automotive Ethernet switch families is the NXP SJA1105 series:

* [NXP SJA1105 Automotive Ethernet Switches](https://www.nxp.com/products/interfaces/ethernet-/automotive-ethernet-switches/sja1105pel-qel-rel-sel-series-ethernet-switches%3ASJA1105PQRS?lang=en&lang_cd=en&utm_source=chatgpt.com)

Features include:

* TSN (Time Sensitive Networking)
* AVB support
* VLAN/QoS
* 100BASE-T1 / 1000BASE-T1 connectivity
* Functional safety support
* Automotive AEC-Q100 qualification ([NXP][2])

Typical applications:

* ADAS domain controllers
* Zonal ECUs
* IVI backbones
* Camera/radar aggregation

---

### Marvell Automotive Ethernet Switch ICs

[Marvell Automotive Networking Solutions](https://www.marvell.com/automotive/?utm_source=chatgpt.com)

Marvell has many automotive Ethernet switch families:

* 88Q50xx
* Brightlane series
* Multi-gig TSN switches

Older industrial/embedded switch ICs include:

* 88E6097
* 88E6352
* 88E1548

Examples from the search:

* ([ETEI][3])

---

## Are There Integrated CAN XL + Ethernet Switch ICs?

### Short answer:

Not commonly as a single monolithic chip yet.

Current industry trend is:

```text
CAN XL subnet
        │
CAN XL controller/transceiver
        │
Gateway MCU / MPU
        │
Automotive Ethernet switch
        │
Zonal / backbone Ethernet
```

This architecture is becoming common in:

* SDV (Software Defined Vehicle)
* Zonal E/E architectures
* HPC/domain controller systems

---

## Emerging Gateway / Zonal Processor Vendors

The following companies are actively developing mixed CAN XL + Ethernet architectures:

| Vendor                                                                   | Focus                     |
| ------------------------------------------------------------------------ | ------------------------- |
| [NXP Semiconductors](https://www.nxp.com?utm_source=chatgpt.com)         | S32G zonal processors     |
| [Infineon Technologies](https://www.infineon.com?utm_source=chatgpt.com) | AURIX + Ethernet          |
| [Renesas Electronics](https://www.renesas.com?utm_source=chatgpt.com)    | R-Car / RH850             |
| [Texas Instruments](https://www.ti.com?utm_source=chatgpt.com)           | Jacinto + DP83TC PHY      |
| [Microchip Technology](https://www.microchip.com?utm_source=chatgpt.com) | LAN966x TSN               |
| [Marvell Technology](https://www.marvell.com?utm_source=chatgpt.com)     | Brightlane Ethernet       |
| [Broadcom](https://www.broadcom.com?utm_source=chatgpt.com)              | Automotive switch fabrics |

---

## Architectural Direction (Very Important)

The industry trend is *not* replacing CAN with Ethernet entirely.

Instead:

| Layer                        | Best Technology          |
| ---------------------------- | ------------------------ |
| Hard real-time local control | CAN FD / CAN XL          |
| Sensor fusion backbone       | Automotive Ethernet      |
| OTA / diagnostics            | Ethernet/IP              |
| Safety island communication  | CAN XL                   |
| High-bandwidth cameras       | 1000BASE-T1 / 10GBASE-T1 |

CAN XL is especially attractive because it can transport:

* IP packets
* tunneled Ethernet frames
* mixed CAN FD / CAN XL traffic ([ボッシュ自動車半導体とセンサー][1])

---

## Interesting New Direction: CAN XL ↔ TSN Convergence

A major research area now is:

* deterministic Ethernet TSN
* CAN XL coexistence
* unified time synchronization

This is becoming critical for:

* autonomous driving
* x-by-wire
* centralized compute
* digital twin vehicle networks

The paper below is a good overview:

* [Composite CAN XL-Ethernet Networks for Next-Gen Automotive Systems](https://arxiv.org/abs/2306.09498?utm_source=chatgpt.com)

---

## Typical 2026 Vehicle Network Topology

```text
       10G Automotive Ethernet Backbone
                  │
        TSN Ethernet Switch IC
      ┌───────────┼───────────┐
      │           │           │
  Zonal ECU   ADAS ECU    Infotainment
      │
  CAN XL Gateway MCU
      │
 ┌────┼────┐
Body  Chassis  Powertrain
CAN XL / CAN FD buses
```

That hybrid topology is currently the dominant direction in next-generation automotive E/E architectures.

[1]: https://www.bosch-semiconductors.com/products/ip-modules/can-ip-modules/can-xl.html?utm_source=chatgpt.com "CAN_XL, CAN XL, CAN, Bosch_CAN, IP-modules"
[2]: https://www.nxp.com/products/interfaces/ethernet-/automotive-ethernet-switches/sja1105pel-qel-rel-sel-series-ethernet-switches%3ASJA1105PQRS?lang=en&lang_cd=en&utm_source=chatgpt.com "SJA1105PQRS | Automotive Ethernet Switches | NXP Semiconductors"
[3]: https://www.etei.com/product/88e6097fa2-lgo1i000?utm_source=chatgpt.com "88E6097FA2-LGO1I000 Marvell Tech | wholesale"
