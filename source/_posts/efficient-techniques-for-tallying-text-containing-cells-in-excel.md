---
title: Efficient Techniques for Tallying Text-Containing Cells in Excel
date: 2024-12-02T16:24:17.350Z
updated: 2024-12-06T16:47:47.981Z
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/qObsqoJB9LI?si=ppqxfXzP0UL4J6Tp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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

##  Count Cells With Specific Text in Excel

 To make Excel only count the cells that contain specific text, use an argument with the `COUNTIF` function.

 First, in your spreadsheet, select the cell in which you want to display the result.

![Select a cell in an Excel spreadsheet.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/11/1-select-cell-3.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/omWG4u39lmE?si=yk1AEo_gzDpGjYbl" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 In the selected cell, type the following `COUNTIF` function and press Enter. In the function, replace `D2` and `D6` with the [range](https://video-screen-grab.techidaily.com/updated-playful-pioneers-the-kids-game-bazaar-for-2024/) where your cells are. Also, replace `a` with any character or word that your cell should have for it to be counted.

 The below function counts all cells that contain the letter `a`. This means, in our example, it will count both `Mahesh` and `David` as both these names have the letter `a` in them.

=COUNTIF(D2:D6,"*a*")

![Enter the COUNTIF function to count cells containing specific text.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/11/5-countif-count-specific-text-cells.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/43goO8X0iX0?si=48Cqf6td2q_6T6h3" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Here's the result:

![The number of cells containing specific text.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/11/6-countif-specific-text-result.png) 

 To make the function count those cells that only have your specified character or word in them, remove the \* (asterisk) sign from before and after your character or word, as follows.

=COUNTIF(D2:D6,"a")

![Enter the COUNTIF function to count cells only containing specific text.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/11/7-countif-count-only-specific-text-cells.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/hHPljBHrvkA?si=HwdfDM9rlbABSIrx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 In our example, the count result is `0` because there are no cells that only contain the character `a` in them.

![The number of cells containing only specific text.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2021/11/8-countif-only-specific-text-cell-result.png) 

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/YfEPmG_O6F8?si=93ZTVtH_zjFRz5eh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://youtube-docs.techidaily.com/ed-2024-approved-crafting-powerful-video-titles-and-sizes/"><u>[Updated] 2024 Approved Crafting Powerful Video Titles & Sizes</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-in-2024-amplify-audience-connection-best-creative-reacting-techniques/"><u>[Updated] In 2024, Amplify Audience Connection Best Creative Reacting Techniques</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/ed-in-2024-revitalize-your-routine-with-these-top-10-yoga-streams-of-note/"><u>[Updated] In 2024, Revitalize Your Routine with These Top 10 Yoga Streams of Note</u></a></li>
<li><a href="https://extra-information.techidaily.com/2024-approved-a-guide-to-writing-successful-vlogging-scripts/"><u>2024 Approved A Guide to Writing Successful Vlogging Scripts</u></a></li>
<li><a href="https://youtube-help.techidaily.com/2024-approved-optimize-your-content-searchability-with-these-7-top-tier-youtube-tags-extractor-tools/"><u>2024 Approved Optimize Your Content Searchability with These 7 Top-Tier Youtube Tags Extractor Tools</u></a></li>
<li><a href="https://win-dash.techidaily.com/addressing-and-solving-the-problem-of-missing-dts-support-in-selected-speakers-or-headphones/"><u>Addressing and Solving the Problem of Missing DTS Support in Selected Speakers or Headphones</u></a></li>
<li><a href="https://win-able.techidaily.com/battle-against-glitches-overcoming-pc-crash-issues-in-final-fantasy-xiv-online-adventures/"><u>Battle Against Glitches: Overcoming PC Crash Issues in Final Fantasy XIV Online Adventures</u></a></li>
<li><a href="https://win-able.techidaily.com/how-to-resolve-elden-rings-initial-black-screen-problem-for-a-smooth-gaming-experience/"><u>How to Resolve Elden Ring's Initial Black Screen Problem for a Smooth Gaming Experience</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/in-2024-how-to-unlock-disabled-apple-iphone-11-pro-maxipad-without-computer-drfone-by-drfone-ios/"><u>In 2024, How to Unlock Disabled Apple iPhone 11 Pro Max/iPad Without Computer | Dr.fone</u></a></li>
<li><a href="https://win-able.techidaily.com/remnant-from-the-ashes-gameplay-interrupted-heres-how-to-stop-the-crashing/"><u>Remnant: From the Ashes Gameplay Interrupted? Here's How To Stop The Crashing</u></a></li>
<li><a href="https://win-able.techidaily.com/resolve-intensive-resource-consumption-fixes-for-baldurs-gate-cuisine-usage/"><u>Resolve Intensive Resource Consumption: Fixes for Baldur's Gate Cuisine Usage</u></a></li>
<li><a href="https://win-able.techidaily.com/resolved-optimize-gaming-experience-fixing-stutter-and-boosting-fps-in-red-dead-redemption-2/"><u>Resolved: Optimize Gaming Experience - Fixing Stutter & Boosting FPS in Red Dead Redemption 2</u></a></li>
<li><a href="https://fox-search.techidaily.com/restoring-lost-files-on-windows-top-6-effective-techniques/"><u>Restoring Lost Files on Windows: Top 6 Effective Techniques</u></a></li>
<li><a href="https://win-able.techidaily.com/the-definitive-guide-to-roller-champions-cross-platform-gaming-on-your-computer-updated/"><u>The Definitive Guide to Roller Champions Cross-Platform Gaming on Your Computer (Updated )</u></a></li>
<li><a href="https://win-able.techidaily.com/whats-new-in-rainbow-six-siege-a-complete-overview/"><u>What's New in Rainbow Six Siege : A Complete Overview</u></a></li>
</ul></div>

