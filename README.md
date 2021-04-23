# PaperAutoUpdater
 
PaperAutoUpdater is a Java program that is used to update a PaperMC build executable to the most recent build from the [Paper website](https://papermc.io/). The reason I made this program is because I wanted to always have the most recent build of PaperMC to get the most recent vanilla bug fixes and performance improvements.

I used Java to make this program because Java is needed to run Paper anyway. The program is compiled with Java 8 and should work with all versions 8 and above. The only library used is [Google GSON](https://github.com/google/gson).

# Installation

All that is needed to run this program is Java 8 or above. The release executables can be found on this page.

Put the PaperAutoUpdater executable in your Minecraft server directory. If you already have a PaperMC executable installed, make sure the file is named `paper.jar` (this is how the PaperAutoUpdater program knows which file is the PaperMC executable). If it is not, rename it.
Run PaperAutoUpdater before the server every time you want to run the server.

If you are using a shell or batch script to start your server, run the PaperAutoUpdater executable before the server. Example:

```
java -jar PaperAutoUpdater-X.x.jar
java -jar -Xms1G -Xmx4G paper.jar
```