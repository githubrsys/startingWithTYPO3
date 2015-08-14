> Hi, I'm rosieres from TYPO3 IRC Channel. Dealing with TYPO3 is my daily business for several years now. If you need qualified technical support or want to start a project you can reach me @ http://r-system.de (don't be scared - we just do not have the time for overhauling)

##### I made this sheet for shortening the entrance into TYPO3 

#Howto start with TYPO3 CMS in 2015
* Based on personal experience
* Still valid for 7.x
* broke down to the bare minimum

## What this document does

* Shows you some basic stuff for TYPO3. How to get into it, how to handle some things and partially gives some hints for developing
* Does not show you basic principles of the TYPO3-CMS itself
* This document aims torwards newbie integrators and can be overflown also by newbie developers
* It has no benefitical information for editors

## Prerequisites

* You should at least be familar with HTML and CSS 
    * -> Learn it on [Codeacademy](http://www.codecademy.com/tracks/web) for free
* Some JS knowledge is even more wise to have. In particular jQuery 
    * -> Learn it on [Codeacademy](http://www.codecademy.com/tracks/jquery) for free

After you are familar with these things you are able to dig into CMS business. 

**If you don´t have a clue about HTML and CSS, you will get seriously frustrated and you should not start anything.**
 
If you dig into TYPO3 you need a lot of time to understand it.
 
#### Prerequisites - for developers
* You should at least have read this: http://docs.typo3.org/typo3cms/ExtbaseFluidBook/2-BasicPrinciples/3-Model-View-Controller-in-Extbase.html
* You are good advised to read the basic principles completely http://docs.typo3.org/typo3cms/ExtbaseFluidBook/2-BasicPrinciples/Index.html
* **TYPO3 Extbase Reference** shows you the mandatory stuff http://docs.typo3.org/typo3cms/ExtbaseFluidBook/b-ExtbaseReference/Index.html
 
## Keep it in mind

* If you are new to TYPO3 keep on going but don´t get disappointed if things take long time. TYPO3 has a huge learning curve, but gives you a dramatically big, flexible and quite secure universe in content management.
* A lot of stuff you read can be outdated. **Keep always verifying** that you read the **latest** information, howtos and snippets and that they **match** your usecase / TYPO3 Version.
* Verify extension versions and read always the documentations to the extensions.
* If you see a bug or a non self-explanatory documentation **start contributing immediately**. It is always welcome. And do not forget: You are using all for free, so the minimum you can do is to contribute. Your skilllevel is secondary in this moment because **every point of view has its own reason to be there**.

## Good to have

* A fully qualified IDE -> see section [Tools](#tools) 
* If not an IDE then at least a cool text-editor -> see section [Tools](#tools)
* Get familar with git and it's usage. Versioncontrol of your code is a big help in any case at any stage
* I recommend you to write **ALWAYS ANY** code in your own providerextension -> See section [extensions](#extensions) -> ext:builder

## Getting into it

1. If you know nothing -read [getting started](http://docs.typo3.org/typo3cms/GettingStartedTutorial)
2. Know the base principles of TYPOSCRIPT in [general](http://docs.typo3.org/typo3cms/TyposcriptIn45MinutesTutorial/)
3. Know the principles of extensions in [general](http://typo3.org/extensions/what-are-extensions/) and in [detail](http://docs.typo3.org/typo3cms/CoreApiReference/ExtensionArchitecture/Index.html)
4. Know where to find documentations -> see section [Documentations](#documentations)
5. Know how to get help -> see section [Help Resources](#help-resources) and [Howto ask](#howto-ask) the right way
6. Build your environment
    * Webserver -> see section [Other resources](#other-resources)
    * DB Server -> see section [Other resources](#other-resources)
    * IDE -> see section [Tools](#tools) IDE Editor
7. Get familar with [git](http://rogerdudler.github.io/git-guide/index.html) and [github](http://github.com) [definition](http://wikipedia.org/wiki/GitHub) and [gist](http://gist.github.com) [definition](http://en.wikipedia.org/wiki/GitHub#Gist)
8. Providerextension - I recommend you to write **ALWAYS ANY** code in such a -> See section [extensions](#extensions) -> ext:builder
9. Start fiddeling around with TYPOSCRIPT and FLUID
    * If you come to a point where markers are mentioned like ``###marker###`` - read it but don´t use it. Go to FLUID
10. If you want to stick to OOP paradigms, get familiar with Extbase, since this is the built in MVC framework of TYPO3. For other use cases the core offers a lot of ready made API stuff besides Extbase out of the box. So be sure to check for existing core methods before reinventing the wheel.
11. If you install extensions from [TER](http://typo3.org/extensions/repository/), try to use current versions compatible to the latest TYPO3 versions as often as possible. Even if you go for older LTS versions of TYPO3, this will make sure to stay up to date with core upgrades in the future.

* You should always know what has happened in the last versions of the cms to avoid issues with outdated documentations http://typo3.org/download/release-notes/whats-new/

* You should always know what has happened in the last versions of extensions that you use. Several locations do give advice. [git/forge/TER/individual location] -> Depends on the extension, just find out.

* Make a decision if you want to go the FLUIDTYPO3 way, go with TYPOSCRIPT only or if you want to use both. Once you have chosen TYPOSCRIPT -> print this and sleep on it. Perhaps it finds the way to your brain. 
  * http://docs.typo3.org/typo3cms/TyposcriptReference/singlehtml/
  
* This is what you need as bookmark for TYPOSCRIPT in any case 
   * http://docs.typo3.org/typo3cms/TyposcriptSyntaxReference/singlehtml/

* **If you are interested in programming**, go with extbase + FLUID
   * And dive into [documentations and cheatsheet section](#documentations)
 

### Templating
 
There a a lot of different templating methods and systems in TYPO3. I won't go into details here. These days FLUID is the recommended way. It´s extremely powerful and gives you great flexibility. Forget what you ever heard. If someone sais "fluid is odd" - this person has no idea of it´s capabilities and what benefits it is giving to you.


## Sometimes mentioned - here clarified

- **FLUIDTYPO3 (former fedext) and ext:gridelements** 
   work great together - There´s no need for fedext vs. gridelements - but you should make a decision :-) mine is fluidtypo3 due the fact of more ground control.
- **Should I start with the latest TYPO3 SPRINT or with the latest TYPO3 LTS Version?**   
  * It's up to you. Both are stable but the LTS has a core which will remain longer the same. The SPRINT Version has always the latest changes in core
- **Is templavoila for templating an option?**
  * IMHO not. It was once a smart approach for templating which is outdated by now. It's still kept "working" but in the end there's no active feature devolopment anymore. If you think that you need a GUI with "Point and Click" for templating then honestly you should consider changing your job

## What is....
- **What is TYPOSCRIPT**
  * Read this: http://docs.typo3.org/typo3cms/TyposcriptSyntaxReference/AppendixA/Index.html
- **What is the TSOB - TYPOSCRIPT OBJECT BROWSER**
  * Read this: http://docs.typo3.org/typo3cms/GettingStartedTutorial/Templates/TheObjectBrowser/Index.html
- **Is TYPOSCRIPT mandatory**
  * No. But you are good advised to know the principles as every extension uses it more or less. If you decide to avoid TYPOSCRIPT you can use ext:fcc and ext:vhs to reach your goals. And plain extbase programming of course.
- **What is FLUIDTYPO3**
  * FLUIDTYPO3 is a set of extensions that give you handy tools for developing and templating based on fluid and extbase. See section extensions in this document.
- **What is FLUID**
  * Is the recommended templating engine of TYPO3. It's not mandatory but nearly every new extension of typo3 relies on that. So you are good advised to use it.
- **What is the difference of FLUID and FLUIDTYPO3**
  * See above. FLUIDTYPO3 is a set of extensions that heavily use FLUID as templatingengine and extbase as logic processor.
- **What is extbase**
  * Read this http://docs.typo3.org/typo3cms/ExtbaseGuide/Extbase/Index.html

## Howto ask

If you have a question -there are plenty of resources -> see section [Help Resources](#help-resources) 

They all have one thing in common. You must ask the right questions and provide necessary information to get qualified help. Otherwise people wont help you as it takes to long to pull things out of your nose.  

**Use this pattern as a rule of thumbs:**

> **tl;dr** 
> ### WwwwwP 
> **W**hat is your environment, **w**hat do you want to achieve, **w**hat did you do, **w**hat do you expect, **w**hat do you get. **P**rovide a [gist](https://gist.github.com/)

*  **What is your environment** 
    * Tell us what TYPO3 Version
    * Which extensions and versions do you use
    * Where is your code nested in
    * Server environment if necessary
* **What do you want to achieve**
    * Tell us what you want to have in the end. 
    * Needed to determine if you are on the right track.
* **What did you do**
    * Tell us what did you do and why.
    * In some circumstances this can also be understood as "how to reproduce" your actual behaviour
* **What do you expect**
    * Tell us what do you expect
* **What do you get**
    * Tell us what do you get
* **Provide a [gist](https://gist.github.com/)**
    * Show us your code. Everything else is digging in the dark -mostly.
    * Copy and paste your original code to avoid typos. 
    * Break down code to a minimum working example if you are asked to or if your problem relies on a principle that you do not understand
    * divide into several files if your problem relies on multiple files or situations

## Pitfalls

This section has to be done one day. Here just the topics that are taken into account:

#### In General
#### Server
#### Installation
#### TYPOSCRIPT
#### FLUID
#### EXTBASE
 
 
## Useful Links

### Help resources

* **Mailinglists** - You must use a [Newsreader](http://typo3.org/support/mailing-lists/use-a-newsreader/ )
    * http://lists.typo3.org/ 
* **Forum** - Hint: Search the forum like [this](https://www.google.de/#q=site:forum.typo3.org+searchwords) 
    * http://forum.typo3.org/ 
* **Forge | bugs and useful info for extensions** 
http://forge.typo3.org/projects
* **Forger** https://forger.typo3.org It basically provides an intuitive interface to filter reviews and shows some statistics based on forge 
* **Slack** The Slack tool is also used by plenty of other teams around the TYPO3 ecosphere so it is easier to interconnect teams. If you want to join the Slack team, please register at http://forger.typo3.org/slack/.
Then join http://typo3.slack.com/ and our channel #typo3-cms
* **IRC - Internet relay chat** Hint: Search the typo3 irc like [this](https://www.google.de/#q=site:riesvantwisk.com+typo3+IRC+Log+searchwords) and the fluidtypo3 irc like [this](https://fluidtypo3.org/search.html?q=foo)
typo3 && fedext channel on freenode.net 

### Tools

* **IRC Client** 
https://hexchat.github.io/ is an example. There are plenty of out there
* **IDE Editor** 
https://www.jetbrains.com/phpstorm/ is an example. There are plenty of out there. **This one is highly recommended**
* **Text Editor** just cool. And don't forget to install [packagecontrol](https://packagecontrol.io/installation) 
http://www.sublimetext.com/

### Documentations
#### in general
* **TYPO3 documentations in general** 
http://docs.typo3.org/ 
* **TYPO3 CMS related documentations** 
http://docs.typo3.org/typo3cms/Index.html
* **TYPO3 extension manuals** 
http://docs.typo3.org/typo3cms/extensions/
* **Hardening & Security in TYPO3 - Guidelines - best practice**
http://docs.typo3.org/typo3cms/SecurityGuide/stable/GuidelinesIntegrators/
* **Understand TYPOSCRIPT**
- http://docs.typo3.org/typo3cms/TyposcriptSyntaxReference/singlehtml/
- http://docs.typo3.org/typo3cms/TyposcriptReference/singlehtml/

#### dedicated extensions
* **FLUIDTYPO3 documentations** 
https://github.com/FluidTYPO3/documentation
* **FLUIDTYPO3 ext:vhs and FLUID viewhelper reference** 
https://fluidtypo3.org/viewhelpers/

#### for developing + cheatsheets
* **TYPO3 API Reference** helps you to understand principles
http://docs.typo3.org/typo3cms/CoreApiReference
* **TYPO3 API Documentation** shows you all available classes and functions within the CMS API
http://typo3.org/documentation/api/
* [Reserved-folders](http://docs.typo3.org/typo3cms/CoreApiReference/ExtensionArchitecture/FilesAndLocations/Index.html#extension-reserved-folders) is a good start *before* reading the [extbase book](http://docs.typo3.org/typo3cms/ExtbaseFluidBook/singlehtml/). Then you are good advised to build a providerextension and try to adopt working scenarios from existing extbase extensions. That's the fastest way to dig into it extbase.
   * **TYPO3 Extbase Reference** shows you the mandatory stuff http://docs.typo3.org/typo3cms/ExtbaseFluidBook/b-ExtbaseReference/Index.html
   * Also mentionworth http://vosp.info/index.php/Typo3_Extensions_entwickeln
    * **Extbase: Query and Repository Overview / Cheatsheet**  http://lbrmedia.net/codebase/Eintrag/extbase-query-methods/
    * **Extbase & Fluid: Cheatsheet** http://www.lobacher.de/files/cs/ExtbaseFluidCheatSheet_3.02_pluswerk.pdf

### Contribute / Patch / Bugfix
If you want to contribute, there are several ways
* **Core** https://wiki.typo3.org/Contribution_Walkthrough_Tutorials
* **Extensions** Depends on the Extension. See docs of extension if forge.typo3.org, github.com, git.typo3.org or other resource

### Extensions 

* **[FLUIDTYPO3](https://fluidtypo3.org/)** 
A peek worth - it is a huge tool universe - pure extbase and FLUID
 - **ext:fluidcontent** does "FCE's" aka Flexible Content Elements - that allows individual content elements for your special needs https://github.com/FluidTYPO3/fluidcontent
 - **ext:vhs** can be a great starter/companion for diving into FLUID as it takes the hassle of wiring everything within TYPOSCRIPT. It is a collection of extremely powerful and advanced template viewhelpers for FLUID templating tasks https://github.com/FluidTYPO3/vhs
 - **ext:fluidpages** gives you pagetemplates with the FLUIDTYPO3 way. Similar to TEMPLAVOILA -more powerful. But without any "GUI" -believe me: GUI is not needed for that https://github.com/FluidTYPO3/fluidpages
 - **ext:fcc** fluid content core is a extension which replaces css-styled-content extension (which builds every contentelement from TYPOSCRIPT). FCC builds EVERY contentelement from FLUID with the help of EXTBASE. https://github.com/FluidTYPO3/fluidcontent_core
  - **ext:builder** lets you kickstart providerextensions and validate any FLUIDTYPO3 and FLUID syntax https://github.com/FluidTYPO3/builder
* **ext:extension_builder** lets you kickstart extensions and build complex models with a GUI. Also writes automatic getters and setters and many, many, many more http://typo3.org/extensions/repository/view/extension_builder 
* **ext:typo3_console** gives you some CLI functions
https://github.com/helhum/typo3_console
### Other resources

* **Launchr**
 https://launchr.com is a service to launch a TYPO3 instance within some seconds to try things in a clean environment.
* **Vagrant**
https://www.vagrantup.com/ is a tool for installing a complete preconfigured virtual machine with no hassle. See https://github.com/FluidTYPO3/FluidTYPO3-Vagrant
* **Bitnami for XAMPP**
https://bitnami.com/stack/typo3 is an addition to XAMPP (local webserver, mysql,php enviconment) Quickly install a complete clean and working typo3 locally
* **Own and manual installation**
read this in general https://github.com/TYPO3/TYPO3.CMS/blob/master/INSTALL.md
* **Git -[short and sweet](http://rogerdudler.github.io/git-guide/index.html)**
### TYPO3 itself
 
* **TYPO3 Package** 
http://get.typo3.org/ 
 - All in all-the bootstrap package is by far the most current "distribution" for starters and really shows great use of FLUID and TS (TYPOSCRIPT) side by side.
* **TYPO3.CMS Git repo** - See what's going on with shortlog and examine core files
https://git.typo3.org/Packages/TYPO3.CMS.git

### Found a problem

* for TYPO3 core
    * https://forge.typo3.org/projects/typo3cms-core
* for TYPO3 extensions
    * Determine from extension manual where to post issues to. Can be forge / github / mail / external site

### Thanks
- to cedricziel, kraftb, NamelessCoder and many others

### Contribution
Highly welcome

### This site is published
http://githubrsys.github.io/startingWithTYPO3
