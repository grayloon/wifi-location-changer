# WiFi Location Changer
* Automatically change location when WiFi connection changes in Mac OS X
* Allows having different IP settings depending on the WiFi SSID
* Automatically select the location corresponding to the SSID, if none
  exists: select the "Other" location

## Installation
Note: location name should be the same as the name of SSID with all spaces removed.

For example: **SSID**: ```GrayLoon``` Will translate to **Location Name**: ```Gray Loon```

    sudo mkdir /usr/local/var/log
    sudo cp locationchanger /usr/local/bin/
    cp LocationChanger.plist ~/Library/LaunchAgents/
    launchctl unload ~/Library/LaunchAgents/LocationChanger.plist
    launchctl load ~/Library/LaunchAgents/LocationChanger.plist

or

    ./install
