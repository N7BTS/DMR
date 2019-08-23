# WECG DMR Codeplug for Anytone D-878UV
Modified from [@AG7GN](https://www.github.com/AG7GN)'s D-868UV codeplug for use with the D-878 and added analog and digital APRS functionality. Codeplug contains the PNW repeater network frequencies/zones along with other various Brandmeister repeaters in Northwest Washington and the WECG frequency list for Whatcom County. 

This codeplug was created using the Anytone D-878UV Codeplug Software (CPS) version 1.13. It can be downloaded from [Bridgecom Systems](https://www.bridgecomsystems.com/pages/anytone-at-d878uv-support-page). It should be compatible with the D-868UV radio and the D-868UV CPS, except for the APRS features. 

# Change log
### 7-31-19 (Changes from AG7GN D-868 Codeplug)
* Imported and saved with D-878 CPS
* Updated Digital Contact List
* Changed PNW parrot TG to 9998
* Changed WCSO ACS zone to WECG, listing channels in same order as WECG freq list
* Added zones/channels for Bremerton, Port Angeles, Sequim, and Sehome BM repeaters
* Added zone/channels for Analog APRS, with 14 frequently used local Whatcom repeaters plus VHF Calling Freq
* Added zone/channels for Digital APRS, with WASH EMCOMM, WASH 1, WASH TAC, and Local 2, all through NC7Q Ferndale repeater
* Added analog APRS functionality through the menus
### 8-23-19
* Updated digital contact list
* Pointed Lookout U and V (B'ham) Parrot channels to the correct TG
* Changed template DMR ID to a default 13153958

# Known Issues
* Some newer radios get a "Band Error" when trying to write this codeplug to the radio. Bridgecom has created a [video](https://www.youtube.com/watch?v=yj-AoN1ofGc) explaning this error and how to fix it. More information about the error is on their [878 Support Page](https://www.bridgecomsystems.com/pages/anytone-at-d878uv-support-page).

# I just got a new Anytone D-878 radio... now what?
* **Important:** Obtain a DMR ID by registering on [Radioid.net](https://radioid.net/register). You may do this before you get the radio.
* Download the **<Date> AT-D878 WECG Template.rdt** file from this website. 
* Download the CPS software. Scroll to the bottom of the [Bridgecomm Systems](https://www.bridgecomsystems.com/pages/anytone-at-d878uv-support-page) website and click  the **AT-D878UV CPS, Firmware, and Driver Update 1.13** link which will save as a zip file named **D878UV_V1.13_Official_release**. Extract all, and then run the **D878UV_Setup_1.13c.exe** file inside the **D878UV CPS V1.13 Update File** folder. At the end of the installation, launch the **D878UV** program. This is the Codeplug Software (CPS).
* In the CPS, click **File -> Open...** and then locate and double-click **<Date> AT-D878 WECG Template.rdt**. 
* On the left-hand side of the window, click the **+** next to **Digital** to drop down the list, and click **Radio ID List**. Double-click the **13153958** and when the pop-up appears, change the **13153958** to your DMR ID, and **ChangeMe** to your call sign. Click **Ok**.
* If you wish to enable APRS functionality, in the menu bar click **Tool -> Options** and then check **GPS** and **APRS**. Click **Ok**. Double-click **APRS** on the left-hand side of the window, and change **Your Callsign** from **CHANGE** to your callsign. You may also change your SSID in this menu, although -7 is standard for a HT. 
**NOTE:** In this template, analog APRS is enabled by switching to the **Analog APRS** zone. While in this zone, each channel will beacon your GPS location to 144.39 MHz every 120 seconds. You will see a screen pop-up on the radio when the beacon data is being sent.  **_IMPORTANT: Only use the APRS zones when you wish to actively use APRS._** If you have no reason to be beaconing your position (i.e. sitting in your house monitoring all day), you may inadvertently be saturating the APRS frequency. However, the APRS zone may prove to be very useful when used as intended. For example, you may be monitoring the Mt Constitution VHF Repeater channel in the Analog APRS zone on the A side while monitoring the Lookout Mtn Repeater WASH 1 DMR talkgroup on the B side while hiking in the woods, and your GPS track will be transmitted to the APRS frequency in the background, digipeated, and then uploaded to the internet through iGates.
* **Optional (but recommended):** Update the digital contact list. This will ensure that your radio will display the name and location of anybody it receives by digital voice, even if they are new users. [Click here](https://radioid.net/database/dumps) and download **user.csv**. Go back to the CPS and in the mendu click **Tool -> Import** and then click the **Digital Contact List** button. Locate and select **user.csv** and click **Open** and then **Import**. 
* Save your codeplug to a location of your choice by clicking **File -> Save As...**.
* Set the Comm Port. Plug the radio in to the computer using the data cable, and turn on the radio. In the CPS menu bar, click **Set -> Set COM**. When the window pops up, select the correct comm port. If you don't know which port is correct, you can close the window, unplug the cable, and re-open **Set COM** to see which port disappeared. 
* Upload to radio. In the menu bar, click **Program -> Write to radio**. Click **Ok** and then check both boxes **Digital Contact List** and **Other Data**. Click **Ok** and wait for the data to be written to the radio. Don't turn off or unplug the radio during this step. It may take several minutes, as the digital contact list contains tens of thousands of contacts. 

* If required, you may update the firmware to your radio by locating the **D878UV_V1.13_Official_release** folder you downloaded and extracted in the third step. Open the folder, and then open **A READ FIRST - Update Instructions** folder, and then open **Firmware Update Instructions.pdf** and follow the instructions to update your firmware.
