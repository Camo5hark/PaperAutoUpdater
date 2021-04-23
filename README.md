# PaperAutoUpdater
 
PaperAutoUpdater is a small, easy-to-implement Java program that is used to update a PaperMC build executable to the most recent build from the [Paper website](https://papermc.io/). It supports all versions of paper from 1.8 to 1.16, even though 1.16 is the only maintained version.

The reason I made this program is because I wanted to always have the most recent build of PaperMC to get the most recent vanilla bug fixes and performance improvements. I used Java to make this program because Java is needed to run Paper anyway. The program is compiled with Java 8 and should work with all versions 8 and above. The only library used is [Google GSON](https://github.com/google/gson).

# Installation

All that is needed to run this program is Java 8 or above. The release executables can be found on this page.

- Put the PaperAutoUpdater executable in your Minecraft server directory. 
- Run PaperAutoUpdater before the server every time you want to run the server.

The executable requires two arguments, the first being the version of paper you want to update to, and the second being the name of the server executable to install the update. Example update command:

```
java -jar PaperAutoUpdater-1.1.jar 1.16 paper.jar
```

Make sure the server executable you run to start the server is the same as the server executable updated by PaperAutoUpdater.

If you are using a shell or batch script to start your server, run the PaperAutoUpdater executable before the server. Example server start script:

```
java -jar PaperAutoUpdater-1.1.jar 1.16 paper.jar
java -jar -Xms1G -Xmx4G paper.jar
```
