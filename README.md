# DumbTesla
How to turn your Tesla dumb, disable tracking and take back your privacy. 

This project originally was inspired by techlore who was complaining about tesla privacy and data collection in this video https://invidio.us/watch?v=uJuWT_wekaI
so i took it apon myself to do research on how to disable tracking in tesla and features the car provides. It took more than a month to break ground on this project DumbTesla which is focused at turning your car "dumb" as the repository name suggests. Initially in the beginning of the project i was able to collect the domains tesla sends data through which i will link in this repository for others to continue that research. I was able to collect them very simply by running the tesla through a pi hole. If you don't run a pi hole on your network i highly suggest you do https://pi-hole.net/. Once i collected the domains that was the easy part, the hard part was getting a hotspot to run the domains through a custom host file. Initially i was able to disable tracking on the tesla but only using a home wifi never with a hotspot as everytime i used a hotspot it would give a error saying "failed to identify DHCP server" i even tried using a custom nodeMCU board that i had loaded a fake probe hotspot which gave me the same error. Until today when i broke ground on how to use a hotspot while disabling all wifi capabilies. 

Requirements - 
A iPhone running a jailbreak and access to cydia
Currently there are 2 jailbreak tools avaiable for iOS https://unc0ver.dev/ and https://checkra.in/ i personally use checkra1n as it's unpatchable.
