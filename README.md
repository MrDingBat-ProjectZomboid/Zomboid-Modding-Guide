# Project Zomboid Modding Guide
**_This document is very much a Work-In-Progress._**
## Read Me First!
* [Goto ToC](TOC.md)  

## Contents
* [About this guide](#about-this-guide)  
* [Overview](#overview)  
* [Required Tools](#required-tools-software)
* [Topics](#topics)

----------------------------------------------------------------------------------
----------------------------------------------------------------------------------

## Introduction

### About this guide
This guide is originally forked from [FWolfe/Zomboid-Modding-Guide](https://github.com/FWolfe/Zomboid-Modding-Guide). The guide has been split up into several documents. 
 
The goal of this guide is to have a one-stop-spot for how to mod TheIndieStone's [Project Zomboid](https://projectzomboid.com), covering all aspects of modding, tools required, tips and tricks, as well as tutorials, examples and useful code snippets.

Much of the current modding information is in outdated tutorials, scattered in forum posts, etc. Ideally by hosting a universal guide on Github, it can be collected all in one spot and anyone can contribute new information, corrections or updates as PZ's API changes over time.

This guide is not meant to be a tutorial (although will *contain* tutorials), but a reference for both new and experienced modders.

Contributions to this guide are more then welcome. However please read [Contritbuting](CONTRIBUTING.md) first.

----------------------------------------
### Overview
"Modding" is a vague term covering multiple areas. Many of these areas sometimes overlap but should be considered separate as they require different skill sets and knowledge.

#### Adding basic items and recipes
This can be done with little (or none) coding knowledge and minimal tools. Item and recipe definitions are inside standard .txt documents, although these txt files must conform to a specific syntax and style.  

#### Code changes, advanced items and recipes
Being able to add on to or edit Zomboid's code is a major bonus, and where the real power of mods comes in. PZ is coded in a mixture of Java (the main engine) and Lua (the moddable components).  
Knowledge of the [Lua programming language](https://www.lua.org/) is HIGHLY advised. You'll save yourself a lot of grief and effort learning Lua before diving into this area. Fortunately Lua is a simple language by design, and relatively easy to learn.  
The internet is scattered with tutorials.

#### 3d Models
For build 40 and below, 3d art for Project Zomboid primarily consists of weapon models and vehicles. At this time all 3d mods fall into one of these 2 types.  Models are in a custom .txt format.
The processes of exporting from your modelling app and importing in PZ is fairly simple, though initial positioning, scaling and rotation can take a bit of tweaking. Minor coding is required to tell Zomboid to load the custom models.

Build 41 is expected to bring additional 3d models such as clothing and static items used in timed actions, and a different model format.

#### Textures


#### Map Making

----------------------------------------
### Required Tools (software)
**_This section should describe the various software tools required for various areas, and provide url links for the more common software used_**

For the most part, you are free to use what ever tools you want. The exception is custom map creation, where you are currently limited to the tools released by TIS.

#### Text Editors:
Used in all areas of modding. [Notepad++](https://notepad-plus-plus.org) is often the preferred editor for windows OS's (it also runs amazingly well on linux with wine)

#### 3d Modelling:
Used for the creation of custom items, vehicles and weapons. [Blender](https://blender.org) is the common choice as its free, and import/export scripts for PZ's model format exist. Any 3d app can be used to make your models, with blender doing the final conversion.

#### Image Editor:
If your doing custom icons, textures, maps or 3d models you'll need one of these. Paint.NET, Photoshop and [GIMP](https://gimp.org) are the most used, but whatever supports the .png format will work.

#### Custom Mapping:

----------------------------------------
### Topics
* [Mod Structure](Mod_Structure.md)
* [PZ Scripts](PZ_Scripts.md)
* [Lua Coding](Lua_Code.md)
* [Lua Events](Lua_Events.md)
* [Lua Methods](Lua_Methods.md)  
* [Java Classes](JavaClasses.md)
* [Translations](Translations.md)  
* [Mapping](Mapping.md)  

----------------------------------------
* [Goto ToC](TOC.md)  
