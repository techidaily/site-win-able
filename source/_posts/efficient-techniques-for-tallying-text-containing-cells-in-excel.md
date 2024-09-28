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


