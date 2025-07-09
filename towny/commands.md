---
icon: terminal
---

# Commands

> This list breaks each command down by word. Eg: /resident set perm {on/off}.

> For resident commands, the add command would auto-match online players, while add+ requires exact spelling to choose offline players.

> Just about every subcommand has it's own help menu. Use /resident set, or a similar cutoff, to show all the options for that command ingame. You can also use /resident set ?, you will probably need to use that in the case where a subcommand actually has a function by itself. Example: /town claim, and /town claim ? would show all it's subcommands.

> The { } brackets are used to show variables, or what you need to fill in. The elipse ".." (or shortened elipse) is used to show that you can specify multiple things at once (like inviting 10 residents at once).

> The {bleh/blah/bluh} is used to show that the input can be multiple words.

> An empty bullet represents that the subcommand itself does something and will not show a help menu.

## /towny

*
  * Shows basic towny commands.
* ? - Shows more towny commands.
* allowedblocks - Opens a menu where you can check what blocks might be allowed to be built/destroyed in
* itemuse - Shows the items in the item\_use\_ids list.
* map - Shows the towny map.
  * hud - Activates the map in the player's scoreboard.
* plotclearblocks - Shows the blocks deleted using `/plot clear`
* prices - Shows taxes/costs associated with running a town.
* switches - Shows the blocks in the switch\_ids list.
* time - Shows time until next new-day (tax/upkeep collection.)
*   top

    * residents {all/town/nation} - Shows top residents.
    * land {all/resident/town} - Shows top land owners.



## /plot



* Shows the /plot commands.
* claim - Resident command to personally claims a plot that are for sale.
  * auto - Resident command to personally claim an area of plots that are for sale, around the player typing the command.
* unclaim - Resident command to unclaim personally owned plots.
  * circle/rect - Resident command to unclaim personally owned plots in a circle or rectangle shape.
    * {# (radius around current position)} - Radius of the area to unclaim.
* {forsale/fs} - Set a plot for sale.
  * circle/rect - Set a shape.
    * {# (radius around current position)} - Radius of the area to set forsale.
  * \$$ - Cost of plot.
    * circle/rect - Set a shape.
      * {# (radius around current position)} - Radius of the area to set forsale.
* {notforsale/nfs} - Set a plot to not be for sale.
  * circle/rect - Set a shape.
    * {# (radius around current position)} - Radius of the area to set notforsale.
* district
  * create|new \[name] - Creates a new district, with the given name.
  * add {name} - Adds a townblock to the given district. If you are actively adding to a district you do not need to continue supplying the name.
  * rename \[name] - Changes the name of a district.
  * remove - Remove the townblock you are stood in from a district.
  * delete - Deletes the district you are stood in.
* evict - Used to remove a plot from a plot owner, usually by the mayor or assistant.
  * forsale - Evicts the plot owner and puts the plot up for sale immediately.
* trust
  * add {name} - Adds a player as Trusted on the plot.
  * remove {name} - Removes a player from being Trusted on the plot.
* perm - Shows the perm line of the plot in which the player stands.
  * gui - opens the GUI to configure the plot perm override.
  * add {name} - Adds a player to the plot perm override.
  * remove {name} - Removes a player from the plot perm override.
* perm hud - Toggles on/off the plot perm hud scoreboard which shows the perm line of the plot in which the player stands along with more useful plot info.
* set
  * reset - Sets a shop/embassy/arena/wilds plot back to a normal plot.
  * shop - Sets a plot to a shop plot.
  * embassy - Sets a plot to an embassy plot.
  * arena - Sets a plot to an arena plot.
  * wilds - Sets a plot to a wilds plot.
  * inn - Set a plot to an inn plot.
  * jail - Set a plot to an jail plot.
  * farm - Set a plot to a farm plot.
  * bank - Set a plot to a bank plot.
  * outpost - Set a plot to an outpost plot, costs the same as /t claim outpost.
    * spawn - Sets the spawn point inside of an existing outpost plot to where the player is standing.
  * name - allows a mayor or plot-owner to rename plots they own, overwriting the \~Unowned message. Personal-plots display both the plot's given name and the name of the plot-owner.
  * perm
    * {on/off} - Edits the perm line of the single plot in which the player is standing. [See here for details.](https://github.com/TownyAdvanced/Towny/wiki/How-Towny-Works#towny-plot-perms)
    * {resident/ally/outsider} {on/off}
    * {build/destroy/switch/itemuse} {on/off}
    * {resident/ally/outsider} {build/destroy/switch/itemuse} {on/off}
    * reset - Resets the plot in which you stand to the default perm line of the /town or /resident screen (depending on if the plot is owned personally or by the town.)
  * minjoindays
    * {#] - Sets the # of days, or removes the minjoindays amount when clear is used.
    * clear - Removes the minjoindays requirement.
  * maxjoindays
    * {#] - Sets the # of days, or removes the maxjoindays amount when clear is used.
    * clear - Removes the maxjoindays requirement.
* toggle
  * fire - Turn on/off firespread in the plot in which you stand.
  * pvp - Turn on/off pvp in the plot in which you stand.
  * explosion - Turn on/off explosions in the plot in which you stand.
  * mob - Turn on/off hostile mobspawning in the plot in which you stand.
  * taxed - Turn on/off whether a plot will charge a plotowner taxes, while they own the plot personally.
* clear - Command to remove list of block id's from a plot, used by a mayor on town-owned land, or by a plot-owner on their personal plots.
* group
  * add|new|create {groupname} - Creates a plot group where a player is standing, also adds plots to an existing group.
  * remove - Removes the plot stood in from its plot group.
  * delete - Deletes a plot group entirely.
  * rename {newname} - Renames a plot group.
  * set {plottype} - Sets the group to a specified plot type. Not able to be used for Jail plots.
  * set perm ... - Used to set the perm line of the group you are standing in. See above section for /plot set perm for remainder of commands.
  * toggle ... - Used to toggle plot settings. See above section for /plot set toggle for remainder of commands.
  * forsale|fs {price} - Set the group for sale at the set price.
  * notforsale|nfs - Set the group not for sale.
  * trust
    * add {name} - Adds a player as Trusted on the plot group.
    * remove {name} - Removes a player from being Trusted on the plot group.
  * perm
    * gui - Opens the GUI to edit the plot perm override.
    * add {name} - Adds a player to the plot perm override.
    * remove {name} - Removes a player from the plot perm override.
*   jailcell

    * add - Adds a jail cell to a jail plot, where the player is stood.
    * remove - Removes a jail cell from a jail plot, where the player is stood.



## /resident

* Shows a player their resident screen.
* ? - Shows /res commands available.
* {resident} - Shows a player another player's resident screen.
* friend
  * add {resident} .. {resident} - Resident adds online player to their friends list.
  * add+ {resident} .. {resident} - Resident adds offline player to their friends list.
  * remove {resident} .. {resident} - Resident removes online player from their friends list.
  * remove+ {resident} .. {resident} - Resident removes offline player from their friends list.
  * clearlist - Removes all friends from a resident's friend list.
  * list - Returns a list of your friends.
* list - Lists residents in towny's data folder who are online.
* jail paybail - Allows a player to pay to get out of jail. Funds go to the town which owns the Jail.
* outlawlist {playername} - Display the list of towns in which a resident is outlawed in. Leave out the optional player name to see the towns in which you are an outlaw.
* plotlist
  * {#} - Shows a player their own list of plots, with an optional page number.
  * \[name] {#} - Shows a list of plots for the given player name, with an optional page number.
* spawn - If deny\_bed\_use: true and player has a current bed spawn, command will teleport player to their bed.
* toggle
  * pvp - Changes a resident's personally owned plots' PVP status.
  * fire - Changes a resident's personally owned plots' fire status.
  * explosion- Changes a resident's personally owned plots' explosions status.
  * mobs - Changes a resident's personally owned plots' mobs status.
  * map - Turns on map which refreshes when moving across plot borders.
  * townclaim - Turns on mode where /town claim is automatically used when moving across plot borders.
  * townunclaim - Turns on mode where /town unclaim is automatically used when moving across plot borders.
  * bedspawn - Turns on the mode where you will prefer your bed spawn over your town spawn.
  * plotborder - Turns on smokey plot-border view. Border shows when players cross to different townblocks.
  * constantplotborder - Turns on smokey plot-border view. Border doesn't disappear.
  * townborder - Turns on smokey plot-border view of the town you are stood in. Border doesn't disappear.
  * bordertitles - Turns on/off the Title messages seen when entering/leaving town, when using\_titles is true in the config.
  * plotgroup - Turns on a mode that will automatically add plots you enter into, into the plot group you are constructing.
  * spy - Admins can turn on chat-channel spying.
  * ignoreplots - Turns on/off plot notifications in town.
  * reset - This turns off all modes that are active.
  * infotool - Allows an admin to use the clay brick tool to determine the Bukkit names/classes of blocks and entities.
  * adminbypass - Used to make admins play as non-admins.
* set
  * perm
    * {on/off} - Edits the perm line on the resident screen. [See here for details.](https://github.com/TownyAdvanced/Towny/wiki/How-Towny-Works#towny-plot-perms)
    * {friend/ally/outsider} {on/off}
    * {build/destroy/switch/itemuse} {on/off}
    * {friend/ally/outsider} {build/destroy/switch/itemuse} {on/off}
    * reset - This takes the perm line seen in the /resident screen and applies it to all plots personally owned by the player typing it.
  * about
    * {message] - Sets a bio/about message shown in the /res status screen.
    * {clear} - Removes all of your modes.
    * {reset} - Removes all of your modes and re-assigns your default modes.
* tax {resname} - Shows taxes a player pays.



## /town

* Shows a player their town's town screen.
* ? - Shows /town commands available.
* {town} - Shows a player another town's town screen.
* here - Shows you the town screen of the town in which you stand.
* leave - Leaves a town.
* list
  * by name {page #} - order alpabetically.
  * by resident {page #} - order by town with most residents.
  * by balance {page #} - order by town with the highest nation bank balance.
  * by townblocks {page #} - order towns by how many townblocks they have claimed.
  * by online {page #} - order by how many players are online at that moment.
  * by open {page #} - lists open towns first, in order of most residents to least residents.
  * by public {page #} - lists public towns first, in order of most residents to least residents.
  * by ruined {page #} - lists ruined towns first, in order of most residents to least residents.
  * by bankrupt {page #} - lists bankrupt towns first, in order of most residents to least residents.
  * by founded {page #} - order by founded date, oldest first.
* online - Shows players in your town which are online.
* plots {townname} - Shows a helpful list of plots and their types/revenue which are owned by the town.
* new {townname} - Creates a new town.
* add {resident} .. {resident} - Mayor command to add residents to your town.
* kick {resident} .. {resident} - Mayor command to remove residents from your town.
* invite - Show a list of players who've been sent invites to your town.
  * sent - Show a list of players who've been sent invites to your town.
    * removeall - Denies all of your town's sent invites.
  * received - Show a list of invites your town has received from nations.
  * accept {nationname} - Accept an invite to join a nation.
  * deny {nationname} - Deny an invite to join a nation.
  * {playername} - Send an invite to a player to join your town.
* spawn - Teleports you to your town's spawn.
* spawn {town} - Teleports you to another town's spawn.
* claim - Mayor command to claim the townblock in which you stand for your town.
  * outpost <#|{name}|{name:#} - Claims an outpost for your town. {name} uses the plot name. {name:#} is used when a plot name begins with a number.
  * {# (radius around current position)} - Claims an area of townblocks around you for your town.
  * auto - Claims as many townblocks around you as is possible given money in townbank and available townblocks.
  * fill - Flood fills a surrounded section of plots. You must claim your border before using this command.
* unclaim - Mayor command to unclaim the townblock in which you stand.
  * all - Mayor command to unclaim all townblocks.
  * {# (radius around current position)} - Command to unclaim an area of townblocks around you.
  * outpost - Used to unclaim glitched outposts on MySQL Towny servers pre-0.92.0.0
* /town cede plot {townname}
  * Attempts to give the townblock the player is stood in, to the given town.
* withdraw
  * {$} - Removes money from town bank.
  * all - Withdraws all of the money from the town bank.
* deposit
  * {$} - Adds money from player to the town bank.
  * all - Deposits all of your money into the town bank.
  * {$} {townname} - Deposits money from player into the specified town's bank.
* baltop {townname} - Opens a book displaying the richest players in a town.
* bankhistory {#} - Opens a book GUI with # number of transactions listed, showing the town bank history.
* buy
  * bonus {amount} - Buys available bonus townblocks.
* allylist {townname} - Displays a list of allies for the Town.
* enemylist {townname} - Displays a list of enemies for the Town.
* delete {town name} - Admin/Mayor command to delete a town from towny's data folder's files.
* forsale|fs \[$] - Puts up a town for sale at the specified amount.
* notforsale|nfs - Removes a town being available for sale.
* buytown {townname} - Prompts a player to buy a town which is set for sale.
* merge {town name} - {town name} is the town which will be merged into the town owned by the mayor using the command.
* outlawlist {town} - Displays a list of outlaws for a town.
* outlaw {add/remove} {name} - Adds or removes an outlaw from a town's outlaw list
* outpost
  * {# (where # equals the corresponding outpost's number)} - Teleports to an outpost.
  * {list} - lists your town's outposts.
* plotgrouplist {townname} {page #} - Lists a town's plotgroups with forsale and price indicated.
* purge {days} - Kicks residents from the town who have been inactive for the given number of days, exempts npcs and mayors.
* ranklist {townname} - Displays residents and their ranks, optional townname to view another town's rank list.
* rank {add|remove} {playername} {rankname} - Grants or removes a rank to a resident of the town.
* reclaim - allows a resident to reclaim their ruined town.
* reslist {townname} - See a FULL list of all residents in a town.
* say {msg} - Broadcast a message to online town members.
* set
  * board
    * {message} - Sets message seen by residents upon logging in.
    * none - Sets an empty board which will not be seen on login or in the /town status screen.
  * mayor {resident} - Mayor command to give mayor status to another resident.
  * homeblock - Sets the homeblock and spawn of your town.
  * spawn - Sets the town spawn, must be done inside the homeblock.
  * spawncost - Set the cost of spawning to a public town. Doesn't affect town residents, nation members and nation-allies.
  * mapcolor {color} - Sets a town's mapcolor seen in the dynmap.
  * name {name} - Change your town's name.
  * outpost - Resets the outpost's spawn point to the player location. Must be used in an existing outpost plot.
  * perm
    * {on/off} - Edits the perm line on the town screen. [See here for details.](https://github.com/TownyAdvanced/Towny/wiki/How-Towny-Works#towny-plot-perms)
    * {resident/ally/outsider} {on/off}
    * {build/destroy/switch/itemuse} {on/off}
    * {resident/ally/outsider} {build/destroy/switch/itemuse} {on/off}
    * reset - This takes the perm line seen in the /town screen and applies it to all plots owned by the town.
  * tag {upto4character} - Sets the town's tag, which is sometimes used on that chat line.
    * clear - Clears the tag set for the town.
  * taxes {$} - Sets taxes collected from each resident daily. Also sets percentage if taxpercent is toggled on.
  * taxpercentcap {$} - The maximum amount that can be taken when taxpercent is enabled.
  * plottax {$} - Set taxes collected from each resident daily, per plot that they own.
  * plotprice {$} - Sets default cost of plot for the town.
  * shopprice {$} - Sets default cost of a shopplot for the town.
  * shoptax {$} - Set taxes collected from each resident daily, per shopplot that they own.
  * embassyprice {$} - Sets default cost of a embassy plot for the town.
  * embassytax {$} - Set taxes collected from each resident daily, per embassy plot that they own.
  * title {name} {titlegoeshere} - Mayor command to add a Title to a member of the town.
  * title {name} - Mayor command to remove a Title from a member of the town.
  * surname {name} {surnamegoeshere} - Mayor command to add a Suffix to a member of the town.
  * surname {name} - Mayor command to remove a Suffix from a member of the town.
  * primaryjail - Sets your town's primary jail.
* toggle
  * explosion - Turn on/off explosions in town.
  * fire - Turn on/off firespread in town.
  * mobs - Turn on/off hostile mobspawning in town.
  * public - Turn on/off public /town spawning and the co-ordinates of the town's homeblock in the /town screen.
  * pvp - Turn on/off pvp in town.
  * taxpercent - Turn on/off taxing by percent/flatrate.
  * nationzone - Turn on/off the town's NationZone.
  * open - Turn on/off public joining to your town.
* takeoverclaim - Used by a mayor to take over land from an overclaimed town, when overclaiming is allowed in the config.
* join {townname} - Command to join a town that doesn't require invites.
* jail
  * list - Shows jail number, name, coord, cellcount and which jail is the primary jail.
  * **When Bail is not Enabled:**
  * {name} - Jails the given player for 1 hour, must be a resident of your own town.
  * {name} {hours} - Jails the given player for the given hours.
  * {name} {hours} {jail} - Jails the given player for the given hours, in the given jail plot (which is a number.)
  * {name} {hours} {jail} {cell} - Jails the given player for the given hours, in the given jail plot and jail cell (which are both numbers.)
  * **When Bail is Enabled:**
  * {name} - Jails the given player for 1 hour, must be a resident of your own town, with the default bail amount.
  * {name} {hours} - Jails the given player for the given hours, with the default bail amount.
  * {name} {hours} {bail} - Jails the given player for the given hours, with the given bail amount.
  * {name} {hours} {bail} {jail} - Jails the given player for the given hours, with the given bail amount, in the given jail plot (which is a number.)
  * {name} {hours} {bail} {jail} {cell} - Jails the given player for the given hours, with the given bail amount, in the given jail plot and jail cell (which are both numbers.)
* unjail {name} - Unjails someone in your town's jail.
* trust
  * add {name} - Adds a player as Trusted to the entire town.
  * remove {name} - Removes a player from being Trusted by the entire town.
  * list - Displays a list of trusted players for the town.
* trusttown
  * add \[townname] - Adds an entire town as trusted in your town.
  * remove \[townname] - Removes an entire town as trusted in your town.
  * list - Displays a list of trusted towns in your town.

## /nation

* Shows a player their nation's nation screen.
* ? - Shows /nation commands.
* list
  * by name {page #} - order alpabetically.
  * by resident {page #} - order by nation with most residents across all towns.
  * by balance {page #} - order by nation with the highest nation bank balance.
  * by towns {page #} - order by nation with the most towns.
  * by townblocks {page #} - order nations by how many townblocks their towns have collectively claimed.
  * by online {page #} - order by how many players are online at that moment.
  * by open {page #} - ordered by open first, number of residents second.
  * by public {page #} - order by public first, number of residents second.
  * by founded {page #} - order by founded date, oldest first.
* online - Shows players in your nation which are online.
* {nation} - Shows a player the /nation screen of another nation.
* leave - Mayor command to leave the nation they are a part of.
* withdraw
  * {$} - King command to remove money from the nation bank.
  * all - Withdraws all of the money from the nation bank.
* deposit
  * {$} - Command to add money to the nation bank.
  * all - Deposits all of your money into the nation bank.
* baltop {nationname} - Opens a book displaying the richest players in a nation.
* bankhistory {#} - Opens a book GUI with # number of transactions listed, showing the nation bank history.
* deposit {$} {townname} - King command to add money to the bank of a town who is in the nation.
* new
  * {nationname} - Mayor command to create a nation.
* rank - Command to set assistant/custom ranks in the nation.
* add {town} .. {town} - Invites/Adds a town to your nation.
* kick {town} .. {town} - Removes a town from your nation.
* delete {nation} - Deletes your nation.
* invite - Show a list of invites sent.
  * help - Show a list of invites sent.
  * sent - Show a list of invites sent.
  * {town} - Invites a town to a nation.
* ally - Show a list of nation alliance invites sent.
  * add {nation} .. {nation} - Add a nation to your nation's ally list.
  * remove {nation} .. {nation} - Removes a nation from your nation's ally list.
  * accept {nationname} - Accepts an invitation to ally from another nation.
  * deny {nationname} - Denies an invitation to ally from another nation.
  * sent - Show a list of nation alliance invites sent.
  * received - Show a list of nation alliance invites received.
* enemy
  * add {nation} .. {nation} - Add a nation to your nation's enemy list.
  * remove {nation} .. {nation} - Removes a nation from your nation's enemy list.
* rank {add|remove} {playername} {rankname} - Grants or removes a rank to a resident of the nation.
* sanctiontown
  * add \[townname] - Adds a town to the sanctioned town list.
  * remove \[townname] - Removes a town from the sanctioned town list.
  * list - Lists your nation's sanctioned towns.
  * list \[nationname] - Lists the sanctioned towns of other nations.
* say {msg} - Broadcast a message to online nation members.
* set
  * king {resident} - King command to change the king of the nation.
  * capital {town} - Sets the capitol and king of the nation.
  * board
    * {message} - Sets message seen by residents upon logging in.
    * none - Sets an empty board which will not be seen on login or in the /nation status screen.
  * taxes {$} - Sets nationtax applied to the towns within the nation.
  * conqueredtax {$} - Sets a nation's conquered tax, which is paid by the conquered towns.
  * taxpercentcap - Sets the maximum amount that a town will pay in nationtax, when the nation has percent-based taxation.
  * name {name} - Sets the nation's name.
  * spawn - Sets the nation spawn point.
  * spawncost - Sets the cost of public spawns to that nation's spawn point. No effect on members of the nation or nation-allies
  * title {name} {titlegoeshere} - King command to add a Title to a member of the nation.
  * title {name} - King command to clear a Title from a member of the nation.
  * surname {name} {surnamegoeshere} - King command to add a Suffix to a member of the nation.
  * surname {name} - King command to clear a Suffix from a member of the nation.
  * tag {upto4character} - Sets the nation's tag, which is sometimes used on that chat line.
    * clear - Clears the tag set for the nation.
  * mapcolor {color} - Sets the colour seen on the dynmap-towny webpage.
* toggle
  * neutral - Sets whether your nation will pay daily to be neutral during towny war.
  * open - Sets the nation to be open, so that any town can join without an invite.
  * taxpercent - Turns on and off the percentage-based taxation of towns in the nation.
* join {nation}
  * Used by a town mayor to join an open nation.
* merge {nationname}
  * Requests the given nation to merge into your nation.
  * Can only be used by the nation king, and requires the king of the other nation to be online to accept the merger.
  * The soon-to-be-ex-king will receive a confirmation message asking if they will accept the dissolution of their nation.
  * If accepted the towns of the nation transfer to the remaining nation. The nation's bank money is also transferred.
* ranklist {nationname} - Displays residents and their ranks, optional nationname to view another nation's rank list.
* townlist (nation)
  * (nation) is optional, to show townlist of a nation you aren't a part of.
  * lists all towns in a nation.
* allylist (nation)
  * (nation) is optional, to show allylist of a nation you aren't a part of.
  * lists all allies of a nation.
* enemylist (nation)
  * (nation) is optional, to show enemylist of a nation you aren't a part of.
  * lists all enemies of a nation.

## /invite

* Shows subcommands.
* ?|help - Shows subcommands.
* list - Shows a list of invites you have received from towns.
* accept {town} - Accepts an invite to join a town.
* deny {town} - Denies an invite to join a town.
* deny all - Denies all of a player's received town invites.

## Chat Commands

* /tc
  * Put in from of text to speak with members of your town only, or without text afterwards to enter the channel.
* /nc
  * Put in from of text to speak with members of your nation only, or without text afterwards to enter the channel.
* /ac
  * Put in from of text to speak with members of your nation and your nation's allies, or without text afterwards to enter the channel.
* /g
  * Put in from of text to speak in globalchat, or without text afterwards to enter the channel.
* /l, /lc
  * Put in from of text to speak in localchat, or without text afterwards to enter the channel.
* /res set mode reset
  * Reset chat mode to default chat.
* /channel leave|join {channel} - Channel leaving and joining.
* /ch list - list what channels a player is currently listening to. Courtesy of Yaiyan.
* /leave {channel} - Leaves a channel.
* /join {channel} - Joins a channel.
* /chmute {channel} {player} - Mutes a player in a channel.
* /mutelist {channel} - Displays mute list for a channel.
* /chunmute {channel} {player} - Unmutes a player in a channel.
