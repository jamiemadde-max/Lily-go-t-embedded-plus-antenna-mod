8# Lily-go-t-embedded-plus-antenna-mod
Instructions for antenna mod
# T-Embed CC1101 plus External Antenna Mod

This project documents a hardware modification for the LilyGo T-Embed CC1101 plus to replace the stock internal antennas with high-gain external antennas. This modification significantly improves signal range and stability for both LoRa/Sub-GHz (915MHz) and Wi-Fi/Bluetooth (2.4GHz) communications.

## 📸 The Finished Mod
![Front View](path/to/your/front-view.jpg)
*Front view showing the triple antenna setup.*

![Top View](path/to/your/top-view.jpg)
*Top profile showing the custom mounting points.*

## 🛠 Hardware Required

**1. The Device**
* **LilyGo T-Embed CC1101 puls** (LoRa Version)

**2. Antennas**
* **2.4GHz High Gain Antennas (Qty: 2):** Used for Wi-Fi and Bluetooth.
    * [Link to Amazon Product](https://a.co/d/5IQl2xi)
* **915MHz High Gain Antenna (Qty: 1):** Used for LoRa/Meshtastic communication.
    * [Link to Amazon Product](https://a.co/d/8Ta44NI)

**3. Internal Connectors (Crucial)**
* **U.FL to SMA Female Pigtails (Qty: 3):** These are required to connect the board's internal U.FL ports to the external antennas. *Ensure the cable length is short (approx 5-10cm) to fit inside the case.*

## ⚙️ Installation Guide

### Step 1: Disassembly
Remove the rear cover screws to access the internal components. Be careful with the battery wires and the FPC ribbon cable connecting the screen/dial.

![Internal View](path/to/your/internal-view.jpg)

### Step 2: Case Modification
1.  Mark three evenly spaced points on the top plastic rim of the T-Embed case.
2.  Drill holes sized to fit the SMA connectors (usually 6mm or 1/4").
3.  Ensure there is clearance inside the case for the connector barrels so they don't crush the PCB.

### Step 3: Wiring
1.  *lora (915MHz):** Locate the U.FL connector on the CC1101 module (the smaller daughterboard) and connect one pigtail.
2.  **Wi-Fi/BT (2.4GHz):** Locate the ESP32 U.FL connector on the main PCB. Disconnect the stock internal flex antenna and connect the new pigtail.
3.  **Mounting:** Secure the SMA connectors to the drilled holes using the nuts and washers provided with your pigtails.

### Step 4: Reassembly
Route the cables carefully around the battery to ensure the case closes flush. Screw the back cover back on and attach your antennas.

## 🚀 Results
* **Signal Strength:** Significant dB gain over stock internal FPC antennas.
* **Versatility:** Allows for swapping antennas based on use case (e.g., directional vs. omnidirectional).

---
*Created by jamiemadde-max*
