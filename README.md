#How to start with TYPO3 CMS in 2015
6.x Versions mentioned. Based on personal experience.
 
## Prerequisites

You should at least be familar with HTML and CSS. Some JS knowledge is even more wise to have. After you are familar with these things you are able to dig into CMS business. If you don´t have a clue about it, you will get seriously frustrated. 
 
If you dig into TYPO3 you need a lot of time to understand it. 
 
## Keep it in mind

* If you are new to TYPO3 keep on going but don´t get disappointed if things take long time. TYPO3 has a huge learning curve, but gives you a dramatically big, flexible and quite secure universe in content management. 
 
* A lot of stuff you read can be outdated. **Keep always verifying** that you read the **latest** information, howtos and snippets and that they **match** your usecase / TYPO3 Version. 
 
* Verify extension versions and read always the documentations to the extensions.

## Good to have

* A fully qualified IDE -> see Tools section
* Get familar with git and it's usage. Versioncontrol of your code is a big help in any case at any stage
* I recommend you to write **ALWAYS ANY** code in your own providerextension -> See "extensions section" -> builder

 
## Getting into it

* Build your environment. See "Other resources" Section in this document
* Start fiddeling around with TYPOSCRIPT and FLUID
* If you come to the point of markers mentioned anywhere - read it but don´t use it. Go to FLUID.
* If you are interested in programming, go with extbase + FLUID 
   * http://vosp.info/index.php/Typo3_Extensions_entwickeln
   * http://docs.typo3.org/typo3cms/ExtbaseFluidBook/singlehtml/
* If you install extensions, try to use extbase Versions as often as possible
* You should always know what has happended in the last versions to avoid issues with outdated documentations http://typo3.org/download/release-notes/whats-new/
* This is what you need as bookmark for TYPOSCRIPT in any case 
   * http://docs.typo3.org/typo3cms/TyposcriptSyntaxReference/singlehtml/
* TYPOSCRIPT in 45 Minutes is fine way to play around with 
   * http://docs.typo3.org/TYPO3/TyposcriptIn45MinutesTutorial/
* Make a decision if you want to go the fluidypo3 way or go with Typoscript. Once you have chosen Typoscript print this and sleep on it. Perhaps it finds the way to your brain. 
  * http://docs.typo3.org/typo3cms/TyposcriptReference/singlehtml/
 
### Templating
 
There a a lot of different templating methods in TYPO3. These days FLUID is the recommended way. It´s extremely powerful and gives you great flexibility. Forget what you ever heard. If someone sais "fluid is odd" - this person has no idea of it´s capabilities and what benefits it is giving to you.

Especially choosing fluidtypo3 for templating and for logics is highly recommended.

### Sometimes mentioned - here clarified

- ** Fluidtypo3 (former Fedext) and Gridelements** 
   work great together - There´s no need for fedext vs. gridelements - but you should make a decision :-) mine is fluidtypo3 due the fact of more ground control.
- ** Should I start with the latest TYPO3 or with the latest LTS Version?   
  * It's up to you. Both are stable but the LTS has a core which will remain longer the same.
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
https://www.jetbrains.com/phpstorm/ is an example. There are plenty of out there. **Highly recommended**

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
 - **fluidcontent** does "FCE's" aka Flexible Content Elements - that allows individual content elements for your special needs https://github.com/FluidTYPO3/fluidcontent
 - **VHS** can be a great starter/companion for diving into FLUID as it takes the hassle of wiring everything within TypoScript. It is a collection of extremely powerful and advanced template viewhelpers for FLUID templating tasks https://github.com/FluidTYPO3/vhs
 - **fluidpages** gives you pagetemplates with the fluidtypo3 way. Similar to Templavoila but more powerful. But without any "gui" -believe me: GUI is not needed for that https://github.com/FluidTYPO3/fluidpages
 - **FCC** fluid content core is a new extension which replaces css-styled-content extension which builds every contentelement from typoscript. FCC builds EVERY contentelement from fluid. So in the end you are much more flexible https://github.com/FluidTYPO3/fluidcontent_core
  - **builder** lets you kickstart providerextensions and validate any fluidtypo3 and fluid syntax https://github.com/FluidTYPO3/builder

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
