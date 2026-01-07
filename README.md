# T-Embed CC1101 Plus — External Antenna Mod

This repo documents a hardware modification for the LilyGo T-Embed CC1101 Plus to replace the stock internal antennas with high‑gain external antennas. The mod improves signal strength and allows easy antenna swapping for different use cases.

## 📸 Finished mod

<p align="center">
  <img src="./images/top-view.jpg" alt="Top profile showing custom mounting points" width="640" />
</p>

*Figure 1 — Top profile showing the custom mounting points.*

<p align="center">
  <img src="./images/front-view.jpg" alt="Front profile of the finished mod" width="640" />
</p>

*Figure 2 — Front profile of the finished mod.*

<p align="center">
  <img src="./images/internal-view.jpg" alt="Internal view after disassembly" width="640" />
</p>

*Figure 3 — Internal view after disassembly.*

## 🛠 Hardware required

- LilyGo T-Embed CC1101 Plus (LoRa version)
- 2 × 2.4 GHz high-gain antennas (Wi‑Fi / BT)
  - Example: [Amazon link](https://a.co/d/5IQl2xi)
- 1 × 915 MHz high-gain antenna (LoRa / Meshtastic)
  - Example: [Amazon link](https://a.co/d/8Ta44NI)
- 3 × U.FL to SMA female pigtails (short length ≈ 5–10 cm)
- Nuts, washers, and basic tools (drill, small driver)

## ⚙️ Installation

1. Disassembly  
   - Remove rear cover screws and carefully unplug battery wires and the FPC ribbon for the screen/dial.

2. Case modification  
   - Mark three evenly spaced holes on the top rim.  
   - Drill holes sized for the SMA connector barrels (≈ 6 mm / 1/4").  
   - Verify clearance so connector barrels won't press on the PCB.

3. Wiring  
   - LoRa (915 MHz): attach a pigtail to the CC1101 module U.FL.  
   - Wi‑Fi / BT (2.4 GHz): attach pigtail to the ESP32 U.FL and remove the stock flex antenna.  
   - Mount SMA connectors and secure with nuts/washers.

4. Reassembly  
   - Route cables around the battery so the case closes flush, reattach the back cover, and install antennas.

## 🚀 Results

- Noticeable increase in received/transmit signal (dB gain) over stock flex antennas.  
- Flexible antenna choices (omnidirectional, high-gain, directional) for different environments.

jamiemadde-max
---

*Created by jamiemadde-max*
