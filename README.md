# Atari 5200 AV and Power Mod
This repo contains instructions for performing composite A/V out and power supply modification to a first-generation (1982, 4-Port) Atari 5200 game console.

# This is a work in progress, please check back soon!

## Power Modification

The original 4-Port Atari 5200, released in 1982, draws its power from an adapter connected at the far end of a long and bulky coaxial cable. This site contains instructions on how to replace this cumbersome arrangement with a simple barrel jack on the back of the console.

Components Needed:
- 5.5 mm outer diameter / 2.1 mm inner diameter chassis mount power jack 
- 470 \muF electrolytic capacitor 
- Atari 5200 expansion port cover plate (STL file included in this repository)

## Step 1:
Disassemble the Atari 5200 and remove the motherboard from the case.  Be particularly careful when handling the smoked acrylic pieces, as they are ridiculously fragile and easy to break or scratch.

## Step 2: 
Remove the coax cable, the 4700 \muF capacitor, and the coil as shown.  If you're also planning to perform the composite A/V mod, remove the RF modulator while you have the desoldering iron warmed up.

![removals.png](images/removals.png?raw=true "removals.png")
![remove_coax.png](images/remove_coax.png?raw=true "remove_coax.png")

## Step 3:

Attach the replacement 470 \muF electrolytic capacitor to the same spot where the 4700 \muF was connected.  Attach power leads to the spare connectors as shown.
![Connect-Power.png](images/Connect-Power.png?raw=true "Connect-Power.png")


![AV-5volts.jpg](images/AV-5volts.jpg?raw=true "AV-5volts.jpg")
![AV-Audio-inline-resistor.png](images/AV-Audio-inline-resistor.png?raw=true "AV-Audio-inline-resistor.png")
![AV-Audio.png](images/AV-Audio.png?raw=true "AV-Audio.png")
![AV-Ground.png](images/AV-Ground.png?raw=true "AV-Ground.png")
![AV-R33.png](images/AV-R33.png?raw=true "AV-R33.png")
![AV_Amplifier.png](images/AV_Amplifier.png?raw=true "AV_Amplifier.png")
![Amp-Perfboard.png](images/Amp-Perfboard.png?raw=true "Amp-Perfboard.png")
![Cable-Management-01.png](images/Cable-Management-01.png?raw=true "Cable-Management-01.png")
![Expansion-Port-Cover-01.png](images/Expansion-Port-Cover-01.png?raw=true "Expansion-Port-Cover-01.png")
![Protect-Wires-under-Shield.png](images/Protect-Wires-under-Shield.png?raw=true "Protect-Wires-under-Shield.png")

