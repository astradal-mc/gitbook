# Portstones

## AstradalPorts Player Guide

Welcome to **AstradalPorts**, a plugin that enables immersive, lore-friendly travel between major towns and nations via magical lodestones called **portstones**. This guide covers all the features and commands available to players.

***

### ✨ What Are Portstones?

Portstones are special **lodestones** that allow fast travel between distant towns and nations. There are three types:

* ✈ **Airship Portstones** (Nation-only)
* 🌊 **Sea Portstones** (Town-controlled)
* ⛺ **Land Portstones** (Town-controlled)

Each type only connects to other Portstones of the **same type**.

***

### 🚪 How to Use a Portstone

1. **Find a Portstone** (a lodestone block in your town).
2. **Right-click** the lodestone to open the destination menu.
3. Choose a destination from the GUI.
4. Wait for a short teleportation **warmup period**
5. **Do not move**, or the teleport will cancel.
6. You will be teleported near the destination Portstone!

***

### ⏱ Cooldowns

Each Portstone type has its own cooldown timer to prevent rapid travel:

* Attempting to use another portstone of the same type before the cooldown expires will fail.
* Cooldown duration is displayed in the GUI if active.

***

### 💸 Travel Fees

Some towns may charge a fee for travel:

* Fees are displayed in the GUI when selecting a destination.
* Fees are **automatically deducted** from your balance.
* The fee is deposited directly into the destination town's bank.

***

### 🔨 Editing Portstones (Town Mayors Only)

If you are a **mayor**, you can customize Portstones in your town:

`/portstone edit <property> <value>`

Look directly at the Portstone to edit it.

#### Editable Properties:

* `name` — Display name in the GUI.
* `fee` — Travel cost in dollars.
* `icon` — Item shown in the GUI.
  * Can be the item in your hand.
  * Or use `/portstone edit icon <material_name>` with tab completion.

***

### 📃 Useful Commands

#### View Info About a Portstone:

`/portstone info`

* Look at the Portstone to show its full info.

***

If you run into any issues or have suggestions, contact a server admin or visit the support Discord. Happy travels!
