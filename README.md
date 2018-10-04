# MLB Gameday Downloader
A tool to download MLB Gameday data written in Java. ONLY WORKS ON WINDOWS.

http://gd2.mlb.com/components/game/mlb/ <-- fetched from here

The executable can be found in the /bin folder. 

The Downloader takes two parameters, the first is the year that you wish to download, the second is the path to where you want to download the files.

Example:

java -jar Downloader.jar 2014 "c:\Users\me\pitchfx"

NOTE: The tool is multithreaded, and will download an entire season in about 5 minutes. There's a chance that mlb.com will frown upon the speed of HTTP requests made and throttle/block your IP address, but this has not happened to me yet.

*Fixed issue with minor URL modifications to allow for program to function properly.

*Add 3rd command line parameter to specify league (i.e. mlb,aaa,etc.)

*Adjusted date range to support collection of Spring Training, Exhibition, etc games.

*Added in collection of game.xml, gameday_Syn.xml & linescore.xml information as well
