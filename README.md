# QT Teleporter
Teleportation system prefab for VRChat Avatar 3.0.

Simple asset, easy to install with only 2 boolean parameters and 2 animation layers.

Only PCVR and Desktop compatible, not Quest compatible.

## Usage
From the expression menu, you can drop either Portal A or Portal B.
Any other user than yourself can sit on either portals, and when they get out of the station, they will be at the location of the other portal.

## Installation
[Youtube installation guide](https://www.youtube.com/watch?v=PCiYrx87aYc)

### Base installation
1. Download the latest release from [GitHub Releases](https://github.com/dbqt/QTTeleporter/releases)
2. Import the unitypackage into your project.
3. From the folder QTTeleporter, drag the prefab QTTeleporter into the scene.
4. Right-click on the prefab and unpack completely.
5. Place the QTTeleporter object at the root of the avatar.
6. Under QTTeleporter/WorldAnchor/Container/ConstraintA assign the root of your avatar's armature to the sources, then click 'Zero'.
7. Under QTTeleporter/WorldAnchor/Container/ConstraintB assign the root of your avatar's armature to the sources, then click 'Zero'.

### Add as new FX layer
1. On the VRCAvatarDescriptor, under Playable Layers, assign to the FX layer the animator controller QTTeleporterFX.
2. On the VRCAvatarDescriptor, under Expressions, assign the QTTeleporterMenu to the Menu and QTTeleporterParameters to the Parameters. 

### Add to existing FX layer
1. Download and install the latest version of [VRLabs's Avatars 3.0 Manager](https://github.com/VRLabs/Avatars-3.0-Manager) to get the tool to merge animators. 
2. From the VRLabs menu, open the Avatars 3.0 Manager.
3. Drag your VRC avatar descriptor into the panel.
4. Open the FX section and click on add animator to merge.
5. Add the animator QTTeleporter FX to merge as new.
6. On the avatar's VRCAvatarDescriptor, open your existing Expression Menu and add QTTeleporterMenu as a sub menu item to your existing menu.
7. On the avatar's VRCAvatarDescriptor, open your existing Expression Parameters and copy all the parameters from QTTeleporterParameters over exactly the same way.

### Customization
If you want to customize the portals themselves, you can replace the models that are under QTTeleporter/WorldAnchor/Container/ContraintA/StationsA/ModelA (or B) with your own 3D model

Feel free to modify as you see fit, this is under MIT license.
If you have any questions, join the [Discord](https://discord.com/invite/kmdh6RQ) to ask me directly.