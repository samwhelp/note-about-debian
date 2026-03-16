---
title: Download ISO
nav_order: 1000
has_children: false
parent: ISO
---


# Download ISO




## Debian 13

* Debian / News / [Updated Debian 13: 13.4 released](https://www.debian.org/News/2026/20260314)
* Debian / News / [Updated Debian 13: 13.3 released](https://www.debian.org/News/2026/20260110)
* Debian / News / [Updated Debian 13: 13.2 released](https://www.debian.org/News/2025/20251115)
* Debian / News / [Updated Debian 13: 13.1 released](https://www.debian.org/News/2025/20250906)
* Debian / News / [Debian 13 "trixie" released](https://www.debian.org/News/2025/20250809)
* Debian 13 / [Release Notes](https://www.debian.org/releases/trixie/release-notes/)
* Debian / [Live install images](https://www.debian.org/CD/live/)
* [https://cdimage.debian.org/debian-cd/](https://cdimage.debian.org/debian-cd/)
* [https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/](https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/)




## 下載腳本

* [下載腳本](https://github.com/samwhelp/debian-adjustment/blob/main/core/iso/boot-iso/boot-iso-via-grub/demo-boot-debian-13-iso/iso-download.sh)




## 下載點

> 可以到「Debian / [Live install images](https://www.debian.org/CD/live/)」找到下載點。

> 例如可以找到「[https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/](https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/)」。




## 下載方式


### iso-download.txt

先產生一個檔案「iso-download.txt」，內容如下

```
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-13.4.0-amd64-xfce.iso
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-13.4.0-amd64-mate.iso
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-13.4.0-amd64-cinnamon.iso
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-13.4.0-amd64-kde.iso
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-13.4.0-amd64-gnome.iso
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-13.4.0-amd64-lxqt.iso
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-13.4.0-amd64-lxde.iso
https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/debian-live-13.4.0-amd64-standard.iso
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


### sha256sum

* [man sha256sum](https://manpages.debian.org/bookworm/coreutils/sha256sum.1.en.html)

執行

``` sh
wget -c https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/SHA256SUMS

sha256sum -c SHA256SUMS
```

會看到類似如下的內容

```
debian-live-13.4.0-amd64-cinnamon.iso: OK
debian-live-13.4.0-amd64-gnome.iso: OK
debian-live-13.4.0-amd64-kde.iso: OK
debian-live-13.4.0-amd64-lxde.iso: OK
debian-live-13.4.0-amd64-lxqt.iso: OK
debian-live-13.4.0-amd64-mate.iso: OK
debian-live-13.4.0-amd64-standard.iso: OK
debian-live-13.4.0-amd64-xfce.iso: OK
```
