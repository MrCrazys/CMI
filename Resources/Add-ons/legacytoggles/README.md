# :star: 1MoreBlock.com CMI Add-on

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Legacy CMI Toggle Commands / Aliasses

This is a `CMI CustomAlias` add-on made by Floris, for CMI 9.7.5.5 or newer, and Minecraft 1.21.x

1MB Legacy Toggles are a helper to get the old CMI Commands back that were removed in 9.1.4.x. This allows a server owner to offer the set of familiar old legacy commands and their aliases to their players again. 

Where possible, these will try to toggle. They are purposely limited, and with purpose display that things have moved to /options. This is because I personally feel that players can simply be told to use /options moving forward. You're of course free to completely revamp how these work on your server. Consider these merely a courtey solution, and / or an example to start with.

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Permissions

By default, the permissions are not per alias command. They do however require the player to have the appropriate `cmi.command.options`, and `cmi.command.options.[types]` permission nodes.

```
cmi.command.options - Modify personal options

cmi.command.options.[visibleholograms/shiftsignedit/totembossbar/bassbarcompass/tagsound/chatspy/cmdspy/signspy/acceptingpm/acceptingtpa/acceptingmoney] - Allows to modify specific options

Optionally (for team members)
cmi.command.options.others - Modify personal options, of others.
```

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Prerequisites

Okay, **let's get started**. Thank you for being interested in this little add-on.

Make sure your Spigot or Paper jar is up to date and at least 1.18.2, as well as CMI / CMILib. And of course backup everything before making changes. We also assume you've updated `Alias.yml` to enable /options, and that you've given players the appropriate permission nodes.

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Download Instructions

You only need the CMI add-on for this to work.

- :file_folder: (CMI Add-on) [1MB-old-toggle-commands.yml](/Resources/Add-ons/legacytoggles/1MB-old-toggle-commands.yml)


## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Installation Instructions

- Get the `.yml` file and open it in your favorite YAML editor. Such as Notepad++ on Windows or Sublime Text 4 on macOS. You cannot use a regular notepad or Microsoft Word.

- After some initial customizing or perhaps adding any permission requirements, you could delete the commands you don't wish to use. And/or add more to your liking.

- You can now start adding the Options permissions to the appropriate groups.

- Next, add the CMI file into the `~/plugins/CMI/CustomAlias/` folder, so you get: `~/plugins/CMI/CustomAlias/1MB-old-toggle-commands.yml` and type `/CMI reload`.

- Ideally, to properly register all these commands I do recommend to `/stop` the server, and start it again. Just a /cmi reload will work, but the commands will show red until you restart.

- Don't forget if you already have mapped or made any of these legacy commands, to either remove them from that location, or remove them from this file. 

You can now go into the game and try out the commands.

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> How to use this 1MB-Addon .yml file?

You can open it in your favorite editor, make changes accordingly. You can also in-game edit and delete commands, or even add more. 

This video shows you a bit more behind the scenes: PENDING

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> How to use the CMI Alias.yml file?

You can map all `/CMI <command>` commands as `/<command>` by editing the `~/plugins/CMI/Alias.yml` file. Full info and instructions can be found here: <https://faq.CMI.support/commands>. And you can find an alternative alias file with every command enabled by default, here: <https://github.com/mrfdev/CMI/blob/master/Resources/Alternatives/Alias_true.yml>

Note that any command NOT coming default by CMI cannot be added to Alias.yml, you have to use the `/cmi aliaseditor`, this add-on adds those old legacy commands for you. Yay.

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> Contributions?

You're more than welcome to offer fixes, contributions, adjustments, suggestions. Feel free to clone and make a pull request. We can discuss and review your contributions and probably merge them into the main branch. 

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> TODO

- I've added the ten removed commands, but should I add a command toggle for visible holograms?

- Request zrips to add a placeholder for tagsound True/False, so we can complete /tagtoggle

- Some commands probably benefit from a perm:check! first, so we can return a custom 'no permission'?

- add support for first param - `check:$1!=null` and then run `asPlayer!` options if `$1` is an online player `ifonline:$1!`

## <g-emoji class="g-emoji" alias="information_source" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/2139.png">ℹ️</g-emoji> The reason for this Add-on

With CMI 9.1.4.x some GUI menu updates have been introduced to match that of /homes, such as /kits, /warps, and now toggles have been moved to one as well, under /options.

Players keep asking on Discord how to get them back, I thought this will speed that process up for them. 

The changelog where this new /options first happened can be found [here](https://www.spigotmc.org/resources/cmi-298-commands-insane-kits-portals-essentials-economy-mysql-sqlite-much-more.3742/update?update=452373)

# Misc.

- Last updated on August 27th, 2024 | Version 1.2.0 build 012 (third public beta), by Floris
