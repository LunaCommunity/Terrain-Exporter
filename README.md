# Luna Terrain Exporter

## Overview

The Luna Terrain Exporter is a tool that allows you to produce `.OBJ` format versions of your terrain in Unity. This intern allows Luna Playable developers to use this `.OBJ` file, along with the textures, to replace the unsupported terrain environment. 

## How to get started

1. Download & then import the Luna Terrain Exporter into your Unity project<br/><br/>
2. Make sure that the textures used for your terrain have the 'Read/Write Enabled' setting set to true in their import settings<br/><br/>
  ![alt-text](https://i.imgur.com/sSNolRV.png)<br/><br/>
3. Open the Terrain Exporter via the Unity Tools tab (the same place that Luna Playable is located) <br/><br/>
  ![alt-text](https://i.imgur.com/O7hoVza.png)<br/><br/>
  **If Luna Terrain Exporter displays "No terrain found" please make sure you have an active terrain in your Scene** <br/><br/>
4. Configure the [settings](#settings) to suit your needs (we recommend either 'Quarter' or 'Eighth' for the Resolution setting)<br/><br/>
5. Hit Export and a `.OBJ`, material, and `.png` will be created in a numbered folder at 'Assets/Luna Terrain Exporter/Exported files'<br/><br/>
  ![alt-text](https://i.imgur.com/I2A4xe1.png)<br/><br/>
6. You can now replace the terrain in your scene with this object (You will need to apply the exported material to the object after dragging it in)<br/><br/>

## Settings & Options

### Resolution

Set the resolution of the terrain vertices by fractions.

* Full
* Half
* Quarter (recommended)
* Eighth (recommended)
* Sixteenth

### Terrain texture resolution

Resolution size of the terrain textures in pixels.

* 512x512
* 1024x1024
* 2048x2048

### Tiling of the texture

This affects the amount of tiles within the terrain, if set too low the texture will appear stretched, too high and you may begin to lose detail.

* int value (Minimum of 1, no max value)

## Limitations

* As of now we currently only support the use of 4 or less textures in conjunction with this tool
* Vertices need to be under 65k, lower the Resolution setting to avoid this preventing exportation
* Currently we cannot export terrain with holes
