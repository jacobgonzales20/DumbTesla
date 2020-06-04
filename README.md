# DumbTesla
How to turn your Tesla dumb, disable tracking and take back your privacy. 

This project originally was inspired by Techlore who was complaining about Tesla privacy and data collection in this video https://invidio.us/watch?v=uJuWT_wekaI
so i took it upon myself to do research on how to disable tracking in Tesla and features the car provides. It took more than a month to break ground on this project DumbTesla which is focused at turning your car "dumb" as the repository name suggests. Initially in the beginning of the project i was able to collect the domains Tesla sends data through which i will link in this repository for others to continue that research. I was able to collect them very simply by running the Tesla through a pi hole. If you don't run a pi hole on your network i highly suggest you do https://pi-hole.net/. Once i collected the domains that was the easy part, the hard part was getting a hotspot to run the domains through a custom host file. Initially i was able to disable tracking on the tesla but only using a home wifi never with a hotspot as everytime i used a hotspot it would give a error saying "failed to identify DHCP server" i even tried using a custom nodeMCU board that i had loaded a fake probe hotspot which gave me the same error. Until today when i broke ground on how to use a hotspot while disabling all WiFi capabilities. The only problem is the method i found disabled ALL WiFi capabilities meaning no streaming, netflix, youtube, navigation basically only radio as that is not WiFi. I'm hoping i can find a way to individually block domains in the future. 

Requirements - 
A iPhone running a jailbreak and access to cydia, Currently there are 2 jailbreak tools available for iOS https://unc0ver.dev/ and https://checkra.in/ i personally use checkra1n as it's unpatchable.

Installation -
1. You need to be jailbroken and have cydia installed
2. You need to add the current repo in cydia https://repo.packix.com/
3. You will need $1.50 as the tweak is paid sadly but #supportjailbreakdevs
4. You will need to purchase the tweak called Harpy (Which allows you to block individual clients on a hotspot network or wifi)
5. Once Harpy is installed launch your phones hotspot
6. Open Harpy and navigation to the hotspot tab their should be some numbers including a ip and mac address
7. Press once on the numbers and click attempt to block device this will block all data from the device while keeping a established connection

And you are done congrats you can even use when you drive!
A video coming soon on how to do this whole tutorial

A personal request for people wanting to use this in a video or article or sharing it in general please give me credit i don't mind you sharing but just please the proper credit thanks!
