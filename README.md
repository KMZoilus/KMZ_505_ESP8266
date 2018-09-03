# Arduino ESP8266 mini board version UPDATE v2.7
1. Fixed - ApptoUSB v3.0<br>
2. Fixed - HEN + Bin Loader<br>
3. Added - Vortex Hen + VR <br>
4. Added - BO3 Online<br>
5. Added - DB Restore v2.0 and DB Restore UNDO v2.0<br>
6. Other various tweaks and changes and updated info & description page<br><br>


# Arduino ESP8266 mini board version UPDATE v2.6
1. Updated - AppToUSB to v3<br><br>
2. Updated - DB & SG (database & save game back up) to v3<br><br>


# Arduino ESP8266 mini board version UPDATE v2.5
1. Updated the Hen in Mira + Hen to Vortex's v1.7<br><br>
2. Added - Hen + Loader. This will load Vortex Hen v1.7 plus the bin/payload loader at the same time! <br>
   This works GREAT with TylerModz Trainer. Just start the trainer on your pc, run this Hen+loader, then <br>
   inject any payload you want. This will also work to inject mod menus, just run this and then inject the <br>
   menu/payload.  This also takes the place of "original" and the PS4 Cheater.<br>
   If using tylerMods trainer make sure its v.1.3.41.57 or higher<br><br>
3. Removed the PS4 Cheater from exploit. It was the same thing as "Original" and as Bin/Payload loader, now<br>
   that Hen+Loader has been added there is no need to have a bin/payload loader 3 times on the same exploit. <br><br>
4. Other minor changes/tweaks here and there.<br><br>


# Arduino ESP8266 mini board version UPDATE v2.4
KM.Z ESP8266 Exploit Playground<br>

Note:
SSID= PS4_KMZ_ESP <br>
Password= password


1. Added Vortex HEN v1.7<br>
2. Other minor tweaks here and there<br><br>


# Arduino ESP8266 mini board version UPDATE v2.3
KM.Z ESP8266 Exploit Playground<br>

Note:
SSID= PS4_KMZ_ESP <br>
Password= password


1. Removed the Linux exploit, as most don't use it!<br>
2. Added History blocker / UNblocker - read the info & description section in the exploit
to find out more on what this does<br>

3. Some minor changes to the layout and a couple of other minor stuff here and there.<br><br>


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

<br>

# Set up instructions -  (nodeMCU pyFlasher 3.0)

1. Download latest from here: https://github.com/marcelstoer/nodemcu-pyflasher/releases<br>

2. Install, then Run<br> 

3. Plug in your ESP board. You can hold down flash button as you plug it in but its not needed with this program<br>

4. Choose correct com port, browse location for wherever you put the "bin" files you download from here and select.
 <b>Firmware_only.bin</b> is just the admin firmware, after installing you can log in and via browser on your device upload
 any files (self host) you want.
 <b>Complete.bin</b> installs the firmware AND the KM.Z Exploit (you can always delete the files later and or add to them)<br>

5. Set baud rate to: 115200, Flashmode to: Dual I/O (DIO), and "yes, wipe all data", then press "flash nodeMCU"
this ONLY flashes the main firmware/sketch to the ESP. When its done it will say so. unplug the ESP then plug it to any powered usb source (even the ps4), after plugging it in, press and hold "reset" on the esp for like 3 seconds, let go and wait a few seconds.<br> 

6. Use any wifi device with browser , log into the ESP using credentials at top of this page, then in device's browser type:  "http://10.1.1.1/admin.html"  without quotes, you should see the admin page of the ESP. 

7. If you uploaded the "complete.bin" go to "main page" and the exploit should load. If you only did firmware, then it will have a plain payloads page loaded until you up load proper files using the file manager.
<br><br>

# how to use once fully flashed

<br>

1. Plug ESP to ANY usb power sorce (doesn't have to be PS4), go to network, set up internet connect, custom, PS4_KMZ_ESP, password is <b>password</b> , set everything to automatic. Done, go to user guide and the 5.05 exploit's playground main index page should open if you used the "complete.bin" or if you've upload your own self host files proper.

2. After you run Vortex HEN once, your browser will be permanently enabled. I also suggest you run  "update blocker". At this point you should reboot ps4. <br>

If after reboot you don't see browser on home screen, go to the "library" section of the ps4 on main screen all the way to the right, look for the browser and start it, close it , it should now be on your home screen from now on.<br>

Also to access the exploit once browser is enabled, just type http://10.1.1.1 (or ANY address) and the browser will always default
to your ESP Exploit index page. Of course this is only when the ps4 is connected to the esp via WIFI. You can now bookmark that page<br>

whenever you run the admin option from the ps4 many options will not function and just kick back errors BUT you can change the 
"config editor" from the ps4, changes will happen immediately though! <br>

you can access the "admin" of your ESP from any browser as long as that device is connected via wifi to the ESP. You can type 10.1.1.1/admin.html or just 10.1.1.1 (or ANY site) on the browser then pick the Admin panel from the exploit. <br>

When on the PS4 if you are running ADMIN I would suggest BEFORE you run a payload or exploit , that you do it from the MAIN Exploit's Playground Index page  and NOT from the Admin's "main page" located in the little upper left window. Exploits should still work fine
but it may cause less of a problem that way. <br>

for more info on exploit go to:  https://www.psxhax.com/threads/ps4-internal-webserver-project-for-esp8266-d1-mini-by-stooged.5740/
<br>

Many thanks to ALL devs involved in all PS4 projects and Stooged and KiiWii in particular! 
