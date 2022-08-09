---
layout: post
title:  "Backing up Acorn Archimedes ADFS Floppy disks in 2022"
date:   2022-08-09 08:08:00 +0000
categories: retro computing archival archives preservation update
---

## Introduction

The Acorn Archimedes was launched in 1987 and the series continued into the 1990s. It doesn’t seem like that long ago, but if you’re in 2022 with boxes of old Acorn ADFS disks (and no working Archimedes hardware) what do you do?

## The problem

Hindsight is a wonderful thing, and searching online provides mostly information from a decade or more ago when many computers still had floppy disk drives, or interfacing with them was much easier. Although you can easily buy USB floppy disk drives quite cheaply on Amazon, these are of no use for reading legacy disk formats (they only work with PC HD/1.44 MB formatted disks). 

## The solution(s)

The main reason for writing this post is that Google does not turn up anything at all useful for anyone using modern hardware right now. The information I found was through asking a very helpful Acorn enthusiast on eBay and for some reason just doesn’t appear in search results.

So far I've found 3 recommendations that might work:
- Get another Archimedes and network it to a Raspberry Pi running RISC OS. Then copy the files over the network to USB storage.
- Get an old PC with an internal floppy and use OmniFlop (Windows) or mount and dd (Linux). 
- Get an old internal floppy (with 34 ribbon cable) and connect it to a current machine with USB via a device such as [Greaseweazle](https://github.com/keirf/Greaseweazle) or [KryoFlux](https://www.kryoflux.com/).

This [document from the Acorn Preservation Team](https://stardot.org.uk/forums/viewtopic.php?t=22514) is a goldmine of info.

The same approaches should also work for Amiga, Atari ST and other legacy formats.

## My approach
Even though the Greaseweazle is much cheaper and is recommended by the Acorn Preservation Team over the KryoFlux, I decided to go with the KryoFlux. The main reasons for this were that I wanted the convenience of using a well established project with good user support, Mac software with a GUI and all the required cables and power supply included. Sometimes it’s worth spending money to save time and my main motivation was to declutter my home office of decaying legacy disks, but also quickly enjoy accessing my old Acorn disks on my current computer (MacBook M1 Air running [RPCem](#)). Other than the KryoFlux [insert name of pack], the only other thing I had to buy was an old internal floppy (with 34 ribbon cable). As I was going to be working with ADFS disks I bought a drive from an Acorn A3000, which is what the disks were originally written on. If you also have HD floppies you’ll need a drive that can handle them (the Archimedes only had a DD 800k drive (equivalent to PC 720k drive). I have some Akai sampler HD format disks so I may purchase an old PC floppy drive at some point too.

## The workflow
This is relatively simple with the KryoFlux. However, a detailed description will have to wait for another blog post &#8230;.




