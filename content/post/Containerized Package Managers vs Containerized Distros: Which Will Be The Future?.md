```php
title: "Containerized Package Managers vs Containerized Distros: Which Will Be The Future?"
date: 2023-04-30
description: "Containerization is the way but which option is more likely to be the feature?"
tags: ["Linux", "Containerization", "Intermediate", "Distros"]
categories: ["Linux", ]
```

Hello once again! Today we have a more intermediate subject in hand. Please enjoy!

---

#### What is Containerization?

Simply put, instead of installing software on your operating system directly, installing it in a sandbox environment.

And what is a sandbox? Well as the name suggests really, it's an isolated space in your computer that has no access to your real file system... Well at least most of it. 

Why use sanboxing though? Well let's say you installed an unofficial package (such as the packages from AUR/COPR/PPA's), there is no guarantee that that package is properly scanned. I mean sure there might be some automated scans while that person adds that package to its respected external repository but malwares and ransomwares change and become smarter day by day. So the only way you are 100% secure is to use such repositories with sandboxing.

So what's the catch? Well the catch is the disk usage. Because all the programs are in their own container you can have like 15 versions of the same dependency. Each container is to their own they don't interact with each other which is a good thing but like I said that creates the problem of using more space on your drive. I'd say if your total space is under 256GB's don't even think of touching containers.

Well now we got the definitions and reasons out of the way let us talk about our best sandboxing options that may take the Linux world by the storm!

---

#### Contestant One:  Containerized Package Managers:

Unlike your (non-containerized) system's default package manager, these package managers are created to be secure by default.

How can they manage that? Well simply by not using system libraries as dependencies and restricting the packages access to the operating system. Anything goes through these containerized package managers to contact the operating system so you can safely use your system.

What are my options? We got Flatpaks, AppImages and Snaps. I'll dissect them one by one. 

**Flatpaks:** In most cases best option out of the three big container package managers. Most of the software you want to use are available in FlatHub, which is a great repository for Flatpaks. Packages are rather recent and I personally use this option alongside with some AppImages. FlatHub is not a decentralized repository but certainly is a trusted one. Official packages are marked "Verified" so you can't go wrong with that. There is no payment method yet but it is a spoken idea nowadays, so everything is free with no donation option unfortunately.

**AppImages:** Decentralized packages with no one place to find them. AppImageHub is your best bet but even with that the amount of packages there doesn't compare with either Flathub or Snap Store. AppImage is in dire need of a centralized repositories but that's unfortunately not how it works. Still AppImages have really small footprint on your system. Which is a great thing however you need an external tool to update your AppImages. I do use AppImages when specific vendors only uses AppImage to distribute their programs.

**Snaps:** The one with the biggest footprint on your system. Somethings meant to go wrong with Snap since it's designed for server computers. They have an centralized and proprietary store called Snap Store and that is the only place you can get your snaps from as far as I know. I personally don't use them since everything I need is provided from Flatpaks and AppImages.

One note I should add is that most of the time these solutions ends up with programs that doesn't follow your system theme. There is a workaround with Flatpaks called Flatseal but I certainly hope this gets fixed soon.

---

#### Contestant Two: Containerized Distributions:

Unlike your average distros these are made specifically for containers in mind. Sure they do use non-containerized packages as well such as containers themselves, low level system libraries, the kernel and, in most cases window managers and desktop environments. However, years showed us that these sort of packages are certainly less vulnerable than your third party repos. These distros utilize Flatpaks, AppImages and Snaps time to time but plus to those they come with distro containers as well. So what are distro containers? Well basically put they are distros containerized within your distro without access to host distros system files and libraries. They have their own libraries and kernels locked up in the container yet they can be used as if there are a part of your system, so not that different from containerized package managers in that regard. 

So what are your options here? Well before that I must tell you about immutable distributions. An immutable distro is basically a distro that you simply can not change anything on the system layer. Because all of your system files are read-only. This is a time to time limiting looking practice but don't feel discouraged. People already found ways around it. What does immutability bring? Well, ease of troubleshooting mostly and a more stable system. Let's give an example: You got an error, instead of your computer being unique to all of the other systems you have a common system layer. So your problem is not from the thousands of libraries you installed but a genuine problem in your distro of choice. So you can apply the patch easily without looking through all of your system journeys to find where the problem occurred. Now we got that out of the way let's look at our distros.

**BlendOS:** BlendOS is an Arch Linux based distribution that uses their overlay system to manage system packages. BlendOS is immutable but thanks to that overlay system things can be installed as if it's not an immutable distro. And you can fallback whenever a thing goes wrong. BlendOS has their own software to manage containers, plus to Flatpak and AppImage support they have three distro containers as well. Those being Ubuntu, Fedora and Arch Linux. So you can install everything to your system from these three distros.

**VanillaOS:** Another immutable distro, this time Ubuntu based, although they are thinking of switching to a Debian base in time. VanillaOS uses ABroot to manage their system packages, this creates the following side effect: Anything you installed on system layer needs a full reboot to initialize due to them not actually getting installed on the root partition you are using at that moment but to another one. So next time you boot your system you will be in the root partition you just installed the package on. VanillaOS also uses Ubuntu, Fedora and Arch Linux containers. VanillaOS is more popular these days but I should add that I had terrible time in VanillaOS a few months ago while trying to install a window manager using ABroot.

---

#### Fight:

So since we got over what our contestants are we can look into the future and guess which one will be the winner.

So, as all of us can see Linux distros are quite open for change. The current structure of "mutable distros with non containerized package managers" is bound to change. In fact, distros such as Fedora Silverblue already started to show the way to others. Silverblue is not the only example but certainly the highest profile one since it is an official edition of Fedora. The reason I didn't put it on the list was it didn't came with containerized distro inside of it. Same story for SteamOS. These both rely on Flatpak to install other software in them. BlendOS and VanillaOS despite not being official editions of their base distros, showed that both Arch Linux and Ubuntu (or Debian) can certainly be immutable. So far the fight looks as if containerized package managers are winning against containerized distributions. But don't be fooled by current status of the race. Flatpak, AppImage and Snap has been in the baking for a long while and we only started to see these containerized distributions get traction in the last year (Again, excluding Fedora Silverblue and SteamOS since they don't exactly align with my definition of containerized distribution). So it looks like anyone's game right now, but there is an important factor of each ones success.

If containerized package managers won, only a handful of distributions will actually support traditional package managers for everything but libraries. Most of the distributions will actually only have important system libraries in their repositories. When you think about it, it's not that unlikely to see traditional packages being deprecated in a scene that most of the people use containerized package managers.

On the other hand if containerized distributions win this fight, we will see no such change. containerized package managers will still exist with traditional package managers in an harmony.

---

#### My own thoughts:

I think whoever wins this fight it will be beneficial for all the Linux systems. Linux needs more unitilization. And both of these are ideal solutions for that. I'm more of an traditionalist so I would like to see containerized distributions won for the sake of keeping traditional package managers alive.

Maybe in the future we can see these Linux containers working on BSD systems as well and *nix becoming more connected than ever! There is already some work in this field but it's in alpha.

Let me know if you have different opinions than mine, cheers!
