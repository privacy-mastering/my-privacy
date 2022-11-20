---
description: disk encryption, antiviruses
---

# 💻 Laptops

#### Thoughts about data on your laptops

Let's review a situation where somebody has physical access to your laptop (or computer);

How it's possible? There are many options:

1. You lost your device (cafe, airport, it was stolen, etc..)
2. Somebody had access to a laptop when you left it alone (at home/work/cafe)

And you may ask – what is the danger if you locked access to your account with a password?

Answer – everybody is accessing all data on a computer's disk by default, seriously!\
If you did not encrypt all your disks – your laptop on the other hand just like a big flashcard

How to check yourself:

1. Create a Live USB with any operating system
2. Load your computer from this flashcard
3. Find your disk and... get any data

Looks easy? And there is!

You may find a demo on youtube, for example, the first link [https://www.youtube.com/watch?v=yI6RRBrhdh4](https://www.youtube.com/watch?v=yI6RRBrhdh4)

{% embed url="https://www.youtube.com/watch?v=yI6RRBrhdh4" %}

And pay attention to one fact: your password does not have any effect:

1. Everybody can read all data on your disk (all your photos, I believe)
2. Even if you protected all your online accounts with passwords and 2FA, but your data on laptops are not encrypted – everybody who received access to your computer can gain control of your online accounts (Facebook/Gmail/bank, etc...)
3. thus, if you lose your laptop with an unencrypted drive, you have to worry about what will fall into the hands of whoever finds the laptop

I am convinced that one of you does not want some of your photos or documents, or conversations in messengers to be in the wrong hands

So, let's review how to be

1. you have to encrypt your laptops
2. and if you lost your device – just worry about the device, not about the data on it, because the encrypted device is the only device (without readable data)

### Disk encryption

#### Windows

There are two windows versions: The home version and the Pro+ versions&#x20;

The main difference is – The home version does not provide good disk encryption (before windows 11 does not provide any disk encryption, except in cases when you decided to encrypt concrete folders by extension properties)

Pro+ versions provide encryption by TPM module (a chip on your laptop)

So, If you're are lucky – you may just turn on a Bitlocker, read more here [https://www.windowscentral.com/how-configure-bitlocker-encryption-windows-11#config\_bitlocker\_home\_windows11](https://www.windowscentral.com/how-configure-bitlocker-encryption-windows-11#config\_bitlocker\_home\_windows11)

But if you have a Windows Home version and want full disk encryption without buying Windows Pro – I recommend using a free solution `VeraCrypt` [https://www.veracrypt.fr/en/Downloads.html](https://www.veracrypt.fr/en/Downloads.html)

And remember – if you will lost your password you lost data on your disks, so please backup recovery keys and read all text during the disk encryption process

#### Mac OS

In the past, all MacBooks encrypted all drives with APFS (file system)

It means that all your data was not encrypted

So you have to check FileVault settings and turn It on if it's not, just read [https://support.apple.com/en-us/HT204837 ](https://support.apple.com/en-us/HT204837)

If you wanna read more go here [https://mactakeawaydata.com/apfs-vs-apfs-encrypted/](https://mactakeawaydata.com/apfs-vs-apfs-encrypted/)

Just a little notion: if you created a split disk volume – check its file system encryption and convert to the encrypted version if not

#### Linux

Unfortunately, there are many versions of Linux OS, so there is no common way to encrypt your disk after installation

At least you may backup your data and after – just format (erase) your drives with an encryption feature

#### VeraCrypt

Also you may use a VeraCrypt as an additional protection measure because it's a cross-platform solution that works with windows, macOS, Linux and works very fast

So, for good protection:

1. You have to encrypt your drive by default features of your OS
2. You may create an additional virtual volume by VeraCrypt to store their very sensitive data and connect this volume only when it necessary
3. As well VeraCrypt provides a hidden volume (like volume in volume) that hides your data event in the case when you have to disclose your passwords, read more here [https://veracrypt.eu/en/Hidden%20Volume.html ](https://veracrypt.eu/en/Hidden%20Volume.html)

### Antiviruses

Maybe you think that viruses are not about you, just because you use only browsers for surfing and downloading some games

But try to remember the virus WannaCry – your computer just has to be connected any time to network with one infected computer (wifi of a cafe, institute, hospital, office, hotel, etc...)&#x20;

But why your modern OS does not protect users against viruses fastly?

1. Sometimes there is no possibility to patch OS quickly
2. And users do not install OS updates/patches every day
3. Some users even turn off updates! Seriously! I saw it with my eyes
4. Some users use pirated software and... as you already know – cracked software in most cases infected by a botnet agent

Ok, I believe that you (a reader) are an honorable user and you wanna be protected in the Internet event in the case when your Os does not have patches

Antiviruses work today very fast, especially in the case when it's a built-in OS (like a Windows Defender), so If you have it – do not turn off them and their updates services

Because antiviruses update their bases every day (or more often) and even if your OS does not have patched your antivirus may have implemented a protection mechanism fastly

Oh, I forgot one interesting moment – do you share your laptop with someone else? A member of your family, or a friend? And some of them use a USB drive that has been in a school some time ago? I think you already understood that this case describes a threatment

Ok, I hope you already know that antiviruses are good and you need them, like soap or vaccines

And yes – maybe we do not meet any virus during whole our life, but better to be ready when it happens

Ok, what antivirus is good? There is no good answer, just try google:

1. Best Windows 10 antivirus for 2022 – [https://www.techradar.com/best/best-windows-10-antivirus](https://www.techradar.com/best/best-windows-10-antivirus)
2. The best antivirus software for your Mac in 2022 – [https://www.techradar.com/best/best-mac-antivirus-software](https://www.techradar.com/best/best-mac-antivirus-software)
3. About Linux – I used only Eset 32, works good
