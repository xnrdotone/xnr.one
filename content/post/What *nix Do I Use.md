---
title: "What *nix Do I Use"
date: 2022-10-16T01:46:10+03:00
description: "What is my daily driver?"
tags: ["*nix", "personal preferences"]
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

<details>

<summary>CLICK ME</summary>

<p>
<img src= "https://i.ibb.co/BVpYBRh/image.png"></img>
</p>

</details>

![](https://i.ibb.co/BVpYBRh/image.png)

#### Resources:

1 - Image from [9to5Linux](https://9to5linux.com/first-look-at-some-of-the-gtk4-apps-in-gnome-42)