#Howto start with TYPO3 CMS in 2015
* 6.x Versions mentioned. Based on personal experience
* Still valid for 7.0.x

## What this document does

* Shows you some basic stuff for TYPO3, how to get into it and how to handle some things
* Does not show you basic principles of the TYPO3-CMS itself

## Prerequisites

* You should at least be familar with HTML and CSS 
* Some JS knowledge is even more wise to have

After you are familar with these things you are able to dig into CMS business. 
**If you don´t have a clue about it, you will get seriously frustrated.**
 
If you dig into TYPO3 you need a lot of time to understand it. 
 
## Keep it in mind

* If you are new to TYPO3 keep on going but don´t get disappointed if things take long time. TYPO3 has a huge learning curve, but gives you a dramatically big, flexible and quite secure universe in content management. 
 
* A lot of stuff you read can be outdated. **Keep always verifying** that you read the **latest** information, howtos and snippets and that they **match** your usecase / TYPO3 Version. 
 
* Verify extension versions and read always the documentations to the extensions.

## Good to have

* A fully qualified IDE -> see [Tools](#user-content-tools) section
* Get familar with git and it's usage. Versioncontrol of your code is a big help in any case at any stage
* I recommend you to write **ALWAYS ANY** code in your own providerextension -> See section [extensions](#user-content-extensions) -> ext:builder

 
## Getting into it

* If you know nothing http://docs.typo3.org/typo3cms/GettingStartedTutorial
* Build your environment. See "Other resources" Section in this document
* Get familar with git and github. It's a versioning system and let's you dive into coderevisions with ease
* Start fiddeling around with TYPOSCRIPT and FLUID
* If you come to the point of markers mentioned anywhere - read it but don´t use it. Go to FLUID
* If you are interested in programming, go with extbase + FLUID 
   * http://vosp.info/index.php/Typo3_Extensions_entwickeln
   * http://docs.typo3.org/typo3cms/ExtbaseFluidBook/singlehtml/
* If you install extensions, try to use extbase Versions as often as possible
* You should always know what has happended in the last versions of the cms to avoid issues with outdated documentations http://typo3.org/download/release-notes/whats-new/
* You should always know what has happened in the last versions of extensions that you use. Several locations do give advice. [git/forge/TER/individual location] -> Depends on the extension, just find out.
* This is what you need as bookmark for TYPOSCRIPT in any case 
   * http://docs.typo3.org/typo3cms/TyposcriptSyntaxReference/singlehtml/
* TYPOSCRIPT in 45 Minutes is fine way to play around with 
   * http://docs.typo3.org/TYPO3/TyposcriptIn45MinutesTutorial/
* Make a decision if you want to go the FLUIDTYPO3 way, go with TYPOSCRIPT only or if you want to use both. Once you have chosen TYPOSCRIPT -> print this and sleep on it. Perhaps it finds the way to your brain. 
  * http://docs.typo3.org/typo3cms/TyposcriptReference/singlehtml/
 
### Templating
 
There a a lot of different templating methods and systems in TYPO3. These days FLUID is the recommended way. It´s extremely powerful and gives you great flexibility. Forget what you ever heard. If someone sais "fluid is odd" - this person has no idea of it´s capabilities and what benefits it is giving to you.

Especially choosing fluidtypo3 for templating and for logics is highly recommended.

### Sometimes mentioned - here clarified

- **FLUIDTYPO3 (former fedext) and ext:gridelements** 
   work great together - There´s no need for fedext vs. gridelements - but you should make a decision :-) mine is fluidtypo3 due the fact of more ground control.
- **Should I start with the latest TYPO3 SPRINT or with the latest TYPO3 LTS Version?**   
  * It's up to you. Both are stable but the LTS has a core which will remain longer the same. The SPRINT Version has always the latest changes in core
- **Is templavoila for templating an option?**
  * IMHO not. It was once a smart approach for templating which is outdated by now. It's still kept "working" but in the end there's no active feature devolopment anymore. If you think that you need a GUI with "Point and Click" for templating then honestly you should consider changing your job

### What is....
- **What is TYPOSCRIPT**
  * Read this: http://docs.typo3.org/typo3cms/TyposcriptSyntaxReference/AppendixA/Index.html
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


### Pitfalls

This section has to be done one day. Here just the topics that are taken into account:

#### In General
#### Server
#### Installation
#### TYPOSCRIPT
#### FLUID
#### EXTBASE
 
 
## Useful Links

### Help resources

* **Mailinglists** 
http://lists.typo3.org/ 
* **Newsreader**
http://typo3.org/support/mailing-lists/use-a-newsreader/ 
* **Forum** 
http://forum.typo3.org/ 
* **IRC - Internet relay chat** 
typo3 && fedext channel on freenode.net 
* **Forge | bugs and useful info for extensions** 
http://forge.typo3.org/projects


### Tools

* **IRC Client** 
https://hexchat.github.io/ is an example. There are plenty of out there
* **IDE Editor** 
https://www.jetbrains.com/phpstorm/ is an example. There are plenty of out there. **This one is highly recommended**

### Documentations

* **Docs in general** 
http://docs.typo3.org/ 
* **TYPO3 CMS related Docs** 
http://docs.typo3.org/typo3cms/Index.html
* **TYPO3 Extension Manuals** 
http://docs.typo3.org/typo3cms/extensions/
* **Fluidtypo3** 
https://github.com/FluidTYPO3/documentation
* **Fluidtypo3 Viewhelper reference** 
https://fluidtypo3.org/viewhelpers/

### Extensions 

* **Fluidtypo3** 
https://fluidtypo3.org/
Is a peek worth as it is a huge tool universe - it´s pure extbase and FLUID
 - **ext:fluidcontent** does "FCE's" aka Flexible Content Elements - that allows individual content elements for your special needs https://github.com/FluidTYPO3/fluidcontent
 - **ext:VHS** can be a great starter/companion for diving into FLUID as it takes the hassle of wiring everything within TypoScript. It is a collection of extremely powerful and advanced template viewhelpers for FLUID templating tasks https://github.com/FluidTYPO3/vhs
 - **ext:fluidpages** gives you pagetemplates with the fluidtypo3 way. Similar to Templavoila but more powerful. But without any "gui" -believe me: GUI is not needed for that https://github.com/FluidTYPO3/fluidpages
 - **ext:FCC** fluid content core is a new extension which replaces css-styled-content extension which builds every contentelement from typoscript. FCC builds EVERY contentelement from fluid. So in the end you are much more flexible https://github.com/FluidTYPO3/fluidcontent_core
  - **ext:builder** lets you kickstart providerextensions and validate any fluidtypo3 and fluid syntax https://github.com/FluidTYPO3/builder

### Other resources

* **Launchr** *
 https://launchr.com is a service to launch a TYPO3 instance within some seconds to try things in a clean environment.
* **Vagrant** *
https://www.vagrantup.com/ is a tool for installing a complete preconfigured virtual machine with no hassle. See https://github.com/FluidTYPO3/FluidTYPO3-Vagrant
* **Bitnami for XAMPP** *
https://bitnami.com/stack/typo3 is an addition to XAMPP (local webserver, mysql,php enviconment) Quickly install a complete clean and working typo3 locally

### TYPO3 itself
 
* **TYPO3 Packages** 
http://get.typo3.org/ 
 - For definitions of the packages go to http://typo3.org/download/#c1981
 - All in all-the bootstrap package is by far the most current "distribution" for starters and really shows great use of FLUID and TS (TYPOSCRIPT) side by side.

### Thanks
- to cedricziel, kraftb, NamelessCoder and many others

### Contribution
Highly welcome

