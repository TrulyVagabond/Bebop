# An RF Carrier Board for Raspberry Pi 5 Inspired by Cowboy Bebop

<img width="409" height="397" alt="BeBop" src="https://github.com/user-attachments/assets/b748c721-9c97-46ba-820b-c94b6badc429" />

### Schematics:

<img width="1228" height="450" alt="image" src="https://github.com/user-attachments/assets/a2ea1e2c-68e6-45b3-97fc-a8bb2ff5a330" />


### In 3D:
<img width="554" height="444" alt="Complete-Bebop-3D" src="https://github.com/user-attachments/assets/713ae90c-b115-438c-8c8a-74dbf62c1529" />

## What's Different about this Carrier Board?:

Well Because It's made by me, It's an RF Carrier Board, a custom designed Printed Circuit Board (PCB) that acts as a Multi-Band Radio Sheild for Raspberry Pi. Basically A Weapon when there's no internet. This Circuit Board Contains Modules Which are Widely used by Cybersecurity Professionals and Hobbiest. This Board is Engineered to Consolidate Three Distinct Modules such as:

- **NRF24L01+PA+LNA**
- **CC1101** 
- **LoRa RFM95W**

Because RF modules are sensitive to voltage drops and spikes, I have added a Power Regulator **AMS1117**. Which Receives the Power from the 5V Pin and converts it to a smooth 3.3V for the modules. In addition I have also added a ceramic bypass capacitor array.

It just Pops onto the Raspberry Pi GPIO pins and you're good to go. (You do Have to solder the Female Headers and the Modules on the Carrier Board. Follow the Instructions Below to Make this Board.)

## Steps To Reproduce:

- Grab the Gerber.zip File from the repo and Upload it to your Choice of PCB manufacturer.

- You can Either Solder the SMD components like **AMS1117** and the Capacitors Yourself or have a manufacturer assemble it for you.
- Once the Board arrives, grab the 2x20 Female Header and solder it to the bottom of the board (not on the side of logos etc). 
- Solder Standard Female Headers for the Radio Modules such as **NRF24L01**, **CC1101** and **LoRa RFM95W**. then Plug the Modules in its Specific Place.
- Plug into the Raspberry Pi 5 and use a multimeter to verify if 3.3V is successfully reaching the VCC pins of the Radio Modules

 *All the Files can be found in the Repository in it's specific Folders.*

## SAFETY NOTES:

- The Raspberry Pi 5 is very power-hungry and can draw up to 5A (27W) under heavy load. Ensure you are using the official 27W USB-C power supply so the Pi does not throttle when the radio modules pull transmission current.

- Ensure that the Case isn't Air-tight and allows Air-Flow.
- This board supports **Sub-1GHz** and **2.4GHz** transmission. Always ensure you are operating within the legal ISM (Industrial, Scientific, and Medical) radio bands for your specific country.
<<<<<<< HEAD


## Bill of Materials (BOM)

| Component | Designator | Description | Qty | LCSC Part # | Approx Price (USD) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **AMS1117-3.3** | U2 | 3.3V 1A Linear Voltage Regulator (SOT-223) | 1 | C6186 | $0.20 |
| **22uF Capacitor** | C6 | Ceramic MLCC (1206 SMD) - Output Bulk Filter | 1 | C12891 | $0.35 |
| **10uF Capacitor** | C4 | Ceramic MLCC (0805 SMD) - Input Bulk Filter | 1 | C15850 | $0.04 |
| **100nF (0.1uF) Cap** | C2, C3 | 50V Ceramic MLCC (0805 SMD) - High-Frequency Bypass | 2 | C49678 | $0.04 |
| **100uF Capacitor** | C1 | 25V Electrolytic Capacitor (Through-Hole Bulk Filter) | 1 | C4930491 | $0.02 |
| **nRF24L01+PA+LNA** | U1 | 2.4GHz Wireless Transceiver Module with Power Amp | 1 | C9900187674 | $1.50 |
| **CC1101 Module** | 1 | Sub-1GHz Wireless Transceiver Module | 1 | *User Assigned* | $2.50 |
| **LoRa RF Module** | 2 | Long Range SX1278 RF Transceiver Module | 1 | *User Assigned* | $4.00 |
| **F-2x20 Header** | P1 | 2.54mm Pitch Female Socket (For Raspberry Pi 5 GPIO) | 1 | C50982 | $0.29 |
=======
>>>>>>> c5064316a56d8f96ddcd3f81f0e46d8e10d18d74
