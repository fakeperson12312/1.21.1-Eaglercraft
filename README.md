# 1.21.1-Eaglercraft
These are the files for a 1.21.1 Eaglercraft Server

# Usage
Go click the green code button, codespaces, then create new
Open two terminals (use control-shift-p then type terminal)
In one terminal:
```bash
cd main && java -jar purpur.jar
```
In the other terminal:
```bash
cd proxy && java -jar velocity.jar
```
Then go to the ports section and forward port 8081, right click and make it public. 
To use the server, go to eaglercraft, direct connect or wtv u want.
Paste in the given link, but replace https:// with wss://
And you can connect!

# Java Version Sidenote
You should get Java 21, which is the version I use. On one of my computers, Java 23 didn't work. 
To get Java 21:
```bash
wget https://download.oracle.com/java/21/archive/jdk-21.0.4_linux-x64_bin.deb
sudo dpkg -i jdk-21*.deb
```
And to ensure that it worked, just update it if it isn't java 21:
```bash
sudo update-alternatives --config java
java --version
```

# More Side Notes
This server has a shop plugin already installed, along with some other plugins. Some are neccesary, like nlogin and via* but If you don't want it, you can remove things like skript and protocolib. 
Also, It can be used as a real minecraft server that people can connect to. This repository will mostly not be updated, and I might add a resource pack later in the server.properties that might not work later. 
I'll add a waterfall proxy soon, but once that happens, you'll have to cp -r the plugins each time, or use a symbolic link between them. Symbolic link requires the tinyest bit of more knowledge, ill just say that it involves "ln -s <dir> <dir2>"
