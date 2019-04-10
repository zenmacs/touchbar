# The zenmacs BetterTouchTool touchbar settings

This repo contains a BTT touchbar preset, apt for both general macOS usage, and Emacs usage.

The selling points are:

* Big, padded Esc key
* Emacs shortcuts that only show up for Emacs
  * You are free to remove the Emacs layer, or to customize it, taking inspiration from it.
* A consistent layout: the two 'layers' are toggled, without wobbling.

This is how it looks like:

**Global**

<img width="1085" alt="Touch Bar Shot 2019-04-10 at 18 45 42" src="https://user-images.githubusercontent.com/1162994/55897510-f09a4000-5bc0-11e9-82de-d49932f3c269.png">

> br stands for brightness, prev for previous (track), pp for play/pause (track), next for next (track).

**Emacs**

<img width="1085" alt="_" src="https://user-images.githubusercontent.com/1162994/55897295-897c8b80-5bc0-11e9-9c2a-5ac2c2bc6d2e.png">

> The left half keeps its meaning and functionality, the second one adds Emacs-specific commands.

> You'll certainly want to rename + remap the Emacs half: those Emacs shortcuts are not universal at all.

### Why no fancy icons for brightness, volume, etc?

Apple icons are copyrighted, and I can't be bothered to script some solution that fetches them from my computer and makes them available to BTT. There are some git repos similar in scope, but those package copyrighted material.

---

After import, the BTT menu will look like this:

**Global**

![image](https://user-images.githubusercontent.com/1162994/55897533-fe4fc580-5bc0-11e9-97bb-40359d82b65f.png)

**Emacs**

![image](https://user-images.githubusercontent.com/1162994/55897016-ffccbe00-5bbf-11e9-83b1-3a66e86b8305.png)

## Installation

* **First, backup all your settings**.

Hit `Export Highlighted` here:

![image](https://user-images.githubusercontent.com/1162994/55897701-4a9b0580-5bc1-11e9-8c69-e073924437a3.png)

When prompted, choose to backup all your settings.

* **Now, you can import this repo's preset**.

Using the same menu as before, choose `Import`.

## Emacs config explained

The Emacs commands (which have abbreviated names so they fit in the touchbar) simply map to `F7`, or `Control + F7`, etc. My .emacs.d [listens](https://github.com/zenmacs/.emacs.d/blob/master/lib/non-submodules/vemv.shortcuts.global.el) to those shortcuts.

## Debugging

The preset is a plain JSON file, which you can read and eventually edit.
