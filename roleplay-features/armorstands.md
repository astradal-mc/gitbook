---
description: Armor stand and display entity editor.
icon: people-robbery
cover: >-
  https://camo.githubusercontent.com/2ef9520fc54aeab52efb021c45f93c067854dba19dd0ed2e9a775015629b2cb2/68747470733a2f2f63646e2e35363733382e6d652f6561737961726d6f727374616e64732f62616e6e6572322e706e67
coverY: 0
---

# Armorstands

## Official wiki

{% embed url="https://github.com/56738/EasyArmorStands#readme" %}

## Usage

Use `/eas give` and follow the instructions.

If you get stuck, refer to the detailed instructions below.

### Demo video

[![Demo video](https://camo.githubusercontent.com/bb7b0c8513c36c5447f619f022aed317fd5f8a05faddcf564c152e145c489927/68747470733a2f2f692e7974696d672e636f6d2f76692f64515a6b42336d657a2d302f302e6a7067)](https://youtu.be/dQZkB3mez-0)

### Controls

* Right-click: Select
* Left-click: Go back
* Left-click: Open menu
* Q: Deselect entity
* Shift: Disable snapping
* F: Switch between local/global/scale modes

### Editing entities

Hold the tool and right-click an entity to select it.

[![Tools](https://camo.githubusercontent.com/afa5e983d8c2db9986f6c9315eebeb6c69615dd4020b0b97b655e26c2c6751be/68747470733a2f2f63646e2e35363733382e6d652f6561737961726d6f727374616e64732f73637265656e73686f74732f746f6f6c73322e706e67)](https://camo.githubusercontent.com/afa5e983d8c2db9986f6c9315eebeb6c69615dd4020b0b97b655e26c2c6751be/68747470733a2f2f63646e2e35363733382e6d652f6561737961726d6f727374616e64732f73637265656e73686f74732f746f6f6c73322e706e67)

Right-click a line to use the **Move** tool. Move your cursor by walking or looking around, then right-click to confirm your changes. You can abort your changes and restore the previous position by left-clicking instead.

Right-click a circle to use the **Rotate** tool. This works just like the Move tool.

Some entities let you switch between local and global mode by pressing F. Local mode is affected by the rotation, for example, you can use it to move an armor stand along its arms. Global mode uses global coordinates.

Use `/eas undo` and `/eas redo` to undo/redo your changes. You can undo any operation performed using EasyArmorStands, as well as manually placing or destroying armor stands.

### Armor stands

Armor stands have 7 bones:

* Head
* Body
* Left arm
* Right arm
* Left leg
* Right leg
* Position

After selecting an armor stand, you will also have to select which bone you want to edit. The Position bone is the yellow point in the middle (below the head), the other bones are the white lines.

[![Bones](https://camo.githubusercontent.com/750d123e95f7bbc88a4e27f71214bbcf2121f5472b4f5ec39af2b998f0f3ae15/68747470733a2f2f63646e2e35363733382e6d652f6561737961726d6f727374616e64732f73637265656e73686f74732f626f6e65732e706e67)](https://camo.githubusercontent.com/750d123e95f7bbc88a4e27f71214bbcf2121f5472b4f5ec39af2b998f0f3ae15/68747470733a2f2f63646e2e35363733382e6d652f6561737961726d6f727374616e64732f73637265656e73686f74732f626f6e65732e706e67)

You can pick up and carry the armor stand by selecting the position bone and then selecting the **Pick up** tool in the middle (where the lines meet).

Use `/eas name` to edit the custom name of an armor stand. This is often used for holograms. Format the name using [MiniMessage](https://docs.advntr.dev/minimessage/format.html).

**Hint:** If you are on 1.19.4+, you should use text displays for holograms, see below.

### Display entities

Display entities can be edited just like armor stand bones.

Additionally, they can be scaled. Enter the **Scale** mode by right-clicking without looking at anything, just like switching between local and global mode.

Use the menu to place an item into an item display.

Use `/eas text` to edit the text of a text display. Format the text using [MiniMessage](https://docs.advntr.dev/minimessage/format.html). This command also has some subcommands such as `/eas text background`, which can be used to change the background color.

**Hint:** Set the billboard mode to `center` in the menu and reset the rotation (`/eas reset`) to create a hologram which always looks at the player.

Place a block in a block display by holding Shift and left-clicking it, or use `/eas block`. This command also supports block states like `minecraft:birch_stairs[facing=east]`.

Use `/eas box` to resize or move the bounding box. Setting up a bounding box is important for client-side rendering performance. The client will not render display entities if the bounding box is not visible on the screen. By default, display entities do not have a bounding box, so they are always rendered.

Use `/eas brightness` to set a custom brightness (light level) of a display entity.

### Group selection

Hold Shift while right-clicking an entity to add it to your group selection. After selecting the entities you want to edit, right-click anywhere without holding Shift to begin editing the group.

[![Group](https://camo.githubusercontent.com/56f5a44f4fd74153d3bd2e6e75898489d059c7c94a27394f7320c66952f13486/68747470733a2f2f63646e2e35363733382e6d652f6561737961726d6f727374616e64732f67726f75702e706e67)](https://camo.githubusercontent.com/56f5a44f4fd74153d3bd2e6e75898489d059c7c94a27394f7320c66952f13486/68747470733a2f2f63646e2e35363733382e6d652f6561737961726d6f727374616e64732f67726f75702e706e67)

### Menu

[![Menu](https://camo.githubusercontent.com/7e9e22452c6c9f078609487e37d1566153c8bba06c8ca76287dd70189622cb7d/68747470733a2f2f63646e2e35363733382e6d652f6561737961726d6f727374616e64732f6d656e75322e706e67)](https://camo.githubusercontent.com/7e9e22452c6c9f078609487e37d1566153c8bba06c8ca76287dd70189622cb7d/68747470733a2f2f63646e2e35363733382e6d652f6561737961726d6f727374616e64732f6d656e75322e706e67)

The menu can be accessed by left-clicking while no bone or tool is selected. Group selections do not support the menu.

On the bottom left, you can edit the entity equipment slots (armor, held items).

The bottom right contains shortcut buttons to quickly select a certain bone.

Armor stand settings such as visibility can be changed using the buttons in the top right.

#### Head Database integration

If [Head Database](https://www.spigotmc.org/resources/head-database.14280/) is installed and you have permission to use it, you can click the button in the top left to open its menu. After selecting a head, you are returned to the EasyArmorStands menu and can quickly place it into an equipment slot.

### Commands

This list contains some important commands for features which cannot be accessed using the menu. Use `/eas help` to see the full list of commands and their full usage.

* `/eas give`: Give yourself the editor tool
* `/eas align`: Move the selected entity to the middle of its block
* `/eas snap angle`: Toggle angle snapping (or specify an increment)
* `/eas snap move`: Toggle position snapping (or specify an increment)
* `/eas reset <property>`: Reset a property
