# Warning
This is incomplete. Do not follow this guide.

# Setting Up your Sidecraft Installation
Setting up Sidecraft can be a bit complicated, but here's a guide to walk you through it! You'll need an internet connection and Microsoft Sysinternals' Process Explorer, though.
You can find it on their [website](https://learn.microsoft.com/en-us/sysinternals/downloads/process-explorer).

## 1. Sidecraft Installation Structure
Sidecraft has a similar but unique to that of a vanilla Minecraft installation. Begin setup by creating a folder that will contain all of the files for this Sidecraft installation.

## 2. Obtaining Minecraft's Per-Instance Files
When you start Minecraft, it downloads a ton of JAR files that are needed to run the game and puts them in a folder *somewhere* on your system. It's pretty straightforward
to find it, though.
1. Launch Minecraft 1.12.2 using the official Minecraft launcher. Note that modded versions of the game are not compatible with Sidecraft and will result in errors or possible damage
to your Sidecraft installation.
3. Launch ProcessExplorer and locate the Java process running Minecraft. It's probably called `javaw.exe`.
4. Right-click on the process and select *properties*. The Properties window shows the Command Line option for the process. Copy everything from that text box and paste it into Notepad.
5. Now, we need to locate the Java Libraries folder. Look for the file path that comes right after `-Djava.library.path=`. It should be towards the beginning of the text you copied.
6. Next, create a new folder in your Sidecraft installation folder called `javaLibraries`. Copy the *contents* of the folder you just located into this new `javaLibraries` folder.
