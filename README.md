# Atari 5200 AV and Power Mod
This repo contains instructions for performing composite A/V out and power supply modification to a first-generation (1982, 4-Port) Atari 5200 game console.

# This is a work in progress, please check back soon!

## Power Modification

The original 4-Port Atari 5200, released in 1982, draws its power from an adapter connected at the far end of a long and bulky coaxial cable. This site contains instructions on how to replace this cumbersome arrangement with a simple barrel jack on the back of the console.

Components Needed:
- 5.5 mm outer diameter / 2.1 mm inner diameter chassis mount power jack 
- 470 uF electrolytic capacitor 
- Atari 5200 expansion port cover plate (Optional, but pretty. 3D print one from the STL file included in this repository)
- Heat shrink tubing, rubber grommets, soldering/desoldering equipment, various lengths of wire, etc. 

## Step 1:
Disassemble the Atari 5200 and remove the motherboard from the case.  Be particularly careful when handling the smoked acrylic pieces, as they are ridiculously fragile and easy to break or scratch.

## Step 2: 
Remove the coax cable, the 4700 uF capacitor, and the inductor as shown.  If you're also planning to perform the composite A/V mod, remove the RF modulator while you have the desoldering iron warmed up.

![](images/removals.png?raw=true)
![remove_coax.png](images/remove_coax.png?raw=true "remove_coax.png")

## Step 3:

Attach the replacement 470 uF electrolytic capacitor to the same spot where the 4700 uF was connected.  Solder power leads in parallel with the capacitor as shown.  Make sure the power leads are long enough to comfortably reach out of the back of the case through the expansion port door.

![Connect-Power.png](images/Connect-Power.png?raw=true "Connect-Power.png")

If you are only performing the power mod, skip to step 9.

## Step 4: The AV Composite Out Mod

Gather the commponents needed:

- 75R, 3K3, and two 2K2 resistors
- 2N3904 Transistor
- Perfboard 
- Chassis mount RCA jacks, qty 2. 
- Heat shrink tubing, rubber grommets, soldering/desoldering equipment, various lengths of wire, etc.
- Hot glue or double stick tape  

## Step 5 
Remove R33 or simply lift one side and insulate with heat shrink tubing. 
![AV-R33.png](images/AV-R33.png?raw=true "AV-R33.png")

## Step 6: Wires for the AV Composite Mod

We'll need to connect four wires to the system board for the AV.  

### 6.1: +5V

Connect a wire for +5V as shown.  Leave enough length so you can comfortably route the wire to the former location of the RF modulator.  

![AV-5volts.jpg](images/AV-5volts.jpg?raw=true "AV-5volts.jpg")

### 6.2 Ground

Connect a wire for Ground as shown.  Leave enough length so you can comfortably route the wire to the former location of the RF modulator.  
![AV-Ground.png](images/AV-Ground.png?raw=true "AV-Ground.png")

### 6.3 Video

Connect a wire for the Video input to the left of inductor L12 as shown.  Leave enough length so you can comfortably route the wire to the former location of the RF modulator.  
![AV-Video.png](images/AV-Video.png?raw=true "AV-Video.png")

### 6.4 Audio:
Connect a wire for the Audio input to the top of resistor R50 as shown. Leave enough length so you can comfortably route the wire to the former location of the RF modulator.  
![AV-Audio.png](images/AV-Audio.png?raw=true "AV-Audio.png")

This lead will run under the RF shield after reassembly, so protect it with a piece of heat shrink as shown. 

![Protect-Wires-under-Shield.png](images/Protect-Wires-under-Shield.png?raw=true "Protect-Wires-under-Shield.png")

Solder a 2K2 resistor in-line with the audio lead and insulate with heat shrink tubing.  This step isn't absolutely necessary, but I found that the audio sounds cleaner with an inline resistor.

![AV-Audio-inline-resistor.png](images/AV-Audio-inline-resistor.png?raw=true "AV-Audio-inline-resistor.png")

## Step 7:  Build the Video Amplifier

Build the transistor amplifier onto perfboard as shown. 

![AV_Amplifier.png](images/AV_Amplifier.png?raw=true "AV_Amplifier.png")

## Step 8: Attach Input and Output Leads 

Attach the +5V, Ground, and Video In wires to the amplifer circuit.  Attach a lead to the emitter of the transistor as shown for video out, and a second lead to the ground point on the amplifier circuit to ground the A/V out jacks.  These leads should be long enough so they can comfortably reach the expansion port. Attach the amplifier board to the motherboard in the former location of the RF modulator using hot glue, double stick tape, or another insulating adhesive. 

![](images/Amp-Perfboard.png?raw=true)

## Step 9: Run the cables 

Drill a hole in the RF shield near the expansion port and run the wires as shown.  Add a rubber grommet to protect the wires from the sharp edges of the sheet metal.

![Cable-Management-01.png](images/Cable-Management-01.png?raw=true "Cable-Management-01.png")

Attach the chassis mount barrel jack to the expansion port cover plate and solder the wires.  The original Atari 5200 power supply is positive center, so solder the power leads accordingly. 

## Step 10: Connect the jacks and install the cover plate 

Install the chassis mount RCA jacks in the expansion port cover, and then solder the audio, video, and ground leads to the jacks. Remove and store the original expansion port cover, then snap the new expansion port cover into the opening.  Depending on the tolerances of your 3D printer, you may want to secure the cover in place with a few squirts of hot glue to prevent it snapping out of place when cables are inserted and removed into the AV and power jacks.

![Plate_Wired.jpg](images/Plate_Wired.jpg?raw=true "Plate_Wired.jpg")
![](images/Expansion-Port-Cover-01.png?raw=true)

## Step 10:  Reassemble 

Reassemble the console, being careful to not damage the audio wire when the RF shield is reinstalled.  

## Step 11:  Enjoy

Enjoy playing Dig Dug, marveling at your crystal-clear video!

