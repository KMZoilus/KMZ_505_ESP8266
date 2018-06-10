# Arduino ESP8266 mini board version UPDATE v2.0
KM.Z ESP8266 Exploit Playground<br>

Note:
SSID= PS4_KMZ_ESP <br>
Password= password


1. Completely changed sketch. Modded version of Stooges combined with mine.
Now there is no need for any changes in ps4's network set up! Just login and 
go!<br><br>

2. ESP8266 Board specs can now be display, how much space you're using, how much is left, etc.<br><br>

3. Files can now be upload, download, deleted to/from the ESP even while connected
to the PS4, via a device with a browser, like PC, phone etc , thanks to the built in file manager!<br><br>

4. Configure wifi settings of ESP8266 right from the ps4 or via phone, pc etc<br><br>

5. Can work through USER GUIDE and/or browser either way or both!<br><br>

6. ALL addresses put in browser url lead to the INDEX page of the exploit! Unless
they are EXPLOIT specific pages!<br><br>

7. various minor changes here and there<br><br>

<b>ADDED:</b><br>
+ Admin panel to the main exploit/index page as a secondary way to access the ADMIN page.<br>
now it can be access via a browser on a device connected to the ESP or directly from the exploit.
(note: that some options on the ADMIN page will NOT work through the ps4 browser. Must use PC, Phone<br>
etc.  for those options to work)<br><br>

# Set up instructions - Method 1 (ESP tool v2.3)

1. UNzip the ESP Tool v2.3 file<br>

2. open ESP DL Tool v2.3 (run as admin)<br><br>

3.. Put a check mark in the first two boxes under "download path config" leave all others unchecked.  Then click on the 3 dots to the right of the first checked mark box and select KMZ 505 MAIN.bin (name might be a little different but will have the word MAIN in it. Now change the ADDR box to   0x000000 <br><br>

4. Go to the second checked mark box , click on the 3 dots to the right and choose the KMZ 505 FILES.bin (again, name might be a little different but will be a FILES.bin) from wherever you put it. To the right next to ADDR, in that box put   0x100000 <br>

Leave all other ADDR boxes as is (and all others unchecked)<br><br>

5. make all of the changes to the follow in the v2.3 tool (also, see the IMAGE file and match up the settings)<br>

*CrystalFreq  = 40M<br>
*DoNotChgBin   box should be checked, the SpiAutoSet  box should not be checked<br>
*Spi Speed = 80MHz<br>
*SPI Mode = DIO<br>
*Flash Size = 4M<br>
*Com Port = (whatever com port your esp8266 board is on)<br>
*Baudrate = 115200<br><br>

8. Now click on the "START"  box .. it will take a few minutes to finish. <br>

9. When done, unplug the ESP then plug it to any powered usb source, press and hold "reset" on the esp for like 3 seconds, let go and wait a few seconds. All KMZ files/payloads should be loaded! Login using info at top of page. read the <b>how to use once flash</b>
section below.
<br>
# Set up instructions - Method 2  (nodeMCU pyFlasher 3.0)

1. Download latest from here: https://github.com/marcelstoer/nodemcu-pyflasher/releases<br>

2. Install, then Run<br> 

3. Plug in your ESP board. You can hold down flash button as you plug it in but its not needed with this program<br>

4. Choose correct com port, browse location for wherever you put the "KMZ 505 Main.bin" you download from here and select<br>

5. Set baud rate to: 115200, Flashmode to: Dual I/O (DIO), and "yes, wipe all data", then press "flash nodeMCU"
this ONLY flashes the main firmware/sketch to the ESP. When its done it will say so. unplug the ESP then plug it to any powered usb source (even the ps4), press and hold "reset" on the esp for like 3 seconds, let go and wait a few seconds.<br> 

6. Now, you will now need to use a wifi device with a browser such as phone or pc. In this device place then entire "Payload Exploit Files" from above, into it.<br>

7. IN the device's browser type:  "http://10.1.1.1/admin.html"  without quotes, you should see the admin page of the ESP, select "file uploader" , navigate to the "Payload Exploit Files" folder you downloaded from here, highlight ALL files and upload them. 

6. when done, All KMZ files/payloads should be loaded! The ESP is fully flashed! Now go down to <b>how to use once flash</b> section below.
<br><br>



