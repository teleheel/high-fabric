# High Fabric

A high fantasy fabric modpac

**To download and play the modpack:**

1. Create a new instance in MultiMC with Minecraft 1.19 and Fabric Loader 0.14.10.
2. Download the packwiz-installer-bootstrap from [https://github.com/packwiz/packwiz-installer-bootstrap/releases](https://github.com/packwiz/packwiz-installer-bootstrap/releases) and place it in the instance Minecraft folder.
3. Right click the MultiMC instance, select `Edit Instance` and go to the `Settings`.
4. Select the `Custom commands` tab, and check the box that says `Custom commands`.
5. Paste `"$INST_JAVA" -jar packwiz-installer-bootstrap.jar https://teleheel.github.io/high-fabric/packwiz/pack.toml` inside the Pre-launch command: field.
6. Run the MultiMC instance to automatically download and install the modpack.

**To download and run a serverpack:**

1. Download the Fabric installer from [https://fabricmc.net/use/installer/](https://fabricmc.net/use/installer/) and run it.
2. Select the `Server` tab.
3. Select the following options:
    - Minecraft Version: 1.19
    - Loader Version: 0.14.10
    - Select Install Location: choose a location your server files

4. Click `Install`
5. In the pop-up saying "Server successfully installed", click the `Download server jar` button.
6. Click the `Generate` button.
7. When it's finished, click `done`.
8. Download the packwiz-installer-bootstrap from [https://github.com/packwiz/packwiz-installer-bootstrap/releases](https://github.com/packwiz/packwiz-installer-bootstrap/releases) and place it in the server folder.
9. Open `start.bat` in the server folder with notepad (or any other text editor).
10. Delete everything in `start.bat`, and then paste

        java -jar packwiz-installer-bootstrap.jar -g -s server https://teleheel.github.io/high-fabric/packwiz/pack.toml
        java -Xmx4G -Xms4G -jar fabric-server-launch.jar nogui
        Pause

11. Run (double click) on `start.bat` to launch the server and automatically download and install the modpack.
