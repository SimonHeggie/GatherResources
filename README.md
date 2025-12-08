# Gather Resources — the Blender way to collect your project’s media

Collect / assemble / gather all external resources into a single folder with one click.  
Or, in plain English: **GET YOUR SHIT TOGETHER.**

<img src="GatherResources.png" width="420">

Early testing shows it handles most production scenarios correctly —  
but as always: **Make back-ups if testing with major productions.**

---

## What This Add-on Does

**Gather Resources** scans your Blender project for:

- VSE video strips  
- Audio strips  
- Image textures  
- Images used in materials  
- Cache files (e.g., mesh sequence caches)  
- Other external media referenced by your `.blend`

Then it copies all discovered files into a local `textures/` directory beside your `.blend` file.

It’s basically **After Effects Collect Files**, but for Blender.

---

## How to Use

Once installed and enabled:

**File → External Data → Gather Resources**

Blender will create a `textures/` directory beside your `.blend`,  
and copy all referenced external files into it.

A summary of collected files will appear in the status bar.

---

## Roadmap (Speculative)

### Alpha (Current Phase)
- Avoid duplicate file creation by checking size+mtime before copy  
- Smarter detection of duplicate files already present  

### Beta
- Confirm full cross-platform behaviour (Linux, Windows, macOS)  
- Stabilise overwrite and conflict-resolution logic  

### Production / Stable
- Full bug elimination  
- Hardened reliability for archiving, backup, and project transfer  

### Future Ideas
- **Auto-Gather Mode** (toggle to run after saving or before rendering)
- **Gather Proxy / Cache Data** into a separate folder  
- **Distribute Resources**  
  - Opposite of Gather — restore files to original locations using stored mappings  
- **Cleanup Mode**  
  - Identify unused files  
  - Warn if other `.blend` files share dependencies  
  - Remove unreferenced assets for archiving  
- **Menu streamlining** (collapse Pack + Gather tools under one section)

---

## Reporting Bugs

This add-on is new and will absolutely have bugs.  
Any testing you can provide is appreciated.

Submit issues here:  
https://github.com/SimonHeggie/Blender-GatherResources/issues

Please use the template below:

---

### 🐛 Bug Report Template

#### 1. Summary of the Issue
What went wrong?  
What did you expect to happen?

#### 2. Steps to Reproduce
1. Open Blender (include version).  
2. Set up scene with videos/images/audio/cache/etc.  
3. Run Gather Resources.  
4. Check the `textures/` directory.

#### 3. Expected vs. Actual Behaviour
Expected:  
Actual:

#### 4. System Information
- OS:  
- CPU:  
- GPU:  
- RAM:  
- Blender Version:
- Gather Resources version:

#### 5. Files and Formats Involved
Which types were present and which failed?

- Video (.mp4, .mkv, etc.)  
- Image (.png, .jpg, etc.)  
- Audio (.wav, .mp3, etc.)  
- Alembic (.abc)  
- Models (.fbx, .obj, etc.)

#### 6. Errors or Console Output
Paste any error messages or logs.

#### 7. Attempts to Fix / Workarounds (If Any)
What have you already tried?

#### 8. Additional Context
Does it happen always, or intermittently?  
Project-specific or global?

---

## License
GPL-3.0-or-later  
© 2024–2025 Simon Heggie
