---
layout: post
title: How to Reclaim/Make Space on Mac
order: 6
---

## Automated 

You can use [CleanMyMac](https://macpaw.com/cleanmymac). It also helps you to uninstall Applications along with removing their residual files:

* Run a system scan and free up space
* Uninstall Applications using CleanMyMac
* Some Applications/Softwares might not be detected completely using CleanMyMac. Example: [R](https://osxuninstaller.com/uninstall-guides/uninstall-r/)

## Manual 

The key to manually freeing up space, is to figure out where is a sizable portion of your hard disk space getting used up. There are some HDD space visualization softwares which will help you do just that. 

Suggestions for HDD Space visualization softwares: 

* [Disk Inventory X](http://www.derlien.com/downloads/index.html) (Free and Open Source)
	![Disk Inventory X]({{ site.baseurl }}/images/DiskInventoryX.png)
* [DaisyDisk](https://daisydiskapp.com/) (paid)
	![Daisy Disk]({{ site.baseurl }}/images/DaisyDisk.png)

## Misc

* Homebrew
    * [Clean Up Brew](https://stackoverflow.com/questions/27508590/homebrew-size-of-cellar). Check size of cleanup using `brew cleanup -n` and `brew cleanup` to perform it.
    * Check the size of Cellar (where homebrew installs) by using `du -sh /usr/local/Cellar`
* Check iMovies files in `~/Movies/iMovie Library`. I happened to find 7 GBs just lying there from old resources which I no longer needed :)