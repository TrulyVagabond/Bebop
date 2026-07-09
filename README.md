# An RF Carrier Board for Raspberry Pi 5 Inspired by Cowboy Bebop

## Whats Different about this Carrier Board?:

Well Because It's made by me, It's an RF Carrier Board, a custom designed Printed Circuit Board (PCB) that acts as a Multi-Band Radio Sheild for Raspberry Pi. Basically A Weapon when there's no internet. This Circuit Board Contains Modules Which are Widely used by Cybersecurity Professionals and Hobbiest. This Board is Engineered to Consolidate Three Distinct Modules such as:

- **NRF24L01+PA+LNA**
- **CC1101** 
- **LoRa RFM95W**

Because RF modules are sensitive to voltage drops and spikes, I have added a Power Regulator **AMS1117**. Which Receives the Power from the 5V Pin and converts it to a smooth 3.3V for the modules. In addition I have also added a ceramic bypass capacitor array.

It just Pops onto the Raspberry Pi GPIO pins and you're good to go. (You do Have to solder the Female Headers and the Modules on the Carrier Board. Follow the Instructions Below to Make this Board.)

## Steps To Reproduce:

- Grab the Gerber.zip File from the repo and Upload it to your Choice of PCB manufacturer.
- You can Either Solder the SMD components like AMS1117 and the Capacitors Yourself or have a manufacturer assemble it for you.
- Once the Board arrives, grab the 2x20 Female Header and solder it to the bottom of the board (not on the side of logos etc). 
- Solder Standard Female Headers for the Radio Modules such as **NRF24L01**, **CC1101** and **LoRa RFM95W**. then Plug the Modules in its Specific Place.
- Plug into the Raspberry Pi 5 and use a multimeter to verify if 3.3V is successfully reaching the VCC pins of the Radio Modules

 *All the Files can be found in the Repository in it's specific Folders.*

## SAFETY NOTES:

- The Raspberry Pi 5 is very power-hungry and can draw up to 5A (27W) under heavy load. Ensure you are using the official 27W USB-C power supply so the Pi does not throttle when the radio modules pull transmission current.
- Ensure that the Case isn't Air-tight and allows Air-Flow.
- This board supports **Sub-1GHz** and **2.4GHz** transmission. Always ensure you are operating within the legal ISM (Industrial, Scientific, and Medical) radio bands for your specific country.