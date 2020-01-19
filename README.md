# WECG DMR Codeplug for Anytone D-878UV
Modified from [@AG7GN](https://www.github.com/AG7GN)'s D-868UV codeplug for use with the D-878 and added analog and digital APRS functionality. Codeplug contains the PNW repeater network frequencies/zones along with other various Brandmeister repeaters in Northwest Washington and the WECG frequency list for Whatcom County. 

This codeplug was created using the Anytone D-878UV Customer Programming Software (CPS) version 1.16. It can be downloaded from [Bridgecom Systems](https://www.bridgecomsystems.com/pages/anytone-at-d878uv-support-page). 

**Anytone D-868 Users:** Steve, AG7GN, has compiled detailed instructions on how to use this 878 codeplug with the 868, while retaining your personal settings, by making use of the Data Conversion File (DCF). Check it out on his [README.md.](https://github.com/AG7GN/DMR/blob/master/README.md) 

# Change log
### 1-17-20
* Updated to 1.16 CPS
* Changed Ferndale to Sehome in Zone 1 
* Added an APRS direct channel for monitoring
* Added an empty travel zone for users to easily drop TGs to when traveling
* Alphabetized TG order in CPS
* Removed Emcomm1 & Emcomm2 PNW TGs from codeplug
* Removed PS1 and PS2 PNW TGs from codeplug
* Added missing ValleyCamp 3100 & TAC310 channels
* **---HOTSPOT USERS--- Important Change:** Changed single-slot frequencies to 430.425 and dual-slot frequencies to 430.450/439.450 in order to be compliant with WWARA suggestions
* Added roaming zone and channels for BM network repeaters in WA/ID
* Added Whatcom County DMR users to TG list
* Added Santa Barbara TG 31073 (request)
* Updated scan lists to be more useful with slow scan rate. Now only dispatch channels for public service and frequently used repeaters for Whatcom area.
* Added some SMS "Quick Texts"


### 11-10-19
* Updated digital contact list
* Fixed Parrot TG in BM Zones 
* Reordered and renumbered zones
* Deleted Whatcom Ham zone (duplicates of WECG zone)
* Added BC repeaters zone
* Deleted Analog Data zone
* Reordered channels in BM zones
* Activated APRS transmit after PTT in analog APRS zone
* Fixed DMR APRS TG issues
* Changed PTT tone to Motorola type
### 9-29-19
* Updated digital contact list
* Disabled auto startup channels
* Changed WASH EMCOMM and WASH TAC channel names to WA ARES and ARES TAC respectively to match the actual Brandmeister TG names
* Added TG 70, WA ARES Cluster
* Added ARES Cluster channel to Ferndale, Digital APRS, Pt Angeles, Sequim, Bremerton, and Sehome zones
* Opened SAR freqs
* Turned off custom stby background picture by default
* Callsign color to orange, channel name to yellow
* Removed PNW Local 2 channels from BM zones
* Changed the order of channels in BM zones
### 8-23-19
* Updated digital contact list
* Pointed Lookout U and V (B'ham) Parrot channels to the correct TG
* Changed template DMR ID to a default 13153958
### 7-31-19 (Changes from AG7GN D-868 Codeplug)
* Imported and saved with D-878 CPS
* Updated Digital Contact List
* Changed PNW parrot TG to 9998
* Changed WCSO ACS zone to WECG, listing channels in same order as WECG freq list
* Added zones/channels for Bremerton, Port Angeles, Sequim, and Sehome BM repeaters
* Added zone/channels for Analog APRS, with 14 frequently used local Whatcom repeaters plus VHF Calling Freq
* Added zone/channels for Digital APRS, with WASH EMCOMM, WASH 1, WASH TAC, and Local 2, all through NC7Q Ferndale repeater
* Added analog APRS functionality through the menus

# Known Issues
* If you use APRS and notice that your location as shown in aprs.fi is wrong (in Mongolia), the APRS settings in the radio got messed up and the radio is beaconing a fixed location. For unknown reasons, this happens sometimes after updating the codeplug despite following the instructions for setting up the CPS correctly for APRS. To fix: in the radio, press Menu->APRS->Upload Beacon->GPS Beacon. 
* Some newer radios get a "Band Error" when trying to write this codeplug to the radio. Bridgecom has created a [video](https://www.youtube.com/watch?v=yj-AoN1ofGc) explaning this error and how to fix it. More information about the error is on their [878 Support Page](https://www.bridgecomsystems.com/pages/anytone-at-d878uv-support-page).

# Setup Instructions
* **New to DMR? Important:** Obtain a DMR ID by registering on [Radioid.net](https://radioid.net/register). You may do this before you get the radio.
* Download the **<Date> AT-D878 WECG Codeplug.rdt** file from this website. **AT-D868 users:** instead, download the <Date> AT-D878 WECG Template.dcf file. 
* Download the current Customer Programming Software (CPS) version. Scroll in the [Bridgecomm Systems](https://www.bridgecomsystems.com/pages/anytone-at-d878uv-support-page) website and click  the **AT-D878UV CPS, Firmware, and Driver Update 1.16** link which will save as a zip file named **D878UV_V1.16_Official_release**. Extract all, and then run the **D878UV_Setup_1.16.exe** file inside the **D878UV V1.16CPS** folder. At the end of the installation, launch the **D878UV** program. This is the Customer Programming Software (CPS).
* In the CPS, click **File -> Open...** and then locate and double-click **<Date> AT-D878 WECG Template.rdt** (.dcf for 868 users).
* On the left-hand side of the window, click the **+** next to **Digital** to drop down the list, and click **Radio ID List**. Double-click the **13153958** and when the pop-up appears, change the **13153958** to your DMR ID, and **ChangeMe** to your call sign. Click **Ok**.
* If you wish to enable APRS functionality, in the menu bar click **Tool -> Options** and then check **GPS** and **APRS**. Click **Ok**. Double-click **APRS** on the left-hand side of the window, and change **Your Callsign** from **CHANGE** to your callsign. You may also change your SSID in this menu, although -7 is standard for a HT. 
**NOTE:** In this template, analog APRS is enabled by switching to the **Analog APRS** zone. While in this zone, each channel will beacon your GPS location to 144.39 MHz every 120 seconds. You will see a screen pop-up on the radio when the beacon data is being sent.  **_IMPORTANT: Only use the APRS zones when you wish to actively use APRS._** If you have no reason to be beaconing your position (i.e. sitting in your house monitoring all day), you may inadvertently be saturating the APRS frequency. However, the APRS zone may prove to be very useful when used as intended. For example, you may be monitoring the Mt Constitution VHF Repeater channel in the Analog APRS zone on the A side while monitoring the Lookout Mtn Repeater WASH 1 DMR talkgroup on the B side while hiking in the woods, and your GPS track will be transmitted to the APRS frequency in the background, digipeated, and then uploaded to the internet through iGates.
* **Optional (but recommended):** Update the digital contact list. This will ensure that your radio will display the name and location of anybody it receives by digital voice, even if they are new users. [Click here](https://radioid.net/database/dumps) and download **user.csv**. Go back to the CPS and in the mendu click **Tool -> Import** and then click the **Digital Contact List** button. Locate and select **user.csv** and click **Open** and then **Import**. 
* Save your codeplug to a location of your choice by clicking **File -> Save As...**.
* Set the Comm Port. Plug the radio in to the computer using the data cable, and turn on the radio. In the CPS menu bar, click **Set -> Set COM**. When the window pops up, select the correct comm port. If you don't know which port is correct, you can close the window, unplug the cable, and re-open **Set COM** to see which port disappeared. 
* Upload to radio. In the menu bar, click **Program -> Write to radio**. Click **Ok** and then check both boxes **Digital Contact List** and **Other Data**. Click **Ok** and wait for the data to be written to the radio. Don't turn off or unplug the radio during this step. It may take several minutes, as the digital contact list contains tens of thousands of contacts. 

* You may update the firmware to your radio by locating the **D878UV_V1.16_Official_release** folder you downloaded and extracted in the third step. Open the folder, and then open **A READ FIRST - Update Instructions** folder, and then open **Firmware Update Instructions.pdf** and follow the instructions to update your firmware.

# Button Layout
* P1 short press: Cycle through digital monitor settings (OFF/Current Time slot/Both Time slots)
* P1 long press: Toggle scan mode on/off
* P2 short press: Toggle between main and subchannels
* P2 long press: Toggle subchannel display on/off
* PF1 (below PTT switch) short press: Cycle through power settings (Low, Medium, High, Turbo)
* PF1 long press: Toggle between VFO and memory mode
* PF2 (below PF1): Analog monitor mode (as long as button is depressed)
* PF3 (orange/blue* button) short press: Scan channel lockout (only works in scan mode)
* PF3 long press: Toggle recorder on/off
