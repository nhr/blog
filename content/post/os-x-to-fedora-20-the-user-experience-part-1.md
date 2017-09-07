---
title: 'OS X to Fedora 20: The User Experience, Part 1'
date: '2014-08-18'
tags:
- fedora
- linux
- osx
- ux
- thunderbird
- hexchat
- limechat
aliases:
- /post/97304633660/os-x-to-fedora-20-the-user-experience-part-1
- /2014/08/18/os-x-to-fedora-20-the-user-experience-part-1.html
categories:
- Work
- Apple
- Linux
---

A little background here: I have been a Mac enthusiast for a number of years now. I would not say that I am religious about OS X, but if the OS X user experience is a philosophical application of “[opinionated](http://stackoverflow.com/questions/802050/what-is-opinionated-software) [software](https://gettingreal.37signals.com/ch04_Make_Opinionated_Software.php)”, then I find myself in agreement with most of the opinions that the Apple UX team has expressed.

However, I am also an open source developer. I’d like to believe that it is possible to create a similar and possibly even superior experience with a Linux-based desktop environment. And lo, this is what lead me, a few weeks ago, to get Fedora 20 running on a MacBook Air. If you’re interested in trying the same thing, check out Matt Hicks’ [invaluable blog post](http://mattoncloud.org/2014/02/05/fedora-20-on-a-macbook-air/) on setting things up.

Over a series of blog posts I am digging into my impressions of the Fedora 20 user experience as I work through this total switch-over.

### The Important Desktop Apps

I spend 95% of my computer time in front of the same 5 apps:

* A text editor
* A web browser
* A mail client
* A calendar client
* A chat client (specifically for IRC)

I typically also have several helper apps that I call upon and I usually have music going in the background, but I cover “Cloud stuff” in the next part of this series.

### The Same-Same Stuff

For my text editor and web browser, I’m using the same tools on both platforms: vim for text and Firefox for web. The experience of these between OS X and Fedora 20 is 99% identical. Not much else to say there.

Now as you read on you may be thinking: “hey, you could have identical experiences all the way through if you just used `<open_source_tool>` in place of `<os_x_native_tool>`”. And you’d be right. But in the cases below, I really feel like the OS X native tool is a little better, and in each case I will attempt to explain why.

### The Mail Client: Mail.app vs. Thunderbird

I don’t always think that the right answer is to make Linux match OS X, but when OS X does something really well, I wish the open-source equivalent could do the same. In the case of [Thunderbird](https://www.mozilla.org/en-US/thunderbird/), the functionality that I desire is frustratingly close, but not quite there. Specifically, I am talking about the way that Mail.app handles threaded e-mail discussions, both in the e-mails list and the email display field.

To Thunderbird’s credit, you can edit the columns displayed in the e-mails list, turn on threaded views, and Thuderbird even kinda sorta shows an all-discussion view of the thread. But Mail.app’s multi-line mail list entries make for a narrower emails listing field, and the all-discussion view still shows complete, distinct e-mails from the thread - including your own e-mails which may have gone to the Sent folder but still count as part of the conversation1. Thunderbird doesn’t do this even though [someone first raised this issue in 2003 and people have periodically asked for it ever since](https://bugzilla.mozilla.org/show_bug.cgi?id=213945).

But while the threaded views leave something to be desired, I will be the first to say that **Thunderbird’s e-mail search is awesome**. It is very fast, includes a cool chart of word hits by year, and shows enough of each e-mail in the search result to give better context for the word being searched.

Thunderbird isn’t the only mail client for Fedora; in fact, it isn’t even the default client for Fedora. But while [Evolution](https://wiki.gnome.org/Apps/Evolution) offers a very Outlook-like experience, the Outlook that it emulates is Outlook 2003. I don’t want to get into a colors and buttons argumnt, but Evolution looks pretty dated and has similar problems to Thunderbird with regard to offering an information-dense layout. Moreover:

* Evolution lacks the sort of plugin ecosystem that Thunderbird has. These plugins add a ton of value and help Thunderbird to stay current as new kinds of web services arise.

* Evolution doesn’t allow you to map mail boxes to known roles, like for instance having an Archive folder. So if you aren’t using Gmail and you want Archive-like behavior, Evolution isn’t for you.

### The Calendar Client: Calendar.app vs. Lightning

I’d love to be proven wrong, but as far as I can tell, nothing in the open-source space can even come close to what Apple, Google and Microsoft have done with their calendaring apps. I understand that doing calendaring correctly is a really hard problem, but the net result is that on the client side, open source systems seem to be limited to only the most basic functionality.

If you only keep calendars for yourself, this is probably not an issue. But for anyone who wants to schedule a meeting or have access to delegate calendars, you are going to run into problems. For this reason, and because I’d already chosen Thunderbird over Evolution, it seemed logical to pick [Lightning](https://www.mozilla.org/en-US/projects/calendar/) for e-mail. Lightning is “good enough” for showing me my schedule at a glance, but doesn’t distinguish itself as being a more functional calendar app than any of the other Linux options (like Evolution, or even the nascent [California](https://wiki.gnome.org/Apps/California)).

### The IRC Chat Client: LimeChat vs. HexChat

I use [ZNC](http://wiki.znc.in/ZNC) as a proxy server for several IRC servers where I hang out on a daily basis. ZNC’s primary job is to keep a log of the discussion on the channels that I follow so that if I miss something, I can read about it and follow up later. In order for my ZNC server to know which real IRC server I want to connect to, I need use a log name of the form:

    <znc_username>/<znc_config_name>

Well, you’d be surprised to find out how many IRC clients can’t tolerate a `/` in your username. On OS X, this drove me right into the arms of [LimeChat](http://limechat.net/mac/). I’m really glad it did, too, because the information density jammed into LimeChat’s subdued interface is totally amazing.

Many IRC clients on Fedora 20 suffer the same username handling problem, but HexChat stands out for being able to connect to VNC. Additionally it can be configured to look almost identical to LimeChat, save for LimeChat’s awesome extra window pane that shows you a continuous stream of all of the convos from the IRC room you aren’t currently looking at.

### The Upshot on Native Apps

From my perspective, Thunderbird, Lightning and HexChat provide a workable experience on Fedora 20. The more time I spend using them, the more I can work around or otherwise just accept those little bits of polish that are lacking compared to OS X. In a few cases, as with Thunderbird’s search, I can even see myself missing that functionality when I’m in front of the OS X native app equivalent. But there’s room for improvement on the Linux side and I’d love to see some open source projects that can close the gap.

Next up in this series, I’ll be talking aout the cloud services that I use and how I modifed things to use them from both OS X and this Fedora 20 system.
