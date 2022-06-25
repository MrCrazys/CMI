# FAQ - How can I use CMI Chat with Bungee?

<topMenu>
<details>
    <summary><strong>FAQ Menu</strong></summary>
    <p>
     • <a href="https://faq.cmi.support/bungee">Bungeecord-Info</a>, 
     • <a href="https://faq.cmi.support/chance">Chance-Example</a>, 
     • <a href="https://faq.cmi.support/chat">Chat-Manager</a>, 
     • <a href="https://faq.cmi.support/format">Chat-Format</a>, 
     • <a href="https://faq.cmi.support/chatfilter">Chat-Filter</a>, 
     • <a href="https://faq.cmi.support/chatrooms">Chat-Rooms</a>, 
     • <a href="https://faq.cmi.support/commands">Commands-Manager</a>, 
     • <a href="https://faq.cmi.support/joinleave">Custom-Join-Leave</a>, 
     • <a href="https://faq.cmi.support/economy">Economy-Manager</a>, 
     • <a href="https://faq.cmi.support/eventcommands">Event-Commands</a>, 
     • <a href="https://faq.cmi.support/ext-cmds">Extending-Commands</a>, 
     • <a href="https://faq.cmi.support/gettingstarted">Getting-Started</a>, 
     • <a href="https://faq.cmi.support/glow">Glow</a>, 
     • <a href="https://faq.cmi.support/help">Custom-Help</a>, 
     • <a href="https://faq.cmi.support/hexcolors">Hex-Colors</a>, 
     • <a href="https://faq.cmi.support/import">Importing-Data</a>, 
     • <a href="https://faq.cmi.support/library">CMILib</a>, 
     • <a href="https://faq.cmi.support/locale">Locale</a>, 
     • <a href="https://faq.cmi.support/prefix">LuckPerms-Prefix</a>, 
     • <a href="https://faq.cmi.support/migrate">Migrate-Database</a>, 
     • <a href="https://faq.cmi.support/mode-stuck">Mode-Stuck</a>, 
     • <a href="https://faq.cmi.support/moderation">User-Moderation</a>, 
     • <a href="https://faq.cmi.support/more-msg-cmds">More-Msg-Commands</a>, 
     • <a href="https://faq.cmi.support/motd">MOTD</a>, 
     • <a href="https://faq.cmi.support/params">Parameters</a>, 
     • <a href="https://faq.cmi.support/ranks">Ranks</a>, 
     • <a href="https://faq.cmi.support/rules">Custom-Rules</a>, 
     • <a href="https://faq.cmi.support/running">Running-CMI</a>, 
     • <a href="https://faq.cmi.support/safety">Safety-Tips</a>, 
     • <a href="https://faq.cmi.support/specialized">Specialized-Cmds</a>, 
     • <a href="https://faq.cmi.support/toggle">Toggle-Example</a>, 
     • <a href="https://faq.cmi.support/trash">Trash</a>, 
     • <a href="https://faq.cmi.support/votes">Vote-Manager</a>,
     • <a href="https://faq.cmi.support/worth">Worth</a>.
    </p>
</details>

<details>
    <summary><strong>Official Zrips Links</strong></summary>
    <ul>
        <li><a href="https://zrips.net/">Zrips Website</a>
         <pre>https://www.zrips.net/<br>The official website, wiki/documentation/information</pre></li>
        <li><a href="https://discord.gg/dDMamN4">Zrips Discord</a>
         <pre>https://discord.gg/dDMamN4<br>The official Discord community server with member-driven support</pre></li>
        <li><a href="https://github.com/Zrips/">Zrips Github</a>
         <pre>https://github.com/Zrips<br>The place for bug reports and feature suggestions</pre></li>
    </ul>
</details>

<details>
    <summary><strong>Prerequisites</strong></summary>
    <ul>
        <li><a href="https://www.spigotmc.org/resources/3742/">Buy and Download CMI</a> (premium plugin)
         <pre>https://www.spigotmc.org/resources/3742/<br>Get the CMI plugin if you haven't already, and then Install it on all your servers</pre></li>
        <li><a href="https://www.spigotmc.org/resources/87610/">Also Download CMILib</a> (free library) (<a href="https://github.com/mrfdev/CMI/edit/master/Resources/FAQ/cmi-library.md">more info</a>)
         <pre>https://www.spigotmc.org/resources/87610/<br>All Zrips plugins require the CMILib .jar file. Get it and also put it on all your servers.</pre></li>
        <li>All my FAQ pages have been written for Spigot / Paper 1.19 and CMI 9.2.0.x or newer.</li>
        <li>The mrfdev github page is not an official resource, we're building up our knowledge base as a courtesy.</li>
        <li>I am an admin on the Zrips Discord, this does not mean what I share on here is official.</li>
    </ul>
</details>
</topMenu>

---

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> CMI Chat + Bungee Chat

- Download and install CMI's BungeeCord jar on your proxy server (<https://www.zrips.net/wp-content/uploads/2021/09/CMIB1.0.1.0.jar>).
- Update the `config.yml` (see below).
```yaml
BungeeCord:
  # You can disable bungeecord support entirely if you are exrperiencing issues with it
  # When setting this to false some features like public messages over bungee cord, private messages over bungeecord, portals over bungecoord and other features will stop working
  # Keep in mind that regular behavior of those features will remain intacted
  Enabled: true
```yaml
You must also enable the following:
Chat:
  # Will try to modify chat to display it in defined format
  ModifyChatFormat: true
```
Additionally, you can also enable the following settings:
```yaml
  # Attention! This will require you to have CMI Bungee plugin which can be found at zrips.net
  # Or direct download https://www.zrips.net/cmi/
  # Do you want to enable private messaging over bungeecord
  BungeeMessages: true
  # Do you want to enable public messaging over bungeecord
  # Player needs to have cmi.bungee.publicmessages.[servername] permission node to be able to send messages to target server
  BungeePublicMessages: true
  # Do you want to enable staff messaging over bungeecord
  BungeeStaffMessages: true
```
Then walk through all the other options related to chat. 

Don't forget to set up appropriate permissions, such as:
`cmi.bungee.publicmessages.[servername]`


- And finally; `/stop` the server, and start it up again to guarantee that everything's working properly. More information on <https://www.zrips.net/cmi/>.

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Miscellaneous

**Placeholders:**
```
%cmi_user_bungeeserver%
%cmi_bungee_total_[serverName]%
%cmi_bungee_current_[serverName]%
%cmi_bungee_motd_[serverName]%
%cmi_bungee_onlinestatus_[serverName]%
```

**Commands and Permissions:**
```
/cmi bbroadcast (!) [message] (-s:[serverName,serverName])
-> cmi.command.bbroadcast - Sends special message to all players on all servers

/cmi msg [playerName] [message]
-> cmi.command.msg.togglebypass - Allows to send private messages even if player has pm toggled off
-> cmi.command.msg - Sends message to player
-> cmi.command.msg.[maingroupname].send - Allows to send private messages to specific player groups
-> cmi.command.msg.clean - Allows to send clean messages to player using ! at beginning
-> cmi.command.msg.noreply - Allows to send clean messages to player by using !- at beginning without option to reply
-> cmi.command.msg.vanish - Allows to send private messages to vanished players

/cmi options (playerName) (option) (enable/disable/toggle/status) (-s)
-> cmi.command.options.[visibleholograms/shiftsignedit/totembossbar/bassbarcompass/tagsound/chatspy/cmdspy/signspy/acceptingpm/acceptingtpa/acceptingmoney] - Allows to modify specific options
-> cmi.command.options.others - Modify personal options
-> cmi.command.options - Modify personal options

/cmi reply [message]
-> cmi.command.reply - Reply to last message sender

/cmi sendall [serverName]
-> cmi.command.sendall.bypass - Prevents player from being sent to target server
-> cmi.command.sendall - Send all online players to target server

/cmi server [serverName] (playerName) (-f)
-> cmi.command.server.others - Connect to bungeecord server
-> cmi.command.server - Connect to bungeecord server

/cmi serverlist
-> cmi.command.serverlist - Show server list
-> cmi.command.serverlist.others - Show server list
```
**Miscellaneous:**
```
-> cmi.bungee.publicmessages.[servername] - Allows to send public messages to target server
```

**Permissions:**
```
cmi.command.serverlist - Show server list
cmi.command.serverlist.others - Show server list
cmi.command.server.others - Connect to bungeecord server
cmi.command.bbroadcast - Sends special message to all players on all servers
cmi.bungee.publicmessages.spawn - Allows to send public messages to target server
cmi.command.sendall.bypass - Prevents player from being sent to target server
cmi.command.sendall - Send all online players to target server
cmi.command.server - Connect to bungeecord server
```

**config.yml:**
```yaml
  # Attention! This will require you to have CMI Bungee plugin which can be found at zrips.net
  # Or direct download https://www.zrips.net/cmi/
  # Do you want to enable private messaging over bungeecord
  BungeeMessages: false
  # Do you want to enable public messaging over bungeecord
  # Player needs to have cmi.bungee.publicmessages.[servername] permission node to be able to send messages to target server
  BungeePublicMessages: false
  # Do you want to enable staff messaging over bungeecord
  BungeeStaffMessages: false
```
Additionally, the following can be changed:
```yaml
BungeeCord:
  # You can disable bungeecord support entirely if you are exrperiencing issues with it
  # When setting this to false some features like public messages over bungee cord, private messages over bungeecord, portals over bungecoord and other features will stop working
  # Keep in mind that regular behavior of those features will remain intacted
  Enabled: false
  # When set to true player names from entire bungee network will be included into tab complete
  NamesInTabComplete: false
```

**Installation Instructions:**
- Buy a CMI license to use on your network, if you don't already have one.
- Install CMI on each individual server, except for the proxy.
- Get the CMI Bungee file and put it on the proxy only.
- Configure CMI, enable the CMI Chat, and enable BungeeCord using the instructions from this article.

I do not believe there's any `modules.yml` things that need to get enabled.

**FAQ:**

- If I run 3 servers and they're all on the same network, do I need three licenses?

No, a single license covers the entire network.

- Is the chat global?

Yes, the chat will show on all servers across your network.

- Can I synchronize money on all of my servers?

This is not currently possible. However, using a [plugin](https://www.spigotmc.org/resources/mysql-player-data-bridge.8117/) called MySQL Player Data Bridge, which supports synchronizing some of CMI's data across a BungeeCord network, this can be achieved by using the plugin on top of CMI.

- Can all of the warps synchronize across each of the servers?

No, this is unfortunately not possible using CMI.

- Can homes synchronize across each of the servers?

No. Like warps, this is unfortunately not possible using CMI.

- Can I use portals to teleport players to another server on the network?

Yes, this can be achieved using the portals system of CMI. More information about portals can be found [here](https://www.zrips.net/cmi/portals/).
- if i run 3 servers and they're all on the same network, do i need three licenses? no, from what i gather that license covers the network
- is chat global? yes
- can i sync up economy on all servers? no, probably not (mysql player-data bridge plugin supporst cmi though)
- can all the /warps be the same on all servers? no
- what about homes? no
- can i use portals to teleport ppl to another server on the network? yes
- can i use /server or /server the way i want? yes alias.yml (/cmi server) (there's also /cmi serverlist)
- if a command doesn't support running on another server, can i still send it? what? no, i dont think so
- if a command doesn't move a player to another server, can i still do it? no, but yes, with /cmi aliaseditor you can make your own command that uses /cmi server and/or placeholders.
- are my inventories shared between servers? i doubt it, you probably need a bungee-inventory plugin dedicated to this (mysql player-data bridge plugin supporst cmi though)
- can i use 1 database for all cmi instances? no, default is sqlite, use mysql, and make sure they all use a unique prefix. Using 1 user table for every server for example will very very very likely cause massive issues.
- i put CMIB jar on the proxy (bungeecord) but it did not make any files or folders? yes, i dont think it does. On your 'servers' on the network type: /cmi version, if bungee is hooked, it should show there. Again, cmi goes to the servers behind the proxy, cmib jar goes to the proxy server only.
```

MYSQL player data bridge (third party plugin i was talking about) <https://www.spigotmc.org/resources/mysql-player-data-bridge.8117/>

---

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> LATEST
Per CMI 9.0.4.3 this was in the changelog:
```
- Added better support for bungeeservers in the sense that now we can show custom messages when player switch servers to and from it. This will only works after you update CMIB plugin and only applies when you have custom login/logout messages enabled. New locale lines got added to CMI locale file
- Updating CMIB plugin will properly take player out of afk mode if he uses bungee only commands which previously would have been ignored
```

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Will CMIB help sync x y z?

At the moment the answer is probably no, it won't sync inventories, money, or things like warps and homes. Is there an interest by Zrips to add more support for this? Yes, from what I gathered there is. I have no ETA on this. 

Currently it's mainly for syncing public and private chats, staffmsgs, and to better support /cmi server, /cmi serverlist, and jumping through portals, and custom messages changing between servers. 

There's a third party (and unsupported) plugin on SpigotMC that claims to have support for CMI, <https://www.spigotmc.org/resources/mysql-player-data-bridge.8117/>

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Velocity Support

There's currently no Velocity support. A comment below a review had Zrips confirm that it's in the works. I have no ETA for this. 

People have said they are using Snap to get CMI / CMIB combo working on Velocity as well. You need to put the CMIB jar in the plugin directory inside the snap directory, I believe.


