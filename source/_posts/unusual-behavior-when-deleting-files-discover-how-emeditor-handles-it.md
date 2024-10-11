---
title: Unusual Behavior When Deleting Files - Discover How EmEditor Handles It
date: 2024-10-04T16:05:29.489Z
updated: 2024-10-10T23:52:45.088Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/cceaece01aa4bcb3e2bd94d9a7dafd046bccc2616fb9998b912dd3cd3c939c21.jpg
---

## Unusual Behavior When Deleting Files - Discover How EmEditor Handles It

Viewing 5 posts - 1 through 5 (of 5 total)

* Author  
Posts
* February 28, 2013 at 11:02 am [#10874](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/5e2551a06c05e17c7abab191ebd0d3f3?s=80&d=identicon&r=g)XXCloneMan](https://www.emeditor.com/forums/users/XXCloneMan/ "View XXCloneMan's profile")  
Member  
Today, my EmEditor stopped accepting a file being dropped on the EmEditor area (to initiate a new edit session).  
 It’s so strange and I can’t figure out why. Like most other tools (Notepad, MSPaint, etc.), one way to open a file for editing (or just viewing) in Windows, EmEditor accepts a file being drag-and-dropped and a new edit session starts. Now, all of a sudden, that feature stopped working.  
 The following image shows how the mouse cursor changes its shape while a file is being dragged around the Desktop.  
<http://xxclone.com/img/dragdrop.png>  
 When the application under the cursor is ready to accept the file, the cursor shape changes to the “drop-accepted” icon, else, the “drop-disallowed” cursor goes with the mouse. For some reason, my EmEditor only shows the “drop-disallowed” cursor. I searched everywhere in EmEditor to see if it was accidentally disabled, and I could not find a switch for it.  
 On the other hand, other tools such as NotePad works with drag-and-drop, so, I can’t imagine it is done by Windows.  
 There must be a checkbox for this somewhere in EmEditor — I just can’t find it.  
 (EmEditor’s help did not give me any match with various keyword for this).  
 Am I the only one who became completely lost on this?  
February 28, 2013 at 6:08 pm [#10875](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
Hello,  
 The only option we have is “Enable Text Drag and Drop” check box on the Mouse tab of the Customize dialog box, but this is not related to the issue you described. Plug-ins can have something to do with this issue, so can you disable plug-ins if you have installed plug-ins other than default installed plug-ins?  
 If you still have issue, I would restart Windows. If you still have the issue after restarting Windows, can you export all your settings to .REG files from Tools menu > Import and Export > Export all settings into a registry, and then uninstall EmEditor, make sure all files in the C:Program FilesEmEditor are deleted, restart Windows, and then install the newest version of EmEditor? Can you also please zip the reg files and email me at [tech@emurasoft.com](https://tools.techidaily.com/emeditor/products/)? I would like to reproduce the issue here.  
 Thank you!  
March 1, 2013 at 3:55 am [#10877](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/5e2551a06c05e17c7abab191ebd0d3f3?s=80&d=identicon&r=g)XXCloneMan](https://www.emeditor.com/forums/users/XXCloneMan/ "View XXCloneMan's profile")  
Member  
Today, I cannot observe the same “disallowed-drop” behavior by EmEditor on the same machine (Win7 Ultimate x86). So, Yutaka’s suggestion of restarting Windows seemed to have eliminated the problem.  
 But, if I remember correctly, I did reboot the system at least once and saw the problem persisting before I made the report. I had to make some extra efforts to prepare the illustration image (<http://xxclone.com/img/dragdrop.png>) to explain what I saw.  
 While it is easy to dismiss this episode as a semi “random” behavior of an unstable machine, the computer happens to be a very stable one which seldom goes to the blue screen. So, before I forget this story, let me document what was somewhat different from my routine EmEditor operations.  
 In retrospect, I was doing something that I did not do before. That is, before I observed the strange “disallowed-drop” behavior, for the first time, I started to use the the “Projects” pane in a new (to me) way. That is, until yesterday, I always used the Visual Studio (VS2010) solution file as the starting point.  
 Yesterday, for the first time, I started to use the “Project” scheme as opposed to the “Solution” scheme. Then, I realized it is more suitable for me to create my own set of files that are relevant to a given version of my “project”. Actually, I was delighted to discover EmEditor’s “Project” scheme (.eeproj in addition to the .eesln) which was new to me yesterday. Before I started to notice the “disallowed-drop” behavior, I was playing with the feature that relates to the .eeproj file (adding, removing the member files) for several hours as part of my work.  
 So, for now, let me report that the strange observation was noticed after considerable manipulation of the Project pane’s contents while doing my own editing session. Once I noticed the “disallowed-drop”, it did no go away, not even a reboot.  
 What I’m saying is that this may never surface again. But, I have a hunch that it may be related to the way EmEditor handles the .eeproj (or .eesln) feature.  
 Thank you for your attention. If I observe something more, I will make another report in this thread.  
March 1, 2013 at 4:27 pm [#10878](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
Thanks for observation. It is possible the Projects plug-in can be something to do with the “disallowed-drop”. I will look into this issue.  
 Thanks!  
March 2, 2013 at 9:33 am [#10879](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/5e2551a06c05e17c7abab191ebd0d3f3?s=80&d=identicon&r=g)XXCloneMan](https://www.emeditor.com/forums/users/XXCloneMan/ "View XXCloneMan's profile")  
Member  
Yes. It happened again (I’m still looking at it as I write this). This always seems to happen very late at night (now, it’s 2:38 am). An interesting thing is that  
 I opened a fresh EmEditor while the misbehaving EmEditor window is still there, side-by-side (as Microsoft says “sxs” :-)  
 It is quite interesting that grabbing a text file from somewhere (usually originates at a display of TotalCommander — one of my favorite tools, but I also tried to grab a file in Windows explorer display for the same result) and then drag it over the newly opened EmEditor’s area that shows “drop-accepted” cursor and then continue fly over to the older EmEditor’s area and the cursor changes to the “drop-disallowed” shape. It reminds me of an airliner fly over a friendly country that welcomes you and then go over a hostile airspace that does not cooperate.  
 Furthermore, there is another interesting aspect of this.  
 It seems there are three types of area in EmEditor’s display area.  
 1) Top area (TitleBar, MenuBar, Toolbar and the tabarea)  
 2) Projects pane (I usually keep it at the left hand side)  
 3) The main text-editing area  
 When I drag a file over a good EmEditor display,  
 The mouse cursor always remains the “drop-accepted” shape and I can drop it at Area 1 and Area 3 that starts the editing session. But, when drop it in Area 2, depending on where to drop, it behaves differently (according to the rule that governs the Projects pane behavior which is OK).  
 Now, when I try the same thing over a misbehaving Emeditor’s display area, The top section (Area 1) shows the “drop-accepted” image — but when I drop the file there, nothing seems to happen without any error message (a black hole). Then, of course, Area 2 and Area 3 of misbehaving EmEditor give me the “drop-disallowed” cursor and obviously, nothing happens when I drop it. That is, whether the mouse cursor shows drop-accepted or drop-disaallowed, the effects are the same — no discernible action takes place.  
 Anyway, right now, I’m looking at a total of four EmEditor displays. Two of them are “misbehaviing” with the “drop-disallowed” cursor display. I sometimes open with the “-sp” switch and sometimes without. When I open a new instance of EmEditor, the new one seem to behave well.  
 …Wait. I just found something different. The problem seems to have gone while I was experimenting (as I have been wriing this report (inside the Forum section here).  
 Now, all of the EmEditor displays behaves well and I don’t have any of them that gives the “drop-disallowed” cursor.  
 So, my experiment tonight ends right now. (It’s 3:32 am and I’m going to bed — strange things happen to old men at very late night). Very spooky.  
 One more thing: Tonight, I did not play with the Project pane very much. I was mostly doing my own work (a lot of activities with several tabs open and a few separate EmEditor displays all over the two-monitor configurations— I always need more desktop!!!  
 Good night…
* Author  
Posts

Viewing 5 posts - 1 through 5 (of 5 total)

* You must be logged in to reply to this topic.

<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="autorelaxed"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="1223367746"></ins>

<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="8358498916"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>

<span class="atpl-alsoreadstyle">Also read:</span>
<div><ul>
<li><a href="https://digital-screen-recording.techidaily.com/new-in-2024-in-depth-minecraft-gameplay-recording-strategies/"><u>[New] In 2024, In-Depth Minecraft Gameplay Recording Strategies</u></a></li>
<li><a href="https://fox-helps.techidaily.com/new-in-2024-tailored-audio-connector-for-podcasting-pros/"><u>[New] In 2024, Tailored Audio Connector for Podcasting Pros</u></a></li>
<li><a href="https://some-guidance.techidaily.com/updated-ultimate-digital-lecture-name-builder/"><u>[Updated] Ultimate Digital Lecture Name Builder</u></a></li>
<li><a href="https://win-guides.techidaily.com/advanced-pro-dashboard-with-bootstrap-4-exclusive-admin-design-by-creative-tim/"><u>Advanced Pro Dashboard with Bootstrap 4: Exclusive Admin Design by Creative Tim</u></a></li>
<li><a href="https://extra-hints.techidaily.com/beginners-guide-to-visual-storytelling-key-shot-techniques/"><u>Beginner’s Guide to Visual Storytelling Key Shot Techniques</u></a></li>
<li><a href="https://win-guides.techidaily.com/build-your-own-professional-author-portfolio-using-the-premium-nextjs-and-tailwind-integration-free-template-from-creative-tim/"><u>Build Your Own Professional Author Portfolio Using the Premium NextJS and Tailwind Integration - Free Template From Creative Tim</u></a></li>
<li><a href="https://win-guides.techidaily.com/creative-tims-ultimate-horizon-ai-pro-template-pack-with-pre-configured-nextjs-includes-advanced-integration-with-stripe-and-supabase-featuring-oauth-suppor10/"><u>Creative Tim's Ultimate Horizon AI Pro Template Pack with Pre-Configured NextJS: Includes Advanced Integration with Stripe and Supabase Featuring OAuth Support</u></a></li>
<li><a href="https://technical-tips.techidaily.com/desktop-icon-disappearance-troubles-heres-how-to-fix-them-for-windows-11/"><u>Desktop Icon Disappearance Troubles? Here's How to Fix Them for Windows 11</u></a></li>
<li><a href="https://win-guides.techidaily.com/download-our-complimentary-bootstrap-based-material-design-ui-framework-from-creative-tim/"><u>Download Our Complimentary Bootstrap-Based Material Design UI Framework From Creative Tim</u></a></li>
<li><a href="https://win-guides.techidaily.com/download-your-ace-landing-page-with-free-nextjstailwind-course-from-creative-tims-resource-hub/"><u>Download Your Ace Landing Page with Free NextJS/Tailwind Course From Creative Tim's Resource Hub!</u></a></li>
<li><a href="https://technical-tips.techidaily.com/essential-free-tools-for-testing-your-hard-drives-in-july-2e-the-top-13-selections/"><u>Essential Free Tools for Testing Your Hard Drives in July 2E: The Top 13 Selections</u></a></li>
<li><a href="https://youtube-help.techidaily.com/in-2024-key-strategies-in-building-successful-youtube-shorts-templates/"><u>In 2024, Key Strategies in Building Successful YouTube Shorts Templates</u></a></li>
<li><a href="https://program-issues.techidaily.com/resolved-how-to-stop-eye-straining-flicker-on-your-display/"><u>Resolved: How to Stop Eye-Straining Flicker on Your Display</u></a></li>
<li><a href="https://program-issues.techidaily.com/troubleshooting-tips-overcoming-the-persistent-loading-hurdle-in-among-us-gameplay/"><u>Troubleshooting Tips: Overcoming the Persistent Loading Hurdle in Among Us Gameplay</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2130885/7443" target="_top" id="2130885">
  <img src="//a.impactradius-go.com/display-ad/7443-2130885" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2130885/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

