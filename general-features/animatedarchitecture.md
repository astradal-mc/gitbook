---
description: >-
  Use animated blocks that can be used to create many kinds of animated
  architectural structures.
icon: wind-turbine
---

# AnimatedArchitecture

This plugin is a rewrite of the old Bigdoors plugin, so if you're familiar with that, this should be easy.

## Preview

[![AnimatedArchitecture Showcase](https://camo.githubusercontent.com/82e2b2fac1cadd9acefc2a158b9c555fbc31ea770ea242b89cf07a68fc6267c1/68747470733a2f2f696d672e796f75747562652e636f6d2f76692f34355477464c42763879592f302e6a7067)](https://www.youtube.com/watch?v=45TwFLBv8yY)

## Commands

All command fields with <> brackets are mandatory, all command fields with \[] brackets are optional.

| Command                                                                   | Description                                                                   |
| ------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `/aa help [query]`                                                        | Display list of available commands, or a specific command.                    |
| `/aa menu`                                                                | Display GUI menu to create or manage your AA structures.                      |
| `/aa addowner <newOwner> <permissionLevel> <structureRetriever>`          | Add another owner to a structure.                                             |
| `/aa cancel`                                                              | Cancels any process without waiting for your input.                           |
| `/aa close <structureRetriever>`                                          | Closes a structure if possible.                                               |
| `/aa confirm`                                                             | Confirms an action AnimatedArchitecture wants to perform.                     |
| `/aa delete <structureRetriever>`                                         | Deletes a structure.                                                          |
| `/aa delete <structureRetriever>`                                         | Prints the information about a specific structure.                            |
| `/aa inspectpowerblock`                                                   | Gives you a tool to inspect which structures are associated with a powerblock |
| `/aa liststructures [structureName]`                                      | List all structures, optionally using criteria.                               |
| `/aa lock <lockStatus> <structureRetriever> [SendUpdatedInfo]`            | (Un)locks a structure                                                         |
| `/aa movepowerblock <structureRetriever>`                                 | Moves the powerblock to a different location                                  |
| `/aa newstructure <structureType> [structureName]`                        | Creates a new structure                                                       |
| `/aa open <structureRetriever>`                                           | Opens a structure if possible                                                 |
| `/aa preview <structureRetriever`                                         | Previews an animation using glowing blocks                                    |
| `/aa removeowner <targetPlayer> <structureRetriever>`                     | Removes an owner of a structure                                               |
| `/aa setblockstomove <blocksToMove> [structureRetriever]`                 | Changes the number of blocks a structure will move for supported types        |
| `/aa setname <name>`                                                      | Sets the name of a structure during the creation process                      |
| `/aa setopendirection <direction> [structureRetreiver] [sendUpdatedInfo]` | Changes the opening direction of a structure                                  |
| `/aa setopenstatus <isOpen> [structureRetriever] [sendUpdatedInfo]`       | Changes the open status of a structure without actually moving it             |
| `/aa toggle <structureRetriever>`                                         | Toggles a structure                                                           |

## Supported structure types

The following structure types are currently supported:

* Big Doors
* Clocks that display the in-game time
* Drawbridges
* Flags
* Garage Doors
* Portcullises
* Revolving Doors
* Sliding Doors
* Windmills
