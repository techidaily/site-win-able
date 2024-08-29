---
title: Efficient Techniques for Tallying Text-Containing Cells in Excel
date: 2024-08-28T05:22:48.104Z
updated: 2024-08-29T05:22:48.104Z
tags:
  - excel
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/09/microsoft_excel_hero_1200x675.jpg
---

## Efficient Techniques for Tallying Text-Containing Cells in Excel

### Quick Links

* [Count Cells With Any Text in Excel](https://some-approaches.techidaily.com/2024-approved-the-uav-connoisseurs-guide-to-essential-equipment/)
* [Count Cells With Specific Text in Excel](https://facebook-record-videos.techidaily.com/updated-2024-approved-discover-engaging-youtube-threads/)

 Do you want to [count the number of cells](https://howto.techidaily.com/fix-the-error-of-unfortunately-the-processcomandroidphone-has-stopped-on-vivo-v29-pro-drfone-by-drfone-fix-android-problems-fix-android-problems/) that contain any or specific text while ignoring all other cells? If so, Microsoft Excel has a dedicated function to help you do that. We'll show you how to use it.

 In Excel, you can [use the COUNTIF function](https://win-forum.techidaily.com/complete-tutorial-clearing-out-windows-10-memory-dump-data/) to count either cells containing any text or cells containing specific text. Use the method below that works for your specific situation.

##  Count Cells With Any Text in Excel

 To count the number of cells that contain any text, but ignore any numbers, blank cells, and [errors](https://ios-unlock.techidaily.com/in-2024-iphone-12-pro-asking-for-passcode-after-ios-1714-update-what-to-do-by-drfone-ios/), use the method here.

 First, open your spreadsheet with Microsoft Excel. In the spreadsheet, select the cell in which you want to display the result.

![Select a cell in an Excel spreadsheet.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/11/1-select-cell-3.png) 

 In the selected cell, type the following `COUNTIF` function and press Enter. Make sure to replace `D2` and `D6` in this function with the range where your cells to be counted are.

=COUNTIF(D2:D6,"*")

 Here, the \* (asterisk) argument tells the function to only count cells containing text.

![Enter the COUNTIF function to count all text cells.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/11/2-countif-count-text-cells.png) 

 You can also count the cells that contain anything but text. To do so, use the following modified version of the `COUNTIF` function. In this function, the argument specifies that only the non-text cells should be counted.

 If a cell has a mix of both text and numbers, it won't be counted.

=COUNTIF(D2:D6,"<>*")

![Enter the COUNTIF function to count all non-text cells.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/11/3-countif-count-non-text-cells.png) 

 This is the result you will see when you use the COUNTIF function to count the number of cells containing any text.

![The number of cells containing any text.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/11/4-countif-result.png) 

Related: [How to Highlight Blanks or Errors in Microsoft Excel](https://ios-unlock.techidaily.com/in-2024-iphone-12-pro-asking-for-passcode-after-ios-1714-update-what-to-do-by-drfone-ios/) 

<!-- affiliate ads begin -->
<a href="https://caperobbin.sjv.io/c/5597632/2006118/18460" target="_top" id="2006118"><img src="//a.impactradius-go.com/display-ad/18460-2006118" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2006118/18460" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
##  Count Cells With Specific Text in Excel

 To make Excel only count the cells that contain specific text, use an argument with the `COUNTIF` function.

 First, in your spreadsheet, select the cell in which you want to display the result.

![Select a cell in an Excel spreadsheet.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/11/1-select-cell-3.png) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=3851655&QTY=1&AFFILIATE=108875&CART=1"><img src="http://www.aiseesoft.com/avangate/30p/banner.jpg" border="0"></a>
<!-- affiliate ads end -->
 In the selected cell, type the following `COUNTIF` function and press Enter. In the function, replace `D2` and `D6` with the [range](https://video-screen-grab.techidaily.com/updated-playful-pioneers-the-kids-game-bazaar-for-2024/) where your cells are. Also, replace `a` with any character or word that your cell should have for it to be counted.

 The below function counts all cells that contain the letter `a`. This means, in our example, it will count both `Mahesh` and `David` as both these names have the letter `a` in them.

=COUNTIF(D2:D6,"*a*")

![Enter the COUNTIF function to count cells containing specific text.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/11/5-countif-count-specific-text-cells.png) 

<!-- affiliate ads begin -->
<a href="https://twopages.pxf.io/c/5597632/2016067/18544" target="_top" id="2016067"><img src="//a.impactradius-go.com/display-ad/18544-2016067" border="0" alt="" width="1020" height="380"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2016067/18544" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Here's the result:

![The number of cells containing specific text.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/11/6-countif-specific-text-result.png) 

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=45152810&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/842ca578342915ccb8ae069595ba7233/products/copy_bootit-ss1_178x139.jpg" border="0">The BootIt Collection covers multi-booting, partitioning, and disk imaging on traditional PC's using the standard BIOS and  newer PC's using UEFI.   The collection includes BootIt Bare Metal (BIBM) for standard BIOS systems and BootIt UEFI (BIU) for UEFI system. 
</a>
<!-- affiliate ads end -->
 To make the function count those cells that only have your specified character or word in them, remove the \* (asterisk) sign from before and after your character or word, as follows.

=COUNTIF(D2:D6,"a")

![Enter the COUNTIF function to count cells only containing specific text.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/11/7-countif-count-only-specific-text-cells.png) 

<!-- affiliate ads begin -->
<a href="https://tinyland.pxf.io/c/5597632/1793214/19135" target="_top" id="1793214"><img src="//a.impactradius-go.com/display-ad/19135-1793214" border="0" alt="" width="900" height="900"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793214/19135" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 In our example, the count result is `0` because there are no cells that only contain the character `a` in them.

![The number of cells containing only specific text.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/11/8-countif-only-specific-text-cell-result.png) 

<!-- affiliate ads begin -->
<a href="https://shop.systoolsgroup.com/affiliate.php?ACCOUNT=SYSTOOBY&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.systoolsgroup.com%3FAFFILIATE%3D108875%26RESOURCE%3DSysTools%2BSQL%2BRecovery"><img src="https://www.systoolsgroup.com/box/sql-recovery.png" border="0"></a>
<!-- affiliate ads end -->
 And that's how you specify what cells to consider for calculation in your Microsoft Excel spreadsheets. Very useful!

---

 Did you know Excel can also [count blank or empty cells](https://fox-blue.techidaily.com/2024-approved-revel-in-richness-your-pcs-pathway-to-exceptional-video-quality/) in your spreadsheets? Check that out if you're interested.

Related: [How to Add Text to a Cell With a Formula in Excel](https://buynow-reviews.techidaily.com/a-comprehensive-review-top-long-reach-routers-dominating-the-market-in-ebytes/)

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
<li><a href="https://youtube-sure.techidaily.com/024-approved-comedy-classics-a-curated-15-channel-collection-for-humor/"><u>[New] 2024 Approved  Comedy Classics  A Curated 15-Channel Collection for Humor</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/new-best-of-the-best-12-screen-capture-tools-no-end/"><u>[New] Best of the Best 12 Screen Capture Tools (No End)</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/new-enhancing-visual-storytelling-with-impeccable-voice-over/"><u>[New] Enhancing Visual Storytelling with Impeccable Voice Over</u></a></li>
<li><a href="https://video-capture.techidaily.com/new-in-2024-effective-webinar-logging-tips-avoiding-common-pitfalls-windows-macos/"><u>[New] In 2024, Effective Webinar Logging Tips  Avoiding Common Pitfalls (Windows, macOS)</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/new-pure-sound-capture-on-your-mac-for-2024/"><u>[New] Pure Sound Capture on Your Mac for 2024</u></a></li>
<li><a href="https://screen-recording.techidaily.com/updated-2024-approved-digging-into-sharex-assessment-and-choices/"><u>[Updated] 2024 Approved  Digging Into ShareX  Assessment & Choices</u></a></li>
<li><a href="https://eaxpv-info.techidaily.com/updated-2024-approved-giggles-galore-7-entertaining-video-sets-for-chuckleheads/"><u>[Updated] 2024 Approved  Giggles Galore  7 Entertaining Video Sets for Chuckleheads</u></a></li>
<li><a href="https://video-capture.techidaily.com/updated-2024-approved-screen-review-snapshot-is-active-8-top-tier-or-not/"><u>[Updated] 2024 Approved  Screen Review Snapshot  Is Active 8 Top-Tier or Not?</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/ed-2024-approved-your-pathway-to-a-clutter-free-device-with-video-deletion-tips/"><u>[Updated] 2024 Approved  Your Pathway to a Clutter-Free Device with Video Deletion Tips</u></a></li>
<li><a href="https://fox-access.techidaily.com/updated-in-2024-m1-pro-vs-m1-max-examining-the-advancements-in-apples-cpu-technology/"><u>[Updated] In 2024, M1 Pro Vs. M1 Max  Examining the Advancements in Apple's CPU Technology</u></a></li>
<li><a href="https://fox-links.techidaily.com/updated-precision-guide-for-subtitles-insertion-in-mp4-files/"><u>[Updated] Precision Guide for Subtitles Insertion in MP4 Files</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/2024-approved-selecting-the-perfect-screen-ultrawide-or-uhd-4k/"><u>2024 Approved  Selecting the Perfect Screen  UltraWide or UHD 4K?</u></a></li>
<li><a href="https://youtube-stream.techidaily.com/2024-approved-unlocking-potential-in-5-second-videos/"><u>2024 Approved  Unlocking Potential in 5-Second Videos</u></a></li>
<li><a href="https://fox-glue.techidaily.com/accelerated-approach-eliminating-signatures-quickly-for-2024/"><u>Accelerated Approach  Eliminating Signatures Quickly for 2024</u></a></li>
<li><a href="https://win-able.techidaily.com/banishing-the-error-effective-fixes-for-continuous-crashes-of-ready-or-not-on-desktops-and-laptops/"><u>Banishing the Error: Effective Fixes for Continuous Crashes of 'Ready or Not' On Desktops and Laptops</u></a></li>
<li><a href="https://win-able.techidaily.com/1723012777769-bypassing-error-re-establish-your-destiny-grope-with-these-fixes/"><u>Bypassing Error: Re-Establish Your Destiny Grope With These Fixes!</u></a></li>
<li><a href="https://win-able.techidaily.com/complete-troubleshooting-guide-ensuring-smooth-steam-downloads-without-interruptions/"><u>Complete Troubleshooting Guide: Ensuring Smooth Steam Downloads Without Interruptions</u></a></li>
<li><a href="https://tech-haven.techidaily.com/contrasting-snapchat-my-ai-with-bing-chat-an-in-depth-analysis-of-their-eight-major-differences-on-skype/"><u>Contrasting Snapchat My AI with Bing Chat: An In-Depth Analysis of Their Eight Major Differences on Skype</u></a></li>
<li><a href="https://win-able.techidaily.com/cut-down-discords-heavy-cpu-load-advanced-troubleshooting-techniques-for-202eby/"><u>Cut Down Discord's Heavy CPU Load: Advanced Troubleshooting Techniques for 202Eby</u></a></li>
<li><a href="https://win-able.techidaily.com/decode-the-fixes-an-authoritative-approach-to-overcoming-devastating-ark-server-crashes/"><u>Decode the Fixes: An Authoritative Approach to Overcoming Devastating ARK Server Crashes</u></a></li>
<li><a href="https://location-social.techidaily.com/does-nokia-105-classic-have-find-my-friends-drfone-by-drfone-virtual-android/"><u>Does Nokia 105 Classic Have Find My Friends? | Dr.fone</u></a></li>
<li><a href="https://win-able.techidaily.com/effortless-fixes-resolving-ghost-recon-breakpoint-sudden-crash-problems/"><u>Effortless Fixes: Resolving Ghost Recon Breakpoint Sudden Crash Problems</u></a></li>
<li><a href="https://win-able.techidaily.com/fixing-the-dark-void-resolving-cyberpunk-2077s-black-screen-issue/"><u>Fixing the Dark Void: Resolving Cyberpunk 2077'S Black Screen Issue</u></a></li>
<li><a href="https://win-able.techidaily.com/fixing-your-loss-of-access-to-blizzard-online-services/"><u>Fixing Your Loss of Access to Blizzard Online Services</u></a></li>
<li><a href="https://win-able.techidaily.com/get-final-age-running-smoothly-on-your-computer-top-fixes-and-hacks-for-a-seamless-2024/"><u>Get 'Final Age' Running Smoothly on Your Computer: Top Fixes & Hacks for a Seamless 2024</u></a></li>
<li><a href="https://win-able.techidaily.com/hogwarts-legacy-launch-troubles-top-strategies-to-overcome-game-failures/"><u>Hogwarts Legacy Launch Troubles? Top Strategies to Overcome Game Failures</u></a></li>
<li><a href="https://win-able.techidaily.com/how-to-eliminate-slow-responses-and-lag-in-lol-a-comprehensive-guide/"><u>How to Eliminate Slow Responses and Lag in LoL: A Comprehensive Guide</u></a></li>
<li><a href="https://win-able.techidaily.com/how-to-jumpstart-societal-advancement-and-fix-humans-not-launching/"><u>How To Jumpstart Societal Advancement and Fix 'Humans Not Launching'</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-recover-old-messages-from-your-infinix-note-30-pro-by-fonelab-android-recover-messages/"><u>How to recover old messages from your Infinix Note 30 Pro</u></a></li>
<li><a href="https://win-able.techidaily.com/how-to-resolve-black-ops-cold-wars-troublesome-error-0xc00e0005/"><u>How to Resolve Black Ops Cold War's Troublesome Error 0XC00e0005</u></a></li>
<li><a href="https://android-transfer.techidaily.com/in-2024-4-ways-to-transfer-music-from-xiaomi-redmi-k70-to-iphone-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>In 2024, 4 Ways to Transfer Music from Xiaomi Redmi K70 to iPhone | Dr.fone</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/in-2024-how-many-attempts-to-unlock-apple-iphone-6-by-drfone-ios/"><u>In 2024, How Many Attempts To Unlock Apple iPhone 6</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-latest-way-to-get-shiny-meltan-box-in-pokemon-go-mystery-box-on-oppo-reno-10-pro-5g-drfone-by-drfone-virtual-android/"><u>In 2024, Latest way to get Shiny Meltan Box in Pokémon Go Mystery Box On Oppo Reno 10 Pro 5G | Dr.fone</u></a></li>
<li><a href="https://win-able.techidaily.com/1723009103402-lost-ark-performance-optimization-for-windows-users-say-goodbye-to-game-interruptions/"><u>Lost Ark Performance Optimization for Windows Users: Say Goodbye to Game Interruptions!</u></a></li>
<li><a href="https://win-able.techidaily.com/mastering-gameplay-smoothness-how-to-eliminate-unresponsive-behavior-and-freezes-in-pubg-for-optimal-pc-gaming-experience/"><u>Mastering Gameplay Smoothness: How To Eliminate Unresponsive Behavior & Freezes in PUBG for Optimal PC Gaming Experience</u></a></li>
<li><a href="https://win-able.techidaily.com/maximize-call-of-duty-warzone-gameplay-by-activating-your-gpu-on-windows-10/"><u>Maximize Call of Duty: Warzone Gameplay by Activating Your GPU on Windows 10</u></a></li>
<li><a href="https://win-able.techidaily.com/no-more-gray-screens-resolving-halo-infinites-black-screen-error/"><u>No More Gray Screens: Resolving Halo Infinite’s Black Screen Error</u></a></li>
<li><a href="https://win-able.techidaily.com/overcome-the-hurdle-resolving-windows-10s-critical-error-code-0xc19001e1/"><u>Overcome the Hurdle: Resolving Windows 10'S Critical Error Code 0xC19001E1</u></a></li>
<li><a href="https://win-able.techidaily.com/resolve-connection-glitches-in-apex-legends-with-these-tips/"><u>Resolve Connection Glitches in Apex Legends with These Tips</u></a></li>
<li><a href="https://win-able.techidaily.com/resolving-issues-with-non-delivery-of-skype-messages-a-comprehensive-guide/"><u>Resolving Issues with Non-Delivery of Skype Messages: A Comprehensive Guide</u></a></li>
<li><a href="https://win-able.techidaily.com/resolving-issues-with-the-msi-afterburner-monitoring-software/"><u>Resolving Issues with the MSI Afterburner Monitoring Software</u></a></li>
<li><a href="https://win-able.techidaily.com/resolving-valheims-launch-problem-for-seamless-gameplay/"><u>Resolving Valheim's Launch Problem for Seamless Gameplay</u></a></li>
<li><a href="https://win-able.techidaily.com/reviving-the-sounds-of-tamriel-solutions-for-skyrims-muted-woes/"><u>Reviving the Sounds of Tamriel: Solutions for Skyrim's Muted Woes</u></a></li>
<li><a href="https://vp-tips.techidaily.com/selecting-sacred-songs-for-smartphone-users-for-2024/"><u>Selecting Sacred Songs for Smartphone Users for 2024</u></a></li>
<li><a href="https://location-social.techidaily.com/set-your-preferred-job-location-on-linkedin-app-of-your-oppo-a56s-5g-drfone-by-drfone-virtual-android/"><u>Set Your Preferred Job Location on LinkedIn App of your Oppo A56s 5G | Dr.fone</u></a></li>
<li><a href="https://win-able.techidaily.com/solution-found-fixes-two-point-fall-in-pc-games-frame-rate-performance/"><u>Solution Found! Fixes Two-Point Fall in PC Game's Frame Rate Performance</u></a></li>
<li><a href="https://win-able.techidaily.com/solve-fortnite-video-memory-crash-effective-fixes-and-workarounds/"><u>Solve Fortnite Video Memory Crash: Effective Fixes & Workarounds</u></a></li>
<li><a href="https://win-able.techidaily.com/solving-pc-issues-in-armored-core-6-navigating-the-rubicon-fire/"><u>Solving PC Issues in Armored Core 6: Navigating the Rubicon Fire</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/syncing-songs-to-social-networks-iphonesandroid-approach/"><u>Syncing Songs to Social Networks  IPhones/Android Approach</u></a></li>
<li><a href="https://buynow-reviews.techidaily.com/the-ultimate-guide-to-choosing-a-twelve-south-bookbook-v2-protective-case-for-your-macbook/"><u>The Ultimate Guide to Choosing a Twelve South BookBook V2 Protective Case for Your MacBook</u></a></li>
<li><a href="https://buynow-marvelous.techidaily.com/thermopro-tp67-analysis-cost-effective-yet-inconsistent-performance/"><u>ThermoPro TP67 Analysis: Cost-Effective Yet Inconsistent Performance</u></a></li>
<li><a href="https://win-able.techidaily.com/troubleshoot-fortnite-play-errors-with-this-simple-permission-denied-fix/"><u>Troubleshoot Fortnite Play Errors with This Simple 'Permission Denied' Fix</u></a></li>
<li><a href="https://win-able.techidaily.com/troubleshooting-fix-how-to-resolve-issues-with-tribes-of-midgard-game-crashes/"><u>Troubleshooting Fix: How to Resolve Issues with 'Tribes of Midgard' Game Crashes</u></a></li>
<li><a href="https://win-able.techidaily.com/troubleshooting-steps-for-resolving-issues-with-corsair-icue-on-windows-1011/"><u>Troubleshooting Steps for Resolving Issues with Corsair iCUE on Windows 10/11</u></a></li>
<li><a href="https://win-answers.techidaily.com/troubleshooting-the-black-startup-error-in-rainbow-six-siege-for-windows-computers/"><u>Troubleshooting the Black Startup Error in Rainbow Six Siege for Windows Computers</u></a></li>
<li><a href="https://win-able.techidaily.com/unlocking-the-secrets-behind-alan-wake-2s-postponed-debut/"><u>Unlocking The Secrets Behind Alan Wake 2'S Postponed Debut</u></a></li>
<li><a href="https://tech-haven.techidaily.com/why-more-ai-rules-insights-from-openais-chief-executive/"><u>Why More AI Rules? - Insights From OpenAI's Chief Executive</u></a></li>
<li><a href="https://common-error.techidaily.com/winning-against-the-ruby-display-glitch-on-your-windows-11-computer/"><u>Winning Against the Ruby Display Glitch on Your Windows 11 Computer</u></a></li>
</ul></div>
