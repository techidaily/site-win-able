---
title: "Excel's Powerful Lookup Function: Mastering VLOOKUP Without an External Table"
date: 2024-08-28T05:22:51.664Z
updated: 2024-08-29T05:22:51.664Z
tags:
  - excel
categories:
  - tech
thumbnail: https://thmb.techidaily.com/89da125ea493abc275649c1f57ef017273ab0d0d83c11a51da5e1af69c65adca.png
---

## Excel's Powerful Lookup Function: Mastering VLOOKUP Without an External Table

In a recent article, we introduced the Excel function called **VLOOKUP** and explained how it could be used to retrieve information from a database into a cell in a local worksheet. In that article we mentioned that there were two uses for VLOOKUP, and only one of them dealt with querying databases. In this article, the second and final in the VLOOKUP series, we examine this other, lesser known use for the VLOOKUP function. If you haven't already done so, please read [the first VLOOKUP article](https://extra-tips.techidaily.com/integrate-sound-and-sight-web-studio/) \- this article will assume that many of the concepts explained in that article are already known to the reader. When working with databases, VLOOKUP is passed a "unique identifier" that serves to identify which data record we wish to find in the database (e.g. a product code or customer ID). This unique identifier must exist in the database, otherwise VLOOKUP returns us an error. In this article, we will examine a way of using VLOOKUP where the identifier doesn't need to exist in the database at all. It's almost as if VLOOKUP can adopt a "near enough is good enough" approach to returning the data we're looking for. In certain circumstances, this is exactly what we need. We will illustrate this article with a real-world example - that of calculating the commissions that are generated on a set of sales figures. We will start with a very simple scenario, and then progressively make it more complex, until the only rational solution to the problem is to use VLOOKUP. The initial scenario in our fictitious company works like this: If a salesperson creates more than $30,000 worth of sales in a given year, the commission they earn on those sales is 30%. Otherwise their commission is only 20%. So far this is a pretty simple worksheet: To use this worksheet, the salesperson enters their sales figures in cell B1, and the formula in cell B2 calculates the correct commission rate they are entitled to receive, which is used in cell B3 to calculate the total commission that the salesperson is owed (which is a simple multiplication of B1 and B2). The cell B2 contains the only interesting part of this worksheet - the formula for deciding which commission rate to use: the one below the threshold of $30,000, or the one above the threshold. This formula makes use of the Excel function called **IF**. For those readers that are not familiar with IF, it works like this: 

> IF(condition,value if true,value if false)

 Where the condition is an expression that evaluates to either **true** or **false**. In the example above, the condition is the expression **B1<B5**, which can be read as "Is B1 less than B5?", or, put another way, "Are the total sales less than the threshold". If the answer to this question is "yes" (true), then we use the value if true parameter of the function, namely **B6** in this case - the commission rate if the sales total was below the threshold. If the answer to the question is "no" (false), then we use the value if false parameter of the function, namely **B7** in this case - the commission rate if the sales total was above the threshold. As you can see, using a sales total of $20,000 gives us a commission rate of 20% in cell B2\. If we enter a value of $40,000, we get a different commission rate: 

![original40k](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2010/04/original40k.png) 

 So our spreadsheet is working. Let's make it more complex. Let's introduce a second threshold: If the salesperson earns more than $40,000, then their commission rate increases to 40%: 

![2thresholds](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2010/04/2thresholds.png) 

 Easy enough to understand in the real world, but in cell B2 our formula is getting more complex. If you look closely at the formula, you'll see that the third parameter of the original IF function (the value if false) is now an entire IF function in its own right. This is called a nested function (a function within a function). It's perfectly valid in Excel (it even works!), but it's harder to read and understand. We're not going to go into the nuts and bolts of how and why this works, nor will we examine the nuances of nested functions. This is a tutorial on VLOOKUP, not on Excel in general. Anyway, it gets worse! What about when we decide that if they earn more than $50,000 then they're entitled to 50% commission, and if they earn more than $60,000 then they're entitled to 60% commission? 

![4thresholds](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2010/04/4thresholds.png) 

 Now the formula in cell B2, while correct, has become virtually unreadable. No-one should have to write formulae where the functions are nested four levels deep! Surely there must be a simpler way? There certainly is. VLOOKUP to the rescue! Let's redesign the worksheet a bit. We'll keep all the same figures, but organize it in a new way, a more tabular way: 

![tableblank](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2010/04/tableblank.png) 

 Take a moment and verify for yourself that the new **Rate Table** works exactly the same as the series of thresholds above. Conceptually, what we're about to do is use VLOOKUP to look up the salesperson's sales total (from B1) in the rate table and return to us the corresponding commission rate. Note that the salesperson may have indeed created sales that are not one of the five values in the rate table ($0, $30,000, $40,000, $50,000 or $60,000). They may have created sales of $34,988\. It's important to note that $34,988 does not appear in the rate table. Let's see if VLOOKUP can solve our problem anyway... We select cell B2 (the location we want to put our formula), and then insert the VLOOKUP function from the **Formulas** tab: 

![findfunc](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2010/04/findfunc.png) 

 The **Function Arguments** box for VLOOKUP appears. We fill in the arguments (parameters) one by one, starting with the **Lookup\_value**, which is, in this case, the sales total from cell B1\. We place the cursor in the **Lookup\_value** field and then click once on cell B1: 

![args1](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2010/04/args1.png) 

 Next we need to specify to VLOOKUP what table to lookup this data in. In this example, it's the rate table, of course. We place the cursor in the **Table\_array** field, and then highlight the entire rate table - excluding the headings: 

![args2](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2010/04/args2.png) 

 Next we must specify which column in the table contains the information we want our formula to return to us. In this case we want the commission rate, which is found in the second column in the table, so we therefore enter a **2** into the **Col\_index\_num** field: 

![args3](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2010/04/args3.png) 

 Finally we enter a value in the **Range\_lookup** field. Important: It is the use of this field that differentiates the two ways of using VLOOKUP. To use VLOOKUP with a database, this final parameter, **Range\_lookup**, must always be set to **FALSE**, but with this other use of VLOOKUP, we must either leave it blank or enter a value of **TRUE**. When using VLOOKUP, it is vital that you make the correct choice for this final parameter. To be explicit, we will enter a value of **true** in the **Range\_lookup** field. It would also be fine to leave it blank, as this is the default value: 

![args4](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2010/04/args4.png) 

 We have completed all the parameters. We now click the **OK** button, and Excel builds our VLOOKUP formula for us: 

![vlookupdone](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2010/04/vlookupdone.png) 

 If we experiment with a few different sales total amounts, we can satisfy ourselves that the formula is working. **Conclusion** In the "database" version of VLOOKUP, where the **Range\_lookup** parameter is **FALSE**, the value passed in the first parameter (**Lookup\_value**) must be present in the database. In other words, we're looking for an exact match. But in this other use of VLOOKUP, we are not necessarily looking for an exact match. In this case, "near enough is good enough". But what do we mean by "near enough"? Let's use an example: When searching for a commission rate on a sales total of $34,988, our VLOOKUP formula will return us a value of 30%, which is the correct answer. Why did it choose the row in the table containing 30% ? What, in fact, does "near enough" mean in this case? Let's be precise: 

> When **Range\_lookup** is set to **TRUE** (or omitted), VLOOKUP will look in column 1 and match the highest value that is not greater than the **Lookup\_value** parameter.

 It's also important to note that for this system to work, the table must be sorted in ascending order on column 1! If you would like to practice with VLOOKUP, the sample file illustrated in this article can be downloaded from [here](https://extra-guidance.techidaily.com/new-orchestrating-originality-top-8-schools-for-story-innovation/).

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
<li><a href="https://screen-activity-recording.techidaily.com/new-2024-approved-audio-capture-system-testing-guide/"><u>[New] 2024 Approved  Audio Capture System Testing Guide</u></a></li>
<li><a href="https://youtube-blog.techidaily.com/024-approved-the-science-of-visual-appeal-crafting-stunning-youtube-shorts-templates/"><u>[New] 2024 Approved  The Science of Visual Appeal  Crafting Stunning YouTube Shorts Templates</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/new-in-2024-make-every-story-stand-out-6-top-rated-apps-for-android-and-iphone/"><u>[New] In 2024, Make Every Story Stand Out  6 Top-Rated Apps for Android & iPhone</u></a></li>
<li><a href="https://youtube-web.techidaily.com/ersonalize-your-soundtrack-constructing-a-youtube-playlist-from-home-and-on-the-move/"><u>[New] Personalize Your Soundtrack  Constructing a YouTube Playlist From Home & On-the-Move</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/ecording-sound-wonders-without-the-use-of-a-microphone/"><u>[New] Recording Sound Wonders  Without the Use of a Microphone</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/updated-in-2024-expert-strategies-for-choosing-ideal-youtube-banner-dimensions/"><u>[Updated] In 2024, Expert Strategies for Choosing Ideal YouTube Banner Dimensions</u></a></li>
<li><a href="https://win-able.techidaily.com/batman-arkham-knight-stutter-free-gaming-guide-how-to-fix-critical-malfunctions-quickly/"><u>Batman: Arkham Knight Stutter-Free Gaming Guide: How to Fix Critical Malfunctions Quickly</u></a></li>
<li><a href="https://win-able.techidaily.com/beat-maplestory-bugs-a-comprehensive-fix-guide-for-players-using-windows-11/"><u>Beat MapleStory Bugs : A Comprehensive Fix Guide for Players Using Windows 11</u></a></li>
<li><a href="https://buynow-tips.techidaily.com/comprehensive-review-of-amazonbasics-versatile-7-port-usb-30-multiport-adapter/"><u>Comprehensive Review of AmazonBasics' Versatile 7-Port USB 3.0 Multiport Adapter</u></a></li>
<li><a href="https://win-able.techidaily.com/discord-display-troubles-fixing-screen-sharing-issues-that-cause-a-black-outage-on-screens/"><u>Discord Display Troubles: Fixing Screen Sharing Issues That Cause a Black Outage on Screens</u></a></li>
<li><a href="https://win-able.techidaily.com/echoes-lost-voices-found-correcting-fallout-amoanqf4-no-output-problems-on-desktop/"><u>Echoes Lost, Voices Found: Correcting Fallout Amoanqf4 No Output Problems on Desktop</u></a></li>
<li><a href="https://win-able.techidaily.com/fixes-implemented-for-seamless-play-r-type-final-2-now-stable-on-windows-machines/"><u>Fixes Implemented for Seamless Play - R-Type Final 2 Now Stable on Windows Machines</u></a></li>
<li><a href="https://win-able.techidaily.com/fixing-the-dota-2-vac-ban-glitch-a-comprehensive-guide/"><u>Fixing the DotA 2 VAC Ban Glitch : A Comprehensive Guide</u></a></li>
<li><a href="https://win-able.techidaily.com/how-to-address-and-fix-no-ping-to-halos-data-centers-error-a-step-by-step-guide/"><u>How to Address and Fix 'No Ping to Halo's Data Centers' Error - A Step-by-Step Guide</u></a></li>
<li><a href="https://apple-account.techidaily.com/how-to-reset-apple-id-and-apple-password-on-apple-iphone-7-plus-by-drfone-ios/"><u>How to Reset Apple ID and Apple Password On Apple iPhone 7 Plus</u></a></li>
<li><a href="https://win-able.techidaily.com/how-to-resolve-continuous-crashes-in-elex-ii-on-your-computer/"><u>How to Resolve Continuous Crashes in Elex II on Your Computer</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-easily-unlock-your-xiaomi-redmi-note-12-4g-device-sim-by-drfone-android/"><u>In 2024, Easily Unlock Your Xiaomi Redmi Note 12 4G Device SIM</u></a></li>
<li><a href="https://apple-account.techidaily.com/in-2024-how-to-fix-when-apple-account-locked-on-apple-iphone-se-by-drfone-ios/"><u>In 2024, How to Fix when Apple Account Locked On Apple iPhone SE?</u></a></li>
<li><a href="https://android-transfer.techidaily.com/in-2024-how-to-transfer-apps-from-tecno-spark-go-2023-to-another-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>In 2024, How to Transfer Apps from Tecno Spark Go (2023) to Another | Dr.fone</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/in-2024-master-image-enhancement-10-pro-tips-for-using-pixlr-effectively/"><u>In 2024, Master Image Enhancement  10 Pro Tips for Using Pixlr Effectively</u></a></li>
<li><a href="https://win-able.techidaily.com/master-assassins-creed-odyssey-stability-expert-troubleshooting-tips/"><u>Master Assassin's Creed Odyssey Stability : Expert Troubleshooting Tips</u></a></li>
<li><a href="https://win-able.techidaily.com/mastering-the-witcher-3-on-pc-fixing-and-avoiding-frustrating-game-crashes/"><u>Mastering The Witcher 3 on PC: Fixing and Avoiding Frustrating Game Crashes</u></a></li>
<li><a href="https://win-able.techidaily.com/1723013063903-minecraft-network-troubles-heres-how-to-re-establish-connection/"><u>Minecraft Network Troubles? Here’s How to Re-Establish Connection</u></a></li>
<li><a href="https://win-able.techidaily.com/overcome-2024s-common-fortnite-game-crashes-on-your-pc-with-these-expert-tips/"><u>Overcome 2024'S Common Fortnite Game Crashes on Your PC with These Expert Tips</u></a></li>
<li><a href="https://win-able.techidaily.com/overcoming-compatibility-hurdles-making-logitech-options-work-seamlessly-in-windows-environment/"><u>Overcoming Compatibility Hurdles: Making Logitech Options Work Seamlessly in Windows Environment</u></a></li>
<li><a href="https://win-able.techidaily.com/overcoming-new-gen-game-latency-a-comprehensive-guide-for-smooth-play/"><u>Overcoming New-Gen Game Latency: A Comprehensive Guide for Smooth Play</u></a></li>
<li><a href="https://win-able.techidaily.com/resolved-common-fixes-for-when-fifa-21-doesnt-open-on-your-pcconsole/"><u>Resolved: Common Fixes for When FIFA 21 Doesn't Open on Your PC/Console</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/revolutionize-your-memes-with-these-7-top-gif-creation-techniques-for-2024/"><u>Revolutionize Your Memes with These 7 Top GIF Creation Techniques for 2024</u></a></li>
<li><a href="https://win-able.techidaily.com/say-goodbye-to-rocket-league-freezing-issues-fixes-and-tips-for-optimal-gameplay/"><u>Say Goodbye to Rocket League Freezing Issues: Fixes and Tips for Optimal Gameplay</u></a></li>
<li><a href="https://win-able.techidaily.com/soil-testing-identifies-specific-soil-needs-allowing-for-targeted-amendments-which-improves-crop-yields-reduces-waste-and-minimizes-environmental-harm-from-613/"><u>Soil Testing Identifies Specific Soil Needs, Allowing for Targeted Amendments, Which Improves Crop Yields, Reduces Waste, and Minimizes Environmental Harm From Over-Fertilization.</u></a></li>
<li><a href="https://win-able.techidaily.com/troubleshooting-the-redred2-errgfxstate-issue-a-comprehensive-guide/"><u>Troubleshooting the RED_RED2 ERR_GFX_STATE Issue: A Comprehensive Guide</u></a></li>
<li><a href="https://win-able.techidaily.com/vanguard-initialization-errors-addressed-a-step-by-step-resolution-for-valorant-players/"><u>Vanguard Initialization Errors Addressed: A Step-by-Step Resolution for Valorant Players</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://purchase.swifdoo.com/order/checkout.php?PRODS=40002162&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/8b932759a5a04ddb34bf79e3f9072e4b/products/1_Product%20box%20white-1024x1024.png" border="0">SwifDoo PDF Perpetual (1 PC) Free upgrade. No monthly fees ever. 
</a>
<!-- affiliate ads end -->