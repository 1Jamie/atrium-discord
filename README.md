# atrium-discord

Chat plugin for [Atrium](https://github.com/1Jamie/Atrium). It is not shipped inside Atrium. Current prerelease is **0.4.0**, aimed at Atrium `0.5.0-devel`.

It uses Atrium's helpers `lib/plugin_secret.js` (token file and keyring lookup) and `lib/ghostty_runtime.js` (`ghosttyEmbedArgs`) from the installed `ATRIUM_ROOT`. Discordo itself stays at `~/.local/bin/discordo`.

## Install

Install Atrium first so `atrium` is on `PATH`. Then, from the [0.4.0 prerelease](https://github.com/1Jamie/atrium-discord/releases/tag/v0.4.0) zip:

```bash
atrium --install-plugin discord-sidecar-0.4.0.zip
```

A directory works the same way:

```bash
atrium --install-plugin /path/to/atrium-discord
```

That copies the plugin to `~/.config/lotus-atrium/plugins/discord-sidecar` and marks it as a user plugin, so it is the one Atrium loads. Remove it with:

```bash
atrium --remove-plugin discord-sidecar
```

From an Atrium checkout, `npx atrium-dev install plugin <dir|zip>` does the same copy.
