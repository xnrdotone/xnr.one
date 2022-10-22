---
title: "What *nix Should You Use?"
date: 2022-10-20
description: "What should you know before picking a *nix distribution"
tags: ["*nix", "Personal Preferences", "Beginner"]
categories: ["*nix"]

---

Hello again, today I'll explain why and which \*nix distribution I use.

---

#### Distribution? What is that?

As I said in my last blog post, \*nix isn't a single operating system but more of a standard for an operating system family. The most important two main branches of this family are BSD and Linux. For example Mac OS X is a BSD distribution and Ubuntu is a Linux distribution I won't try to write the whole distribution tree because that will take ages but [this image](https://upload.wikimedia.org/wikipedia/commons/5/50/Unix_history-simple.png) may give you an idea. And that's only the main branches. When you look at just Linux itself it gets [much wilder](https://upload.wikimedia.org/wikipedia/commons/1/1b/Linux_Distribution_Timeline.svg) not the mention that image barely covers anything. So distributions are basically branches of the Unix project and this branching goes really far, for a random example in higher to lower branch order, tree of a Linux distribution called "Linux Mint" goes like this: Unix > Linux > Debian > Ubuntu > Linux Mint. It goes much deeper then this too but Linux Mint is a good middle depth example. Commonly used in Linux space, another name for an distribution is "Distro" so I'll refer to it as that from now on. 

---

#### Release cycles:

Just like most ongoing software, \*nix distros gets updates too. Since \*nix is quite fragmented some \*nix distros receive updates slower and some receive faster. These distros mainly categorized as "Fixed Release" distros and "Rolling Release" distros. Lets explain them one by one.

1 - Fixed Release Distros:

These distros as the name suggest have fixed upgrade cycles. Meaning they will only get big system updates every now and then. Usually they'll get those updates every 6-4 mouths. But not all update is a major one. Major updates, also called LTS (Long Term Support) updates happens ever other or two releases. An example would be like getting one LTS and 3 minor updates in two years with 6 months between them. These distros are usually are more stable, secure and beginner friendly. The reason they are more stable is they don't have to deal with new untested bugs of most software. The reason they are more secure is they don't have to deal with new vulnerabilities wile getting security updates for old vulnerabilities. And the reason behind being more beginner friendly is its stability as you'll have more problems with more up to date software. However this doesn't mean they are only for beginners. Due to their stable nature most servers around the world uses fixed release distros. One of the downsides of these kind of distros is that you have to update them with a usb stick when you want to get the next release.

2 - Rolling Release Distros:

These distros doesn't require you to update your system with a usb stick... Because they always are up to date! Well... At least as long as you accept the updates. Of course that comes with its own problems such as breaking the update sync if you get too behind the updates. But these are easily fixable problems. The upside and also the downside of rolling release distros is that you will always have the latest version of all the software you install although some rolling release distros likes to come from behind and hang the updates for a week or two.

My personal preference is rolling distros mostly because I don't like how the fixed release model upgrades, however I mostly don't care about having the latest version.

---

#### Package managers:

Most of the distros, at least the sane ones comes with a package manager. But what is a package manager? Well you probably used to downloading the programs you need form internet and update them separately. Or not update them at all... Well BSD/Linux distros has a solution for this! Instead of looking for a website link to download stuff you can use a software center. All the information you need is there and every download is provided by the softwares original author!

Here is an example<sup>[(1)](#resources)</sup> (Gnome Software):

![](https://i.ibb.co/BVpYBRh/image.png)

I know that Microsoft Store and App Store exists however Software Centers are much more powerful and versatile due to having more than one source for one software and having alternatives. Didn't like this software center? Here is another one developed by entirely different people!

Package managers vary from distro to distro but don't worry about which one you should pick even though when it comes to system maintenance they are in top 5 most important things they shouldn't cloud your decision about picking an distro, simply because they all do the same job.

---

#### Look and feel:

Default theming of an distro... Well it's importance is arguable by many because, some like to theme it themselves and some like to use the default theme. However since I am a customization freak I prefer basic defaults, so that I don't have to remove much. Another important issue is which Desktop Environment/Window Manager you will use. The options are limitless. To demonstrate here are the two most famous Desktop environments:

KDE Plasma<sup>[(2)](#resources)</sup>:

![](https://kde.org/announcements/plasma/5/5.26.0/fullscreen_with_apps.png)

Gnome<sup>[(3)](#resources)</sup>:

![](https://i.ibb.co/Yhz2Hj2/image.png)

As a beginner look and feel is one of the most important thing you should look in a distro because you will be using it for a long while until you decide to make it your own. Some distros look identical with the same desktop environment so choice may be hard but don't look too deep into it just pick one. 

As a beginner:

* If you planing to customize your desktop environment, the best choice for you is KDE Plasma.

* If you want to try a new workflow out of the box, your best choice is Gnome.

* If you want a workflow similar to Windows out of the box, you have lots of choices but I'd say the best choice is for you is once again KDE Plasma simply by being the most popular among the Windows like workflow desktop environments.

* If you want a workflow similar to Mac OS X out of the box, Pantheon is your best bet however, Pantheon rarely comes pre installed with a distro due to being a small project. So if you want to use it you have to use pantheon I'd suggest you to install the distro Elementary OS which is developed by same people as Pantheon itself but in my personal opinion Elementary OS isn't perfect for beginners due to it requiring some tweaks to make the software center work, so if you **must** use something similar to Mac OS X go for it but if you are okay with something a little different I once again would recommend KDE Plasma or Gnome.

---

#### Default applications:

One other thing a beginner should think about is their default application suite. Of coure this comes after picking an desktop environment in the priority list. Some desktop environments comes with a large collection of applications and some comes with just absolutely necessary things. Two good examples would be Gnome for large collection and LXQT for just necessary. Plus to desktop environments default applications there are distros default applications too. For example most distros comes with a internet browser (usually Mozilla Firefox) and a office suite too. Of course you can change these defaults but some new users don't bother so if you going to stick with the defaults make sure these programs are able to meet your requirements.

---

#### How to make a choice:

Like I said before, there are endless choices so I wanted to list couple of distros in a random order that are excellent for a starter.

* [Linux Mint](https://linuxmint.com/) (With [Cinnamon](https://linuxmint.com/edition.php?id=299) Desktop Environment)

* [Fedora](https://getfedora.org/) (With [Gnome](https://getfedora.org/en/workstation/) or [KDE Plasma](https://spins.fedoraproject.org/en/kde/) Desktop Environment)

* [Ubuntu](https://ubuntu.com) (With [Gnome](https://ubuntu.com/download/desktop) or [KDE Plasma](https://kubuntu.org/getkubuntu/) Desktop Environment)

* [Pop!_OS](https://pop.system76.com/) (With [Gnome](https://pop.system76.com/) Desktop Environment)

* [Zorin OS](https://zorin.com/os/) (With [Gnome](https://zorin.com/os/download/) Desktop Environment)

All of the above distros I gave you have unique looks and feelings from each other despite some having the same desktop environment. So just look at their sites, maybe search their names in your web browser and look at some pictures or watch videos about them, and most importantly; Just pick one! Don't worry about it, you will like it. It's better than desperately looking at endless options believe me.

You may ask "All the examples above are fixed release distros, what if I want to use a rolling release distro?"

To that I would say, calm down... You won't be using your first distro for more than 6 months probably you can make the choice down the line when you get more familiar with BSD/Linux. Rolling release distros require a bit more knowledge but if you **must** use them I'd say use [Manjaro](https://manjaro.org/) (with [Gnome](https://manjaro.org/download/) or [KDE Plasma](https://manjaro.org/download/) desktop environment) It's rather balanced when it comes to update cycles. But if you want something that gets all the updates instantly well... There is [Endavour OS](https://endeavouros.com/). Don't say I didn't warn you though, things **will** break. Luckly both Manjaro Linux and Endavour OS has rather great community forums, which leads us to our next topic.

---

#### Support:

One of the most important things for a beginner BSD/Linux user is getting support. Even in Windows or Mac OS X you sometimes need to search for something on the web to solve your problems. Well you can search for lots of BSD/Linux related things but plus to that you have the option to ask about it on forums. All the distros I mentioned above has really friendly communities due to being beginner friendly distros.

---

#### My personal preference:

I personally use Manjaro but when I buy a new computer I'll switch to Arch Linux due to few issues I have with Manjaro. I won't get into details on that because they are a bit technical. As for desktop environments and window managers go, I use currently OpenBox which I definitely won't suggest for a beginner. As for default applications... Well I don't have a default suite. I just install whatever I like. Here is how my system looks with OpenBox:

![](https://i.ibb.co/ZBjjJY0/image.png)

Aside from OpenBox I also use few other desktop environments and window managers, namely Bspwm, Qtile and KDE Plasma.

Thank you for reading.

---

#### Resources:

1 - Image from [9to5Linux.com](https://9to5linux.com/first-look-at-some-of-the-gtk4-apps-in-gnome-42)

2 - Image from [kde.org](https://kde.org/)

3 - Image from [gnome.org](https://www.gnome.org/)
