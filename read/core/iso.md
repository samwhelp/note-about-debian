---
title: ISO
nav_order: 1000
has_children: true
---


# ISO




## 主題

| 主題 |
| --- |
| [Download ISO](https://samwhelp.github.io/note-about-debian/read/core/iso/download-iso.html) |
| [Boot ISO](https://samwhelp.github.io/note-about-debian/read/core/iso/boot-iso.html) |




## Live Account

> Source Code:

* Debian / live-config / [0030-live-debconfig_passwd](https://salsa.debian.org/live-team/live-config/-/blob/master/components/0030-live-debconfig_passwd)
* Debian / live-config / [0030-user-setup](https://salsa.debian.org/live-team/live-config/-/blob/master/components/0030-user-setup)


> 使用「Debian Live ISO」開機後，自動登入的帳號。

| Account  | Value  |
| -------- | ------ |
| Username | `user` |
| Password | `live` |


> 執行下面指令，更改目前登入帳號的密碼。

``` sh
sudo passwd $(whoami)
```


> 執行下面指令，移除目前登入帳號的密碼。

``` sh
sudo passwd -d $(whoami)
```
