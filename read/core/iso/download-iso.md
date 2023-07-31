---
title: Download ISO
nav_order: 1000
has_children: false
parent: ISO
---


# Download ISO


## Debian 12

* Debian / News / [Debian 12 "bookworm" released](https://www.debian.org/News/2023/20230610)
* Debian 12 / [Release Notes](https://www.debian.org/releases/bookworm/releasenotes)
* Debian / [Live install images](https://www.debian.org/CD/live/)
* [https://cdimage.debian.org/debian-cd/](https://cdimage.debian.org/debian-cd/)
* [https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/](https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/)


## 下載腳本

* [下載腳本](https://github.com/samwhelp/debian-adjustment/blob/main/core/iso/boot-iso/boot-iso-by-grub/demo-boot-debian-12-iso/iso-download.sh)


## 下載點

> 可以到「Debian / [Live install images](https://www.debian.org/CD/live/)」找到下載點。

> 例如可以找到「[https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/](https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/)」。





## 下載方式

### iso-download.txt

先產生一個檔案「iso-download.txt」，內容如下

```
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-12.1.0-amd64-xfce.iso
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-12.1.0-amd64-mate.iso
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-12.1.0-amd64-cinnamon.iso
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-12.1.0-amd64-kde.iso
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-12.1.0-amd64-gnome.iso
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-12.1.0-amd64-lxqt.iso
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-12.1.0-amd64-lxde.iso
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-12.1.0-amd64-standard.iso
```

### iso-download.sh

接著執行下面的指令，就會下載剛剛「iso-download.txt」裡面所列的檔案

``` sh
wget -c -i iso-download.txt
```

> 關於「-c」指的是續傳

> 關於「-i iso-download.txt」，指的是下載「iso-download.txt」裡面所列的檔案


## Boot ISO

> 簡單「[驗證](#驗證)」過「下載完成的ISO檔案」，接下來可以選擇不同的「[Boot ISO](https://samwhelp.github.io/note-about-debian/read/core/iso/boot-iso.html)」方式。



## 驗證
