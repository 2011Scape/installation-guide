<p align="center">
  <img src="https://cdn.discordapp.com/attachments/1067274729205010463/1082144752985702451/2011scapelogo.png" />
  <br>
  <br>
  <br>
  <img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080005453053956178/image.png" />
  <br>
</p>

# Installation Guide

Welcome to the 2011Scape installation guide, in this guide we will discuss the steps required to install 2011Scape to your local machine and begin the process of developing content, or playing single-player.

Things to keep in mind when installing 2011Scape are that there is no officially supported single-player mode, and that if you choose to play single-player with the bleeding edge commit activity, you are risking your game progress with possible game-breaking bugs. All commits to the official world are not uploaded until quality assured to the best of our ability.

# Required Tools, Files

To begin, you'll need to make sure you have the following files downloaded, and installed.

- [IntelliJ IDE](https://www.jetbrains.com/idea/download/)
- [GitHub Desktop](https://desktop.github.com/)
- [667 Cache](https://archive.openrs2.org/caches/runescape/278/disk.zip)
- [667 xteas](https://github.com/2011Scape/installation-guide/releases/download/v1.0/xteas.json)
- [JDK 11](https://www.techspot.com/downloads/5553-java-jdk.html)

**Note: JDK 11 is required for the RS-Client repository, using newer versions of the Java Development Kit is currently untested, and Java 11 is the recommended option**

You can skip any of these downloads if you have them already installed, or saved somewhere.

# Game Server Cloning

<b>The first step of installation is the game server. To begin, we'll need to clone the repository. To begin, head to the game repository and fork the repository.</b>
<br>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080014884953129080/image.png" />
</p>
<br>
<br>
<br>
<br>
<b>Feel free to name the fork whatever you wish, in my case I'll call it 2011Scape-game to make sure that I can recognize it when sifting through my personal repositories.</b>
<br>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080015188553629726/image.png" />
</p>
<br>
<br>
<br>
<br>
<b>Next, install and open up GitHub Desktop and start by signing in. Once you are signed in, you should see a screen like this.</b>
<br>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080013590217633792/image.png" />
</p>
<br>
<br>
<br>
<br>
<b>Now we'll want to clone the repository we just forked, click on "File" and then "Clone repository..."</b>
<br>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080014026542686349/image.png" />
</p>
<br>
<br>
<br>
<br>
<b>Go ahead and search for the repository you just forked, and click "Clone"</b>
<br>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080016546031738891/image.png" />
</p>
<br>
<br>
<br>
<br>
<b>You should finally come to a screen that looks like this, go ahead and keep the selection "To contribute to the parent project" active and click continue. Congratulations, you just finished forking and cloning the game server!</b>
<br>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080017187995123783/image.png" />
</p>
<br>
<br>
<br>
<br>

# Game Server Installation

<b>Next up we'll want to install the game server on IntelliJ. Make sure you have your cache and xteas downloaded, and IntelliJ installed. To make life easier for you, you can open up the project from GitHub desktop into IntelliJ like so.</b>
<br>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080017972090896404/image.png" />
</p>
<br>
<br>
<br>
<br>
<b>You should get a screen that looks like this. Allow some time for Gradle to download the required libraries and to set-up the project, for some computers this can take awhile so be patient!</b>
<br>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080018349288853554/image.png" />
</p>
<br>
<br>
<br>
<br>
<b>Once Gradle has finished installing and indexing properly, you'll want to get the files from your cache download and place them in data/cache/</b>
<br>
<b>Simply locate and extract the files from the cache.zip you downloaded, you want to make sure you're grabbing the raw files and not the folders.</b>
<br>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080019161251594240/image.png" />
</p>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080019371918893076/image.png" />
</p>
<br>
<br>
<br>
<br>
<b>Next up, make sure xteas.json is downloaded and place the file in data/xteas/</b>
<br>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080019792636936262/image.png" />
</p>
<br>
<br>
<br>
<br>
<b>You should now have all the required files in place, which means next up is adding a Gradle run configuration. Follow the next 3 pictures and make sure your Run task is exactly how I wrote it. This is important to ensure that plugins are properly being built when running the server.</b>
<br>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080019983381307443/image.png" />
</p>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080020126629371924/image.png" />
</p>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080020251145670728/image.png" />
</p>
<br>
<br>
<br>
<br>
<b>Once you've done that, you can now run the server! Simply click on the "Play" button and if you've installed everything correctly, you should see a screen that looks like this.</b>
<br>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080021221384654848/image.png" />
</p>
<br>
<p align="center">
<img src="https://cdn.discordapp.com/attachments/1067274729205010463/1080021770909782066/image.png" />
</p>
<br>
<br>
<br>
<br>
<p align="center">---</p>
<br>
<br>

If you are still having issues installing the game server, then we implore you to join our Discord at [2011Scape Discord](https://discord.gg/jDbBAKjhxh) for further help. 

# File-Server Installation

In order to run 2011Scape locally, you need to run the File Server as well. 

To do this, you must first clone the File Server:

`git clone https://github.com/2011Scape/file-server`

Next, you'll need to copy the cache files into file-server/cache like above with the Game Server.

After you have copied the cache to the File Server, you must cd into it:

`cd file-server`

Now you need to run the File Server via Gradle. 

If you are on Windows, you need to run this command:

`gradlew.bat run`

If you are on Linux, you need to run this command:

`./gradlew run`

After that, you should see the File Server running and ready to serve files to your local client.
