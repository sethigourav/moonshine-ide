---
id: 575
title: Moonshine Source Setup Instructions
date: 2019-04-16T12:47:23+00:00
author: padminuser
layout: revision
guid: http://moonshine-ide.com/13-revision-v1/
permalink: /13-revision-v1/
---
\[vc\_row\]\[vc\_column\][vc\_column\_text el_class=&#8221;text-size-18&#8243;]**Before proceeding you are expected to have:**

1. Following setup instructions demonstrated with Moonshine IDE ™, users may use other IDE to setup also

2. To setup Moonshine IDE ™ please download and install [latest IDE release](https://github.com/prominic/Moonshine-IDE/releases/latest)

3. Clone or download Moonshine source code from GitHub: [Moonshine-IDE](https://github.com/prominic/Moonshine-IDE)

4. You can able to download necessary Apache Flex<sup>®</sup> SDKs in intermediate steps (i.e. through in-built SDK downloader in Windows and through App Store Helper in MacOS)\[/vc\_column\_text\]\[/vc\_column\]\[/vc\_row\]\[vc\_row\]\[vc\_column\]\[vc\_custom\_heading text=&#8221;Moonshine development requisites&#8221; font\_container=&#8221;tag:h3|text\_align:left&#8221; use\_theme\_fonts=&#8221;yes&#8221;\][vc\_column\_text]

  * AIR SDK 20+ (present development usage &#8211; [Apache 4.16.1](https://flex.apache.org/installer.html) with [Adobe AIR 28.0](https://helpx.adobe.com/flash-player/release-note/fp_28_air_28_release_notes.html)). Note: edit **MoonshineDESKTOP-app.xml** (_MoonshineDESKTOPevolved/src/MoonshineDESKTOP-app.xml_) application version per your AIR SDK version:  
    <application xmlns=&#8221;<a class="external-link" href="http://ns.adobe.com/air/application/22.0" rel="nofollow">http://ns.adobe.com/air/application/28.0</a>&#8220;>

\[/vc\_column\_text\]\[/vc\_column\]\[/vc\_row\]\[vc\_row\]\[vc\_column\]\[vc\_custom\_heading text=&#8221;Setup Moonshine IDE ™ with Apache Flex SDK&#8221; font\_container=&#8221;tag:h3|text\_align:left&#8221; use\_theme\_fonts=&#8221;yes&#8221;\][vc\_column\_text el_class=&#8221;text-size-18&#8243;]

  * Start Moonshine
  * Setup _Apache Flex<sup>®</sup> SDK_ in ****Settings****
  * In Moonshine choose _**File -> Settings -> Default SDK  
**_ 

<img class="alignnone size-full wp-image-452" src="http://moonshine-ide.com/wp-content/uploads/default_sdk.png" alt="Default SDK" width="1020" height="250" srcset="http://moonshine-ide.com/wp-content/uploads/default_sdk.png 1020w, http://moonshine-ide.com/wp-content/uploads/default_sdk-300x74.png 300w" sizes="(max-width: 1020px) 100vw, 1020px" /> 

  * _If you are using Moonshine that bundled with different SDKs, then you can use any of them to set default Flex SDK to Moonshine, or even you can downloaded Apache Flex<sup>®</sup> SDK with Adobe AIR SDK at <http://flex.apache.org/installer.html>_
  * If you are using _**OSX El Capitan**_ or higher, make sure your any downloaded SDK&#8217;s location is **~/Downloads** folder. By many restrictions applied to El Capitan, a sandbox app can execute/use SDK stuff only if it&#8217;s in user&#8217;s Downloads folder
  * (OSX) If you have setup Flex SDKs downloaded by Moonshine&#8217;s helper application _**App Store Helper**_ then you should probably see Moonshine&#8217;s default SDK.
  * You can also set your own SDK as _default_, click on _**Change**_ link inside _Default Apache Flex<sup>® </sup>Apache Royale<sup>® </sup>or Feathers SDK__ _section, this will open a popup named &#8220;Select Flex SDK&#8221; consisting of available/added SDK entries
  * To use any SDK from the above entry, simply double-click on it, and it&#8217;ll updated to _Default Apache Flex<sup>® </sup>Apache Royale<sup>® </sup>or Feathers SDK _section, or you can add your own by clicking on plus button in &#8220;Select Flex SDK&#8221; popup and complete the &#8220;Define a SDK Path&#8221; form to add your new SDK to Moonshine
  * When done, click on _**Save**_ button in _Default SDK_ section

\[/vc\_column\_text\]\[/vc\_column\]\[/vc\_row\]\[vc\_row\]\[vc\_column\]\[vc\_custom\_heading text=&#8221;Setup Moonshine Sources&#8221; font\_container=&#8221;tag:h3|text\_align:left&#8221; use\_theme\_fonts=&#8221;yes&#8221;\][vc\_column\_text el_class=&#8221;text-size-18&#8243;]

  * Checkout Moonshine sources from our [GitHub repository](https://github.com/prominic/Moonshine-IDE).
  * Moonshine sources will have three different Flex project folders:**  
** **  
    — MoonshineSharedCore**_(library project shared in desktop and web IDE)_  
    **— MoonshineDESKTOPevolved**_(desktop IDE’s gateway project)_  
    **— MoonshineWEB**_(web IDE’s gateway project)  
_  
    _(Note: this setup instructions demonstrated with desktop version’s IDE source)  
_ 
  * Import Moonshine’s desktop version source in running Moonshine IDE ™, you can do so by any of the following ways:  
    **  
    —** Choose by _**Project -> Open/Import Flex Project**_  
    **—** Click on _**Open Apache Flex/Royale Project**_ link in IDE’s splash screen. In opening folder browser dialogue navigate to the checkout sources, and select **MoonshineDESKTOPevolved **folder to open

  * Moonshine should import you now desktop version’s source in the IDE

<img class="alignnone size-full wp-image-455" src="http://moonshine-ide.com/wp-content/uploads/moonshine_sources.png" alt="Moonshine IDE sources" width="636" height="507" srcset="http://moonshine-ide.com/wp-content/uploads/moonshine_sources.png 636w, http://moonshine-ide.com/wp-content/uploads/moonshine_sources-300x239.png 300w" sizes="(max-width: 636px) 100vw, 636px" /> 

  * Now we now need to setup it&#8217;s library project (**MoonshineSharedCore**), and configure it&#8217;s settings. to do this right-click on project root node in workspace (right-hand tree panel) and choose _**Settings**_
  * You should now open with **MoonshineDESKTOPevolved **project&#8217;s settings window

<img class="alignnone size-full wp-image-420" src="http://moonshine-ide.com/wp-content/uploads/Moonshine-Sources-settings.png" alt="Moonshine Sources settings" width="976" height="580" srcset="http://moonshine-ide.com/wp-content/uploads/Moonshine-Sources-settings.png 976w, http://moonshine-ide.com/wp-content/uploads/Moonshine-Sources-settings-300x178.png 300w" sizes="(max-width: 976px) 100vw, 976px" /> 

  * Make sure the project&#8217;s _**Build Options -> Additional Compiler Options**_ read this:  
    <span style="color: #0000ff;"><span style="color: #0000ff;"><em><br /> -locale en_US -allow-source-path-overlap=true -swf-version 39 -define+=CONFIG::OSX,false +configname=air<br /> </em></span></span><span style="color: #000000;"><br /> (Note: <em>-swf-version 39</em> is the compiler argument for Adobe AIR 28.0. This may needs to vary per your SDK version usage. Please read your Adobe AIR SDK version&#8217;s release notes online to know more)</span>
  * To setup library projects, SWC, other sources etc. go to _Paths_ section in project&#8217;s settings window

<img class="alignnone size-full wp-image-421" src="http://moonshine-ide.com/wp-content/uploads/sources_settings_pt1.png" alt="Moonshine Sources settings" width="1080" height="367" srcset="http://moonshine-ide.com/wp-content/uploads/sources_settings_pt1.png 1080w, http://moonshine-ide.com/wp-content/uploads/sources_settings_pt1-300x102.png 300w" sizes="(max-width: 1080px) 100vw, 1080px" /> 

<img class="alignnone size-full wp-image-422" src="http://moonshine-ide.com/wp-content/uploads/sources_settings_pt2.png" alt="Moonshine Sources settings" width="1078" height="475" srcset="http://moonshine-ide.com/wp-content/uploads/sources_settings_pt2.png 1078w, http://moonshine-ide.com/wp-content/uploads/sources_settings_pt2-300x132.png 300w" sizes="(max-width: 1078px) 100vw, 1078px" />  
&#8212; **Class Paths**: Used to connect linked projects&#8217; source paths. Make sure _Class Paths_ are correct per your directory structure  
&#8212; **Resource Folders**: Link up this path: _MoonshineSharedCore/src/elements  
_ &#8212; **Libraries**: Link up the .SWC file from this path: __MoonshineDESKTOPevolved/libs/ApacheFlexSDKInstallerLib.swc__  
You can add entry to the sections by _**Click to Add**_ button or modify paths by _**Browse Dir**_ button. Make sure **Class Paths** sections points to the _MoonshineSharedCore_ sources per your local file system correctly. **Save** settings.

  * Moonshine uses one Adobe Native Extension for OSX version only (and specifically for it&#8217;s PKG installer). This need not to be added/included during an IDE run. Having the reference in it&#8217;s application descriptor file may also creates problem during a run from an IDE. Thus, you wants to remove the reference of the Native Extension from Moonshine application descriptor file. To do this, open _**MoonshineDESKTOPevolved/src/MoonshineDESKTOP-app.xml**_, and remove the following line if exists:  
    <span style="color: #0000ff;"><em><br /> <extensions><extensionID>karar.santanu.SecurityScopeBookmark</extensionID></extensions></em></span>
  * To test a **Flex** project choose _**Project -> Build & Run**_, to test a **Royale** project you either can choose _**Project -> Build & Run **_(produce .SWF) or _**Project -> Build & Run as JavaScript**_ (produce HTML/JavaScript); if all things are works you should see compilation output in bottom _Console_ view in Moonshine IDE ™ and an AIR window starts running Moonshine IDE&#8217;s instance, eventually. (_**Note**_: To run a _**Flex**_ project you needs your running/default-sdk to be a Flex SDK, to run a _**Royale**_ project you needs to set your running/default-sdk to a FlexJS SDK. You can toggle between SDKs by the steps as discussed in ****Setup Moonshine IDE ****™** with Apache Flex SDK** section)

\[/vc\_column\_text\]\[/vc\_column\]\[/vc\_row\]\[vc\_row\]\[vc\_column\]\[vc\_custom\_heading text=&#8221;ANT Build&#8221; font\_container=&#8221;tag:h3|text\_align:left&#8221; use\_theme\_fonts=&#8221;yes&#8221;\][vc\_column\_text el_class=&#8221;text-size-18&#8243;]

  * Starting an ANT build requires [Apache Ant<sup>®</sup>](https://ant.apache.org/) installed in your system and setup as environment variable (ensure ANT version meets minimum requirement of 1.9.2)
  * Moonshine sources supplies with it&#8217;s Ant build scripts and configured. Upon completion, the process will output desktop installer files for Windows and MacOS. You can immediately start an Ant build process if you already setup Ant in your system; to start an Ant build process we need to locate the Ant build script file (**build.xml**) prior to run the process. Moonshine supplies Ant build script file in it&#8217;s project&#8217;s **build **folder.
  * If you have already ANT_HOME setup then you can immediately build your script file by choosing _**Ant -> Configure**_ from top menu, in opening file browser dialogue navigate to your Flex project&#8217;s folder and select _build/build.xml_ file; click _**Open**_ in browser dialogue; lastly _**Ant -> Build**_. Ant build should produce .SWF and it&#8217;s HTML wrapper file set
  * If you did not have ANT_HOME setup already, choose _**Ant -> Build**_. This will open following window where you can set your Ant binary location and optionally set path to your build.xml file  
<img class="alignnone size-full wp-image-257" src="http://moonshine-ide.com/wp-content/uploads/antConfig.png" alt="antconfig" width="745" height="352" srcset="http://moonshine-ide.com/wp-content/uploads/antConfig.png 745w, http://moonshine-ide.com/wp-content/uploads/antConfig-300x142.png 300w" sizes="(max-width: 745px) 100vw, 745px" /> 
  * Upon successful completion of the process, installer files can be located at **DEPLOY** folder inside **build** folder
  * You can edit **build/ApplicationProperties.xml** to build optional Flex SDK path, build certificate paths etc. If no certificate supplies, ANT script will create a self-signed certificate for the build process automatically

\[/vc\_column\_text\]\[/vc\_column\][/vc\_row]