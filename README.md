# DumbTesla
How to turn your Tesla dumb, disable tracking and take back your privacy. 

A personal request for people wanting to use this in a video or article or sharing it in general please give me credit i don't mind you sharing but just please give the proper credit thanks!

This project originally was inspired by Techlore who was complaining about Tesla privacy and data collection in this video https://tube.privacytools.io/videos/watch/c60165fc-db8b-4867-8489-c9fb5ab27942 so i took it upon myself to do research on how to disable tracking in Tesla and features the car provides. It took more than a month to break ground on this project DumbTesla which is focused at turning your car "dumb" as the repository name suggests. Initially in the beginning of the project i was able to collect the domains Tesla sends data through which i will link in this repository for others to continue that research. I was able to collect them very simply by running the Tesla through a pi hole. If you don't run a pi hole on your network i highly suggest you do https://pi-hole.net/. Once i collected the domains that was the easy part, the hard part was getting a hotspot to run the domains through a custom host file. Initially i was able to disable tracking on the Tesla but only using a home WiFi never with a hotspot as every time i used a hotspot it would give a error saying "Failed To Identify DHCP Server" i even tried using a custom nodeMCU board that i had loaded a fake probe hotspot which gave me the same error. Until today when i broke ground on how to use a hotspot while disabling all WiFi capabilities. The only problem is the method i found disabled ALL WiFi capabilities meaning no streaming, Netflix, YouTube, navigation basically only radio works as that is not WiFi. I'm hoping i can find a way to individually block domains in the future. 

Currently both method's 1 & 2 are for iOS i hope to add a method for android but i don't have access to an android device. 

Method 1 (Disables ALL WiFi Capabilities & Can Be Used When Driving) - 

Requirements - 
A iPhone running a jailbreak and access to cydia, Currently there are 2 jailbreak tools available for iOS https://unc0ver.dev/ and https://checkra.in/ i personally use checkra1n as it's unpatchable.

Video Tutorial Method 1 - https://diode.zone/videos/watch/1f31ad84-f700-448c-843c-4f67500630db

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

Video Proof Here - https://diode.zone/videos/watch/a668552e-8dab-41bd-a14a-48c184077952

Method 2 w/ Windscribe Temporary Fix ( Disables Individual Domains & Can Be Used When Driving)(Only Allows 3 Domains To Be Disabled On Free Plan) - 

Requirements - 
A iPhone running a jailbreak and access to cydia, Currently there are 2 jailbreak tools available for iOS https://unc0ver.dev/ and https://checkra.in/ i personally use checkra1n as it's unpatchable.

Note - Make sure you use TetherMe for your right iOS Version!

Installation -
1. You need to be jailbroken and have cydia installed
2. You need to add the current repo in cydia http://apt.thebigboss.org/repofiles/cydia/ (Usually installed by default)
3. You will need $5 as the tweak is paid sadly but #supportjailbreakdevs
4. You will need to purchase the tweak called TetherMe (Which allows you to use a vpn with a hotspot) 
5. You will then need to install TetherMe
6. You will then need to download a vpn app from the app store called windscribe
6. Once installed head over to https://temp-mail.org/ to get a temp email
7. Launch windscribe then press signup enter in fake details and use the temp email 
8. Then go back to the website https://temp-mail.org/en/ to confirm your email for windscribe
9. Then open up windscribe and install the vpn profile by pressing allow
10. Once the vpn profile is installed open windscribe and click the 3 lines at the top left
11. Then navigate to account then press edit account at the bottom 
12. Once you have been redirected to their website press My Account on the drop down menu then slide to R.O.B.E.R.T
13. Once in the R.O.B.E.R.T section click custom rules
14. In custom rules add these 3 domains telemetry-prd.vn.tesla.services, telemetry-prd.ap.tesla.services, location.teslamotors.com sadly the free plan only lets you have 3 domains so i will for sure be looking for a better method. 
15. Once you have added the 3 domains click "Apply to all connected devices immediately" at the bottom and press yes
16. Now exit the website and head back to the vpn and press enable (Top Right)
17. After it is enabled go to your settings and locate the TetherMe tweak and enable override data source
18. Make sure "Share From" is selected to "Auto-Detect Active VPN" if it isn't select what ever is selected and change it 
19. Once you have selected "Auto-Detect Active VPN" press personal hotspot and enable
20. Then connect your car to your hotspot and you are done!

You can even use when you drive!

Note - I am still looking for a alternative to windscribe that allows custom block lists so if you find one please create a issue

Video Tutorial Coming Soon!

Credits - 
jacobgonzales, greentheonly, techlore
