# Savecraft Demo

Windows demo of **Savecraft**, save and load for multiplayer games in Unreal Engine 5.6 to 5.8: one component on any actor, per-player saves on dedicated servers, crash-safe files, slots with pictures, World Partition and EOS cloud. The demo is the plugin's own test map, packaged as a Shipping build with UE 5.8.

**Download:** [SavecraftDemo_Win64.zip](https://github.com/filipetessaro/savecraft-demo/releases/latest/download/SavecraftDemo_Win64.zip) (215 MB).
Windows 64-bit, DirectX 12. No engine needed.

Unzip it anywhere and run `SavecraftDemo.exe`. The map has 40 crates, each with the Savecraft Saveable component and two SaveGame variables, Coins and Health. Save, destroy a few crates, spawn new ones, change coins, then load: everything goes back as it was saved.

| Key | What it does |
|---|---|
| WASD + mouse | Fly |
| Left click | +10 coins on a crate (and +1 gold for you, saved with your player) |
| Right click | Destroy a crate |
| E | Spawn a crate |
| 1 2 3 | Pick a slot |
| F5 | Save the slot, with a picture of the view |
| F9 | Load the slot |
| Delete | Delete the slot |
| Esc | Quit |

**Two players:** one runs `Host.bat`, the other runs `Join.bat` and types the host's address (Enter for the same PC). On another PC, allow the game through the firewall. With other players connected, F9 loads in place and nobody is kicked; the host does the saving and each player keeps their own gold.

The slots are written to `%LOCALAPPDATA%\SavecraftDemo\Saved\SaveGames\Savecraft`.

Documentation: https://apps.tessaroapps.com/savecraft/docs/
Support: contato@tessaroapps.com
