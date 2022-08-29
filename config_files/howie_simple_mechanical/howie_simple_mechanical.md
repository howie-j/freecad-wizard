# Howie's Simple Mechanical Configuration
This configuration is is customized to suit mechanical CAD workflows centered around PartDesign. It's especially recommended for users coming from commercial low to mid-end CAD systems such as Fusion360 or SolidWorks, or new users trying FreeCAD for the first time.

### Rationale
Toolbar icons should be quick and easy to find, and only tools that are used almost every time FreeCAD is used should deserve a spot on the toolbar. Searching a cluttered toolbar for a tool by hovering the mouse over and reading the tool tips is extremely ineffective, and the superfluous icons distract the designer and makes it harder to quickly find the tool you are searching for.

The file menu on the other hand should include all tools for the current workbench, with the tool name displayed in a convenient and easy to search list.  

![*Finding tools is quick and easy using the often forgotten file menu*](screenshots/file_menu.png)  

### Screenshots
![*PartDesign on 1080p monitor*](screenshots/1080p_partdesign.png)  

![*Sketcher on 1080p monitor*](screenshots/1080p_sketcher.png)  

![*PartDesign on 1440p monitor*](screenshots/1440p_partdesign.png)  

![*Sketcher on 1440p monitor*](screenshots/1440p_sketcher.png)  

### Modified Settings
- Advanced/less used toolbars are hidden and a few custom toolbars are created
- The toolbar is now a single line (only PartDesign and Sketcher are modified)
- Icon size *Large* on 1440p, *Medium* on 1080p
- TreeView and Comboview are split on 1440p, combined on *1080p*
- PartDesign is the default startup workbench
- New Document is created on startup
- Mouse mode: *Blender* (personal preference, might not be suitable)
- *Turntable* and *Drag at object center* navigation
- Auto refine in PartDesign
- Auto remove redundant in Sketcher

### Notes
- Reference plane in PartDesign should be a dropdown menu with point, line and LCS selectable.
- Techdraw is not properly configured
- FEM is not properly configured
- A better measure tool with a single icon should be included in master. [My suggestion is Asm4_Measure.](https://forum.freecadweb.org/viewtopic.php?f=8&t=68243)

### Test on Linux
1. Create a backup of your
`[/.config/FreeCAD]` and `[/.local/share/FreeCAD]` folders.

2. Delete the following folders:  
`[/.local/share/FreeCAD]`  
`[/.cache/FreeCAD]`  
`[/.cache/qtshadercache-x86_64-little_endian-lp64]` (might not be necessary)  
`[/.cache/mesa_shader_cache]` (might not be necessary)  

3. Delete the content of this folder: `[/.config/FreeCAD]` and copy `FreeCAD.conf` and `user.cfg` into it.

### Test on Windows
Follow the same procedure as on linux, except you will find your config files in `C:\Users\USERNAME\%APPDATA%`
