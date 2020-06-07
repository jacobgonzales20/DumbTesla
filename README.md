# DumbTesla
How to turn your Tesla dumb, disable tracking and take back your privacy. 

A personal request for people wanting to use this in a video or article or sharing it in general please give me credit i don't mind you sharing but just please give the proper credit thanks!

This project originally was inspired by Techlore who was complaining about Tesla privacy and data collection in this video https://invidio.us/watch?v=uJuWT_wekaI
so i took it upon myself to do research on how to disable tracking in Tesla and features the car provides. It took more than a month to break ground on this project DumbTesla which is focused at turning your car "dumb" as the repository name suggests. Initially in the beginning of the project i was able to collect the domains Tesla sends data through which i will link in this repository for others to continue that research. I was able to collect them very simply by running the Tesla through a pi hole. If you don't run a pi hole on your network i highly suggest you do https://pi-hole.net/. Once i collected the domains that was the easy part, the hard part was getting a hotspot to run the domains through a custom host file. Initially i was able to disable tracking on the Tesla but only using a home WiFi never with a hotspot as every time i used a hotspot it would give a error saying "Failed To Identify DHCP Server" i even tried using a custom nodeMCU board that i had loaded a fake probe hotspot which gave me the same error. Until today when i broke ground on how to use a hotspot while disabling all WiFi capabilities. The only problem is the method i found disabled ALL WiFi capabilities meaning no streaming, Netflix, YouTube, navigation basically only radio works as that is not WiFi. I'm hoping i can find a way to individually block domains in the future. 

Currently both method's 1 & 2 are for iOS i hope to add a method for android but i don't have access to an android device. 

Method 1 (Disables ALL WiFi Capabilities & Can Be Used When Driving) - 

Requirements - 
A iPhone running a jailbreak and access to cydia, Currently there are 2 jailbreak tools available for iOS https://unc0ver.dev/ and https://checkra.in/ i personally use checkra1n as it's unpatchable.

Video Tutorial Method 1 - https://peertube.social/videos/watch/af411430-6164-4fd4-94b6-4dd663f5a77e

Installation -
1. You need to be jailbroken and have cydia installed
2. You need to add the current repo in cydia https://repo.packix.com/
3. You will need $1.50 as the tweak is paid sadly but #supportjailbreakdevs
4. You will need to purchase the tweak called Harpy (Which allows you to block individual clients on a hotspot network or WiFi)
5. Once Harpy is installed launch your phones hotspot
6. Connect the tesla to your phones hotspot location
7. Open Harpy and navigation to the hotspot tab their should be some numbers including a IP and mac address
8. Press once on the numbers and click attempt to block device this will block all data from the device while keeping an established connection

And you are done congrats you can even use when you drive!

Video Proof Here - https://peertube.social/videos/watch/8a5114d3-1b41-47cf-afc4-6aa7b12a1b9b

Method 2 (TESTING Disables Individual Domains & Can Be Used When Driving) - 

Requirements - 
A iPhone running a jailbreak and access to cydia, Currently there are 2 jailbreak tools available for iOS https://unc0ver.dev/ and https://checkra.in/ i personally use checkra1n as it's unpatchable.

Installation -
1. You need to be jailbroken and have cydia installed
2. You need to add the current repo in cydia http://apt.thebigboss.org/repofiles/cydia/ (Usually installed by default)
3. You will need $5 as the tweak is paid sadly but #supportjailbreakdevs
4. You will need to purchase the tweak called TetherMe (Which allows you to use a vpn with a hotspot)
5. Once TetherMe is installed launch your phones hotspot
6. Open settings and navigate to TetherMe
7. Enable Override Data Source then press "share from" and click Auto-Detect Active VPN
8. Rest of the steps will soon be posted once I find a vpn that allows custom blocks lists if you know of one please make a issue 

Note - Make sure you use TetherMe for your right iOS Version!

Credits - 
jacobgonzales20, techlore
