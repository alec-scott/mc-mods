# Yearn for the Mines

Minecraft 26.1.2 · Fabric 0.19.5. Your mods update themselves every time you press Play.

## One-time setup (about 5 minutes)

1. Install [Prism Launcher](https://prismlauncher.org/download/) and sign in with your Microsoft account.
2. Download **[the instance zip](https://github.com/alec-scott/mc-mods/raw/main/prism/mc-mods-prism.zip)**.
3. In Prism: **Add Instance → Import → Browse**, pick the zip, then **OK**.
4. Double-click **Yearn for the Mines**. A small window downloads the mods, then the game starts.
5. Multiplayer → Add Server → use the address you were given.

That's it. When the pack changes, the next launch picks it up automatically.

You can add your own client-only extras (minimaps, shaders, etc.) in Prism under **Edit → Mods**. They won't be removed by updates.

## When the Minecraft version changes

Prism doesn't change the Minecraft version for you. If the server moves to a new version (it's **26.1.2** now):
select the instance → **Edit → Version** → click **Minecraft** → **Change version** → pick **26.1.2** → close, then press Play.
The mods switch over by themselves on that launch. (Or delete the instance and import the zip again.)

## If the zip doesn't work: manual setup

1. Prism: **Add Instance → Vanilla**, choose Minecraft **26.1.2**, then **OK**.
2. Select the instance → **Edit → Version → Install Fabric** → choose **0.19.5**.
3. **Folder** button (top right) → open the `.minecraft` (or `minecraft`) folder and put
   [packwiz-installer-bootstrap.jar](https://github.com/packwiz/packwiz-installer-bootstrap/releases/latest/download/packwiz-installer-bootstrap.jar) in it.
4. **Edit → Settings → Custom commands** → tick the box, and set **Pre-launch command** to:

   ```
   "$INST_JAVA" -jar packwiz-installer-bootstrap.jar https://raw.githubusercontent.com/alec-scott/mc-mods/main/pack.toml
   ```

## Troubleshooting

- **"Mod mismatch" / can't join:** close the game and press Play again so it re-syncs.
- **Update window shows an error:** check your internet and press Play again. If it keeps failing, message the server admin.
