# Install the token-saving mods on Mac

This is the copy we tested.

## What you need

- A Mac with macOS.
- Claude Code 2.1.287 or newer in the terminal, or 2.1.286 or newer in the desktop app.

Some mods can use more tools. They work without them.

- input-router reads PDFs only when Poppler is installed (`brew install poppler`), so that `pdftotext` works in a new terminal.
- research-router uses Firecrawl only when you install the Firecrawl command-line tool with npm, so that `firecrawl` works in a new terminal.
- efficient-browser-use makes pictures smaller with `sips`. It is already part of macOS.

## Steps

1. Unzip the pack. Put the `token-saving-mods` folder in your Downloads folder.

2. Open Claude Code.

3. Add the pack. Type this:

   ```
   /plugin marketplace add ~/Downloads/token-saving-mods
   ```

4. Install the mods. Type each line:

   ```
   /plugin install input-router@token-saving-mods
   /plugin install effort-optimizer@token-saving-mods
   /plugin install model-router@token-saving-mods
   /plugin install cache-clock@token-saving-mods
   /plugin install handoff@token-saving-mods
   /plugin install research-router@token-saving-mods
   /plugin install efficient-browser-use@token-saving-mods
   /plugin install mods@token-saving-mods
   /plugin install savings-proof@token-saving-mods
   ```

5. Load them. Type:

   ```
   /reload-plugins
   ```

6. Check them. Type `/mods`. The Mods pane opens and shows each mod. Type `/savings` to open the Savings Proof pane.

## If something goes wrong

- If `/plugin marketplace add` says it cannot find the folder, check the path. The folder you give must hold the `.claude-plugin` folder.
- If a mod does not work, turn it off in the `/mods` pane. The other mods keep working.
