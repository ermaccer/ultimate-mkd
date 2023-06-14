<p align="center"><img src=https://i.imgur.com/Hjf4Gsg.png></p>

<h1 align="center">Installation</h1>


# Requirements

- **MK Deception USA** (SLUS-20881) ISO, CLEAN - don't have any other mods or edits done to any files in the ISO.
- **PS2 Tools** (cdvdgen, iml2iso) [Download](https://mega.nz/file/lURTjBYL#cWe9ZIOVIfD5nmwfimwx632Sz-fn1E1DpZddcF9RjJs)
- **Any extracted UMKD version**


# Step by Step

## 1. Extracting ISO
If you use Windows 10 or newer, you should be able to open ISO contents by just
double clicking at the .ISO file. This will mount the ISO as a virtual drive.

Open up the newly mounted drive and simply move everything from the virtual drive to any folder (preferably create one just for UMKD stuff).


## 2. Building a new  ISO

Open "cdvdgen", it's a tool designed to create PS2 DVD and CD images from scratch, it CANNOT edit existing ones!

### CDVDGEN Steps
1. Once launched, select **Create new project**
2. Select **DVD-ROM Master Disc**
3. Go to **Volume tab**
4. Once in volume tab, fill the respective places with following data
   - Master Disc/Disc name: **SLUS 20881**
   - Master Disc/Producer Name and copyright holder: **MIDWAY**
   - Master Disc/License Area: **America**
   - Volume Identifier/Volume: **SLUS-20881**
5. Go to **Directory** tab
6. Start dragging files from your previously extracted folder onto this window. Make sure they end up in following order/hierarchy:
   - SYSTEM.CNF
   - NETR.OVL
   - NTGUI.ELF
   - SLUS_208.81 (**If using PS2 version of the mod, use the provided SLUS_208.81 file from the !PS2 folder instead of the extracted one**)
   - AREA51 (folder, can also be removed)
   - CNF (folder)
   - LICENSE (folder)
   - MODULES (folder)
   - MOVIEPS2 (folder)
   - NETGUI (folder)
   - SNDSPS2 (folder)
   - GAMER.OVL
   - LOADINGE.RAW
   - MKDA.PAK
   - MOVIER.OVL
7. Open **ASSETS** folder of UMKD.
8. In CDVDGEN **Directory** window, highlight **MKDA.PAK** and press delete or remove it using mouse
9. Drag  **MKDA.PAK** from **ASSETS** folder onto the **Directory** window
10. In CDVDGEN open **SNDSPS2** folder
11. Highlight **MSLASSET.MS2** and press delete or remove it using mouse
12. Drag  **MSLASSET.MS2** from **ASSETS** folder onto the current **Directory** window
13. Save the project with File->Save, keep it around in case you'd like to update the mod and save some time
14. Choose **Export iml file** from File menu and save it somewhere you can find
15. Close CDVDGEN


Now pen "iml2iso", it's a tool designed to convert the IML file listing into a working PS2 iso.

### IML2ISO Steps
1. Once launched, click the **...** button near IML file path
2. Locate your previously exported **IML** file from CDVDGEN and open it
3. Press **Start**
4. Wait till the ISO generation process is finished, the resulting .ISO file will be stored in the same path as selected .IML
5. Done


## Settings PCSXF2 UP

# Skip this section if you want to play this mod on PS2!

PCSX2F is a custom fork/edit of normal PCSX2 which comes with more RAM, plugins support and many other modding oriented features!

This tutorial will only cover the QT GUI version of PCSX2F! It also assumes you are familar enough with base PCSX2 usage such as game paths, bios config and more.

[Download Page](https://github.com/ASI-Factory/PCSX2-Fork-With-Plugins/releases)

Select **fork-PCSX2-windows-qt-x64-AVX2.zip** while downloading, if your cpu is older, select the SSE4 version.

Extract the new PCSX2 version into either a seperate folder, or update your old one - its fully up to date with regular PCSX2 all time time, no latest features are omitted.



Copy **MKDHook.elf** and **MKDHook.ini** from UMKD folder (not assets) into **PLUGINS** folder of the new PCSX2 installation.


## PCSX2F Configuration

There are some options that are required to change to make the mod fully work.

### Enable Advanced Settings
Go to Tools menu and select **Show Advanced Settings**, agree with the disclaimer

### Configuring UMKD

Right click on your UMKD iso entry (or if you want, you can also apply these configuration changes globally) and choose **Properties**.

Go to **Graphics->OSD** and untick **Warn About Unsafe Settings**.
Go to **Graphics->Rendering** and set **Blending Accuracy** to **Minimum**, this fixes some bright custom textures used by the mod.
In the same tab, I'd also recommend to set **Dithering** to **Off**.

Go to **Advanced** and set **Rounding Mode** to **Nearest**.


You are ready to play UMKD!

