# WiNETH,I will take care of your miner and you can relax.
WiNETH Miner is a graphical interface to use with ethminer with advanced watchdog options and monitoring.
WinETH Miner written in Qt (C++), is a GUI with options to run ethminer under control.
Features
simple GUI that can run on Windows, Linux and Mac (Qt).
automated ethminer parameters.
watchdog for restarting ethminer in case of errors.
enhanced displaying of ethminer output - highlighted successful solutions, shares & zero hashrate
display useful information for nVidia cards - core temperatures, fan speed, memory and gpu clock, power drawing - a minimum and a maximum from all cards - easy for spotting OC issues.
funny option like blinking cards LEDs on share accepted.
integrated overclocking of nVidia cards!
integrated pools monitoring - in progress 

Download : https://mirrorace.com/m/1qikt

You can find the ready to use package in : 
Install
WinEther uses Qt as main developpement framework. The binary (WinEther.exe) depends on several Qt libraries. You can find them in the archive availabe on the release page [https://github.com/digitalpara/WiNETH]. nVidia option needs the nvml.dll (or .so). On Windows you can copy and paste it in your WinEther directory or add path in the PATH environment variable. Traditionaly, the path is: "C:\Program Files\NVIDIA Corporation\NVSMI"

Usage
1 - Start WiNETH Miner.

2 - Fill the ethminer binary path in the first edit box, e.g.:

C:\Users\USERNAME\Desktop\ethminer\ethminer.exe

3 - Fill the ethminer's startup parameters, as you would normally use on your ethminer startup script, but excluding "ethminer.exe" before, e.g.:

-RH -U -P stratum+ssl://WALLET_ID.MINER_NAME@eu1.ethermine.org:5555

4 - Check the options you want to activate.

5 - Click on "Start mining".

All the parameters you set are automaticaly saved and WinEther will use them on next run.

Please note, "Auto mining" isn't auto startup of the program! We suggest to autorun the WinEther.exe on startup > head to Users/USERNAME/AppData/Roaming/Microsoft/Windows/Start Menu/Programs/Startup and paste a linked file for autostarting.

Build
You need Qt installed (5.9 was used but all 5.x versions are compatible). Open the .pro file with Qt Creator. Clic on "configure" with the good configuration. Then you can build (execute qmake and compile). If you don't want to build for nVIDIA GPU, delete the NVIDIA flag in the DEFINE option in the .pro file.

Contribute
Feel free to make pull request. You can also chat with other users and me on Gitter.

Donation
By default, the binaries built using the code include an automatic donation system: Every 4 hours, ethminer will be restarted using the 0x7F5BB53c415334235a9E42eA03695F11b6553C0D ethereum address in the parameters during 5 minutes. When this 5 minutes delay is gone, ethminer is restarted using the user credentials. If you prefer to not use this system, you have to uncheck the donation checkbox in the About dialog.

You can also donate Ethereum directly on 0x7F5BB53c415334235a9E42eA03695F11b6553C0D
