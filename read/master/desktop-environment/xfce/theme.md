---
title: 佈景主題
nav_order: 3300
has_children: false
parent: Xfce
grand_parent: 桌面環境
---


# 佈景主題


## 參考設定

* [參考設定](https://samwhelp.github.io/rgaps-theme-collection/#style)


## Style

* Xfce / Docs / [Xfconf-query](https://docs.xfce.org/xfce/xfconf/xfconf-query)
* man [xfconf-query](https://manpages.debian.org/testing/xfconf/xfconf-query.1.en.html)

## RGapsBlendNoButtons Gruvbox

| Theme | Theme Name | Theme Dir Path |
| --- | --- | --- |
| xfwm-theme | [RGapsBlendNoButtons](#config-xfwm-theme-rgapsblendnobuttons) | [~/.themes/RGapsBlendNoButtons](https://github.com/samwhelp/rgaps-theme-collection/tree/rgaps-blend-nobuttons) |
| gtk-theme | [Gruvbox](#config-gtk-theme-gruvbox) | [~/.themes/Gruvbox](https://github.com/samwhelp/gruvbox-theme-collection/tree/gtk-theme-gruvbox) |
| icon-theme | [Gruvbox-Dark](#config-icon-theme-gruvbox-dark) | [~/.icons/Gruvbox-Dark](https://github.com/samwhelp/gruvbox-theme-collection/tree/icon-theme-gruvbox-dark) |
| cursor-theme | [breeze_cursors](#config-cursor-theme-breeze_cursors) | [/usr/share/icons/breeze_cursors](https://packages.debian.org/sid/all/breeze-cursor-theme/filelist) |


### config-xfwm-theme-RGapsBlendNoButtons

``` sh
xfconf-query -c "xfwm4" -p "/general/theme" -s "RGapsBlendNoButtons"
```

### config-gtk-theme-Gruvbox

``` sh
xfconf-query -c "xsettings" -p "/Net/ThemeName" -s "Gruvbox"
```


### config-icon-theme-Gruvbox-Dark

``` sh
xfconf-query -c "xsettings" -p "/Net/IconThemeName" -s "Gruvbox-Dark"
```


### config-cursor-theme-breeze_cursors

``` sh
xfconf-query -c "xsettings" -p "/Gtk/CursorThemeName" -s "breeze_cursors"
xfconf-query -c "xsettings" -p "/Gtk/CursorThemeSize" -s "24"
```
