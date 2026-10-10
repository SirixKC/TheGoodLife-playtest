# The Good Life: playtest builds

Downloads for the people helping test *The Good Life*. No job, no papers, one empty flat. This repository only holds the builds; the game's source isn't here.

## Download

**[Latest build](https://github.com/SirixKC/TheGoodLife-playtest/releases/latest)**: under *Assets*, take the Windows `.zip` or the Linux `.tar.gz`.

It's an unfinished prototype, so expect bugs: finding them is the point.

## Starting it

**Windows** (64-bit Windows 10 or 11)
1. Unzip the whole folder first (don't run it from inside the zip).
2. Double-click `TheGoodLife.exe`.
3. If Windows says *"Windows protected your PC"*, click **More info**, then **Run anyway**. The game isn't signed; that's all the warning means.

**Linux** (64-bit)
1. Extract the archive.
2. Run `./TheGoodLife.x86_64` (if it won't start: `chmod +x TheGoodLife.x86_64`).

The first start is slow: a minute or more on the Godot logo while the game builds its world and prepares your graphics card. Windows may say *Not Responding* during that time. Wait, don't close it. Later starts are quicker.

You need a graphics card with Vulkan (almost any card from the last eight years). If it won't start, update your graphics drivers and say what card you have. There's no Mac build.

## Controls

| Key | Does |
| --- | --- |
| Mouse | look |
| Left click | use what's in your hands (hit, cut, dig, pour...) |
| Right click | block; with bare hands, grab and carry loose things |
| W A S D | walk |
| Shift / Space | run / jump |
| C or Ctrl / Alt | crouch / dodge |
| E | use, pick up, open, talk (the screen tells you what) |
| 0–5 or mouse wheel | choose what's in your hands (0 = bare hands) |
| I | look over what you're holding |
| Tab / J / K / B | inventory / notes / crafting / build |
| Esc | menu (Quit saves your game, Continue picks it up) |
| F11 | fullscreen |
| **F8** | **playtest note** |

## Playtest notes: F8

Whenever something looks wrong, breaks, confuses you, or you just have an opinion, press **F8**.

- The game stops and keeps a screenshot of exactly what you see.
- Type what's wrong. A short note is fine ("this tree floats").
- Drag with the mouse to draw on the screenshot in red: circle the problem. Right click takes back the last stroke.
- **Enter** keeps the note. **Shift+Enter** starts a new line. **Esc** throws it away.
- The game carries on where it was.

Each note also records where you were and what was happening: your position and where you were looking, what you were aiming at, the time and weather in the game, who was nearby, and which build you're playing. Nothing is sent anywhere; the notes stay on your computer until you send them.

## Sending your notes back

The notes are in a folder called `playtest_notes`:

| | |
| --- | --- |
| Windows | `%APPDATA%\Godot\app_userdata\The Good Life\playtest_notes` (paste it into the address bar of a File Explorer window) |
| Linux | `~/.local/share/godot/app_userdata/The Good Life/playtest_notes` |

Inside, `INBOX.md` lists every note, and each note has a `.png` (the screenshot), a `_marked.png` if you drew on it, and a `.json` (the details).

Zip the whole `playtest_notes` folder and send it to whoever gave you the link. If you have a GitHub account you can also [open an issue](https://github.com/SirixKC/TheGoodLife-playtest/issues/new) here and attach the zip.
