# ★ 3D Spinning ASCII Hachiware (ハチワレ) ★

A full 3D spinning terminal animation of **Hachiware** from *Chiikawa*, rendered entirely in shaded ASCII characters with 24-bit TrueColor ANSI output! Inspired by ai_caliber's viral ASCII Usagi animation.

---

## Features

- **Accurate 3D Character Model**: Faithfully reconstructs Hachiware from the Chiikawa illustration:
  - Triangular sky-blue cat ears (`#89B5CA`)
  - Parted blue forehead bangs matching the kanji **「八」** (*hachi*)
  - Chubby pure-white body
  - Jet-black eyes with sparkling white pupil highlights (`W`)
  - Blushing cheeks with cute tick marks (`%` and `/`)
  - Open cat mouth with rose-pink tongue (`o`)
  - 3D curved blue cat tail attached to the lower-left back
- **Viral HUD Display**: Matches the viral video overlay:
  - `hachiware.py - ascii` / `hachiware.py - spiderman`
  - `rotation <deg>°` with dynamic `puri 1` trigger when facing backwards (showing the cute butt & tail!)
  - Real-time `letters` counter
  - Yellow elapsed timer (`● xx.xxs`)
- **Spider-Hachiware Mode (`[s]`)**: Transform Hachiware into a superhero in a scarlet-red and navy-blue spider suit with custom spider-webbing and mask eyes!
- **Dynamic Terminal Auto-Fit**: Automatically sizes and centers Hachiware to fill your terminal window cleanly.
- **Rich Interactive Controls**: Rotate, pause, tilt, zoom, and switch modes on the fly.

---

## Quick Start

Run directly with Python 3 (requires `pillow` and `numpy`):

```bash
cd Hachiware_Spin
python3 hachiware.py
```

Or from the workspace root:

```bash
python3 Hachiware_Spin/hachiware.py
```

### Launch Options

| Flag | Description |
|---|---|
| `python3 hachiware.py` | Default smooth auto-spinning animation (~35 FPS) |
| `python3 hachiware.py --big` or `-b` | Launch in **Big Mode** (1.35x zoom) |
| `python3 hachiware.py --huge` or `-H` | Launch in **Huge Mode** (1.65x zoom) |
| `python3 hachiware.py --spiderman` or `-s` | Launch directly into **Spider-Hachiware** mode |
| `python3 hachiware.py --zoom <val>` | Custom zoom multiplier (e.g. `--zoom 1.5`) |
| `python3 hachiware.py --yaw <deg>` | Start at a specific rotation angle (e.g. `--yaw 180`) |
| `python3 hachiware.py --snapshot` | Render a single frame snapshot and exit |

---

## Interactive Controls

| Key | Action |
|---|---|
| `[Space]` | **Pause / Resume** auto-rotation |
| `[s]` | **Toggle Spider-Man Mode** ↔ Classic Hachiware |
| `[b]` | **Toggle Big Mode** (enlarge / reset) |
| `[+]` / `[=]` | **Zoom In** |
| `[-]` / `[_]` | **Zoom Out** |
| `[0]` | **Reset Zoom** to default (1.0x) |
| `[a]` / `[d]` | **Rotate Left / Right** (or adjust spin speed while spinning) |
| `[w]` / `[x]` | **Tilt Pitch Up / Down** |
| `[r]` | **Reset** rotation, pitch, and zoom |
| `[q]` or `[Esc]` | **Quit** safely restoring terminal |
