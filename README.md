# atrium-discord

Chat plugin for Atrium. It is not shipped inside Atrium. Atrium still provides `lib/discord_vault.js` and `lib/ghostty_runtime.js`; this plugin loads those from `ATRIUM_ROOT`.

Install into the user plugin directory (from an Atrium checkout, so `atrium-dev` is on the path):

```bash
cd /path/to/atrium-discord
npm install
cd /path/to/atrium
npx atrium-dev install plugin /path/to/atrium-discord
```

`bin/atrium` sets `ATRIUM_ROOT`, which is how the installed copy finds the vault and Ghostty helper. Discordo itself stays at `~/.local/bin/discordo`.
