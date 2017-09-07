---
title: New Challenges, New Tools
date: '2015-06-10'
aliases:
- /post/121196035340/new-challenges-new-tools
- /2015/06/10/new-challenges-new-tools.html
categories:
- Work
- Apple
- Linux
---
I almost feel like a traitor, which is a weird way to feel about consumer electronics. But my next laptop is not going to be a MacBook. Our current development work on [OpenShift](https://openshift.com) requires easy access to a docker service, and [Boot2docker](http://boot2docker.io/) just doesn’t cut it.

Apple provides an excellent ecosystem of interrelated apps; they find ways to make it easy to move content from one app to another that seem intuitive. This requires the lock-step portfolio-wide architecture that you will rarely see in open source. At least, not across native desktop apps.

But so much of what used to happen on the desktop has been replaced by the cloud, and so many interoperability problems are being solved by cloud app folks that in reality, the playing field is fairly level between OS X, Linux and Windows. My parting comment in my WWDC piece was:

> ...as more of our ‘office’ tools move to the cloud, any platform that can run a modern browser is a competitor...

I don’t necessarily _want_ to do all of my work in a browser, but where web UIs go these days, native clients seem to follow.

### What I Like About Mac

Thinking over my years of Apple product use, here’s the top three things I’ve loved about MacBook and OS X:

**MacBook build quality is as good as it gets.**  
This is a big deal, and it matters to me a lot. The all-aluminum design is heavier than some carbon-fiber competitors, but the laptops can take a beating.

**OS X provides great default apps.**  
There are many computer-based tasks where I am not strongly opinionated about the tools I use, and OS X bundles apps developed by people who were paid to be strongly opinionated about them. I’m talking about Mail, Calendar, Reminders, and Notes. The net result is a native app potfolio that surpases expectations, to the point where I feel no motivation to seek alternatives.

**I can run Windows for Gaming**  
Apparently, Microsoft’s OS is capable of doing other things as well, but my laptop’s Boot Camp partition has one job: running video games.

But continuing to use a MacBook as my primary system when I am part of a development team that is doing full-stack work against a Linux kernel is just making less and less sense. And having needed to straddle OS X and Linux for the past three years, I’ve found a series of great cloud-based apps that replace or even surpass the OS X app portfolio.

### The New Deal

Having taken all of that into consideration, here’s my plan for a replacement system.

**OS: Fedora**  
From a desktop perspective, there are better Linux-based “out-of-box” experiences than Fedora. But for me, a huge part of being productive in OS X was learning the keyboard shortcuts, and Fedora has great keyboard shortcuts. It also provides a full-screen app / screen switching model that is ver similar to OS X, which makes changing desktops easier for Mac users.

I called out some great default OS X apps above; here’s my replacement plan:

* For Mail, [Geary](https://wiki.gnome.org/Apps/Geary). Geary provides a very similar conversation-based mail display model and works perfectly with Gmail. My one wish-list item for Geary: let me map IMAP folders to the “special” folders so that you can treat my “Archive” folder on the work server the same way you treat “All Mail” on Gmail.
* For Calendar, [California](https://wiki.gnome.org/Apps/California). Made by the same folks who do Geary (and Shotwell). The display is very Calendar like, Geary supports all of the same protocols as well.
* For Reminders, I’m partially sticking with Reminders. Well played, Apple. For work tasks I’m mostly using [Wunderlist](https://www.wunderlist.com/) because there are clients for Linux (via Chrome) and iOS. But Reminders has the nice “Remind me when I get to location X” feature so it continues to be used, at least on my phone.
* For Notes, I’m using a combination of [Simplenote](http://simplenote.com/) and [Zim Wiki](http://zim-wiki.org/). Simplenote does everything that Notes does, and Zim Wiki provides a more Evernotes-like experience but in a database that is completely not cloud-based. Some work info doesn’t belong in the cloud; it goes in Zim Wiki so I can still search on it and take freeform notes.

**Hardware: HP Omen 15"**  
If you are not a gaming enthusiast, you’ve probably never heard of [VoodooPC](https://en.wikipedia.org/wiki/VoodooPC). They were a boutique PC manufacturer that made high-end gaming computers. They were bought by HP and after that, Voodoo continued to be associated with HP’s bleeding edge laptops and desktops. These days, the “Voodoo” name has disappeared from HP’s product portfolio, but their DNA remains in products like the [Omen 15](http://store.hp.com/us/en/SearchDisplay?searchTerm=omen&search=%25EF%2580%25A1&beginIndex=0&catalogId=10051&charset=utf-8&langId=-1&pageSize=50&pageView=grid&resultCatEntryType=2&sType=SimpleSearch&searchSource=Q&storeId=10151)".

Like the MacBook, the Omen features an all-aluminum body and a solid-state hard drive. Like the top-end MacBook Pro 15", the Omen features a discrete graphics processor with its own dedicated RAM. But that’s where the similarities end.

### The Benefits of Change

Feature-wise, and based on what we’re hacking at work, I believe I’ve won out in the bargain. Here’s how moving to the Omen matches up…

**Lower Cost**  
As of the time of this blog post, the same-spec''ed MacBook Pro 15" with a lesser discrete graphics card cost more. Now, a major argument in favor of Apple has always been that they don’t charge for OS upgrades and Windows does, but in this case, 1) I’m using Linux as primary, so that’s moot, and 2) Windows 10 is also going to be a free upgrade.

**Better Linux Hardware Support**  
I actually ran Fedora directly on a MacBook Air for a while, but the hardware support is not rock solid. Most notably, Apple’s choice of a PCI-based webcam with no open source drivers meant that I could never videoconference from my laptop. These are non-issues on the Omen.

**Business in the Front, Party in the Back**  
The Omen has an almost embrassing amount of LED-driven “bling lighting”. It has LEDs backlighting the keyboard (which is pretty standard), but also in the speakers and fan exhaust ports. Happily, I can turn all of that off in “work mode” under Linux. The Omen doesn’t need it to stand out and look like an awesome laptop. But hey, when I flip it over to the “gaming OS”? Yeah, I’m cranking up the LEDs :-)

### Return on Investment?

Time will tell if I’m going to miss OS X. From the OS / apps side, I think I’ve found a combination that works well between a Linux laptop and an iOS phone, and on the hardware side, I feel like I’ve found a system with the same solid build as a MacBook.

The first time I spin up OpenShift directly on my laptop – that’s going to be a win.
