**HoRNDIS** (pronounce: *"horrendous"*) is a driver for Mac OS X that allows you to use your Android phone's native [USB tethering](http://en.wikipedia.org/wiki/Tethering) mode and [genucard](http://www.genua.eu/produkte/genucard/index.en.html) to get Internet access.

For more information, [visit the home page for HoRNDIS on my site](http://www.joshuawise.com/horndis).

Build and Install:
 1. Download MacOS 10.6 SDK and extract to macosx10.6/
 2. Install XCode
 3. $ xcodebuild
 4. $ sudo rm -rf /System/Library/Extensions/HoRNDIS.kext/
 5. $ sudo cp -r build/Release/HoRNDIS.kext /System/Library/Extensions/
 6. $ sudo chmod -R 755 /System/Library/Extensions/HoRNDIS.kext/
 7. $ sudo chown -R root:wheel /System/Library/Extensions/HoRNDIS.kext/
 8. $ sudo kextload /System/Library/Extensions/HoRNDIS.kext/
