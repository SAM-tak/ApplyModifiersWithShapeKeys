# Apply Modifiers With Shape Keys

> Read this in other languages: [English](README.md), [日本語](README.ja.md).

## About

Blender addon for applying modifiers with respecting shape keys.

Updated to support Blender 2.80 or higher from founder [mato.sus304](https://sites.google.com/site/matosus304blendernotes/home)'s original version.

## Usage

### Install

- Download zip archive from Release tab of github site.

- Press install button on addon panel of blender's preference window and choose just downloaded zip file.

- Enable 'Apply Modifiers With Shape Keys' addon.

Then, added 'Apply all modifiers' and 'Apply selected modifier' menu items into *Object > Apply* menu.

Select mesh object, and choose added menu item from *Object > Apply* (Ctrl + A) menu.

Blender's default apply function can't apply mirror modifier if mesh has shape keys, but this addon can apply in theese cases.

If mesh has no shape key, this addon works same as default function. No advantage for no shape key mesh object.

### Apply all modifiers with shape keys

You can apply all modifiers with one click.

### Apply selected modifier with shape keys

You can apply specified modifier with respecting shape key this function.

### Limitation

This addon behave to clone mesh object each shape keys, and apply modifiers each clone, and reconstruct shape keys.

Then, if modifier changes vertex count and coresponding vertex in shape key is unknown, this addon just skip reconstruction applicable shape key.

In this case, result will have wrong shape key.

## Licence

[GNU GENERAL PUBLIC LICENSE (v2)](LICENSE)
