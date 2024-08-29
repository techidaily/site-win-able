---
title: "Unlocking Excel's Secrets: 11 Uncommon Yet Essential Features for Enhanced Efficiency"
date: 2024-08-26 14:44:18
updated: 2024-08-29 11:40:56
tags:
  - excel
categories:
  - tech
thumbnail: https://thmb.techidaily.com/2dd3f6016f2ac6912827509209a1009782287114c5fe49411fd5c4ce5c94643b.jpg
---

## Unlocking Excel's Secrets: 11 Uncommon Yet Essential Features for Enhanced Efficiency

### Quick Links

* [FLOOR and CEILING for Rounding](https://instagram-video-recordings.techidaily.com/updated-in-2024-tailoring-your-videography-with-personalized-instagram-captions/)
* [MODE.SNGL for Finding Repetitive Values](https://youtube-help.techidaily.com/new-navigate-your-way-to-partner-status-via-a-quick-10k-view-achievement/)
* [CONVERT for Converting From One Measurement to Another](https://extra-resources.techidaily.com/updated-10-best-screenshot-enhancers-iphoneandroid-sticker-magic/)
* [DELTA for Testing Equal or Not Equal Values](https://youtube-clips.techidaily.com/dive-into-diy-the-beginners-guide-to-eye-catching-mac-videos/)
* [GESTEP for Testing Greater Than or Equal To a Threshold](https://hardware-updates.techidaily.com/amd-collaborates-with-board-vendors-for-new-bios-fixes-addressing-notorious-logo-bug-concerns/)
* [ADDRESS for Finding the Location of a Cell](https://facebook-videos.techidaily.com/new-2024-approved-social-media-connectivity-embedding-live-streams-from-twitch-to-fb/)
* [PI for the Value of Pi](https://screen-video-capture.techidaily.com/2024-approved-screenshot-expert-evaluator/)
* [ARABIC and ROMAN for Converting Numerals](https://location-social.techidaily.com/how-to-changefake-your-realme-v30-location-on-viber-drfone-by-drfone-virtual-android/)
* [REPT for Entering Repeating Text](https://on-screen-recording.techidaily.com/the-most-advanced-virtual-classrooms-not-udemys-offspring/)

 Microsoft Excel offers [hundreds of functions](https://win11.techidaily.com/renaissance-pc-refresh-with-atlasos/). So, there's bound to be at least a handful you don't know exist. These unique functions have specific purposes that you'll be thrilled to learn about and use.

Related: [12 Basic Excel Functions Everybody Should Know](https://visual-screen-recording.techidaily.com/in-2024-a-step-by-step-recorder-for-discord-enthusiasts/) 

##  FLOOR and CEILING for Rounding

 You can use the FLOOR and CEILING math [functions for rounding](https://youtube-zero.techidaily.com/ed-2024-approved-the-quick-pathway-to-establishing-a-video-channel-on-your-phone/) towards or away from zero by a specified multiple. Use FLOOR to round down and CEILING to round up.

 The syntax for each is 

        `FLOOR(value, multiple)`
    
 and 

        `CEILING(value, multiple)`
    
 where both arguments are required.

 To round 4.4 down to the nearest multiple of 2, you'd use the following formula:

=FLOOR(4.4,2)

![FLOOR function in Excel](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/Floor-ExcelFunctionsLittleKnown.png) 

 To round 5.6 up to the nearest multiple of 2, you'd use this formula:

=CEILING(5.6,2)

![CEILING function in Excel](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/Ceiling-ExcelFunctionsLittleKnown.png) 

##  MODE.SNGL for Finding Repetitive Values

 Originally simply the [MODE function](https://support.microsoft.com/en-us/office/mode-function-e45192ce-9122-4980-82ed-4bdc34973120), Microsoft created a newer version of this statistical function for improved accuracy. Use MODE.SNGL to find a single frequently recurring number in an array or cell range.

 The syntax is `MODE.SNGL(array1, array2, ...)` where only the first argument is required. You can use numbers, names, arrays, or references that contain numbers. Use the optional argument(s) for additional cell ranges.

 Here, we look for the repetitive number that appears the most in cells A1 through A5.

=MODE.SNGL(A1:A5)

![MODE.SNGL function for one array](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/ModeSnglArray-ExcelFunctionsLittleKnown.png) 

 To find a recurring number in A1 through A5 and C1 through C5, you'd use this formula:

=MODE.SNGL(A1:A5, C1:C5)

![MODE.SNGL function for two arrays](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/ModeSnglArrays-ExcelFunctionsLittleKnown.png) 

##  CONVERT for Converting From One Measurement to Another

 For a useful engineering function, you can [use CONVERT](https://discord-videos.techidaily.com/mastering-discord-speaking-tts-basics-guide-for-2024/) to change a value from one measurement system to another.

Related: [How to Convert Almost Any Unit in Microsoft Excel](https://discord-videos.techidaily.com/mastering-discord-speaking-tts-basics-guide-for-2024/) 

 The syntax is `CONVERT(value, from, to)` where you'll need all three arguments. For the `from` and `to` arguments, you'll use an abbreviation. Check the [Microsoft Support site for the abbreviations](https://support.microsoft.com/en-us/office/convert-function-d785bef1-808e-4aac-bdcd-666c810f9af2) you need for weight and mass, distance, time, pressure, force, energy, power, magnetism, temperature, volume, area, information, and speed.

 To convert the value in cell A1 from Celsius to Fahrenheit, you would use this formula:

=CONVERT(A1,"C","F")

![CONVERT function for Celsius to Fahrenheit](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/ConvertTemp-ExcelFunctionsLittleKnown.png) 

 To convert the value in cell B1 from centimeters to inches, use this formula:

=CONVERT(B1,"cm","in")

![CONVERT function for centimeters to inches](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/ConvertLength-ExcelFunctionsLittleKnown.png) 

##  DELTA for Testing Equal or Not Equal Values

 Another engineering function that's useful is DELTA. With it, you'll use the [Kronecker delta](https://mathworld.wolfram.com/KroneckerDelta.html) function to test whether two values are equal. Different than the [EXACT function](https://support.microsoft.com/en-us/office/exact-function-d3087698-fc15-4a15-9631-12575cf29926), the result is either 1 (true) or 0 (false).

 The syntax is `DELTA(value1, value2)` where only the first argument is required and can be a number or cell reference. If you leave the second argument blank, Excel assumes zero.

 To test the values in cells A1 and B1, you would enter this formula:

=DELTA(A1,B1)

![DELTA function using cell references](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/DeltaCells-ExcelFunctionsLittleKnown.png) 

 To test the values 2 and -2, use this formula:

=DELTA(2,-2)

![DELTA function using numbers](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/DeltaNumber-ExcelFunctionsLittleKnown.png) 

##  GESTEP for Testing Greater Than or Equal To a Threshold

 One more engineering function you may find useful is GESTEP which allows you to test values that are [greater than or equal to](https://buynow-reviews.techidaily.com/easy-steps-to-activate-your-own-nintendo-network-id-on-the-nintendo-3ds-handheld-system/) a step (threshold). The result is either 1 (true) or 0 (false).

 The syntax is `GESTEP(value, step)` where only the first argument is required and can be a number or cell reference. If you leave the second argument blank, Excel uses zero.

 To test the value in cell A1 against step 4, you'd use this formula:

=GESTEP(A1,4)

![GESTEP function using a cell references](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/GestepCell-ExcelFunctionsLittleKnown.png) 

 To test a value of 10 against step 12, use this formula:

=GESTEP(10,12)

![GESTEP function using a number](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/GestepNumbers-ExcelFunctionsLittleKnown.png) 

##  ADDRESS for Finding the Location of a Cell

 Let's move on to a lookup function in Excel. To find the exact address of a cell, you can use the ADDRESS function. This is convenient if you want an error-free [reference to a cell](https://extra-information.techidaily.com/in-2024-chic-coverage-for-your-portable-screen/).

Related: [How to Cross Reference Cells Between Microsoft Excel Spreadsheets](https://extra-information.techidaily.com/in-2024-chic-coverage-for-your-portable-screen/) 

 The syntax is `ADDRESS(row, column, type, style, name)` where only the first two arguments are required. Enter the row number for the first argument and the column number for the second.

 The optional arguments are as follows:

* **Type**: The type of reference to return. Use blank or 1 for absolute, 2 for absolute row and relative column, 3 for relative row and absolute column, or 4 for relative.
* **Style**: Use TRUE for the A1 or FALSE for the R1C1 [cell reference style](https://facebook-video-content.techidaily.com/new-in-2024-curated-list-of-top-20-prison-jail-memes-boosting-morale-on-social-platforms/).
* **Name**: The sheet name to use for an external reference. If blank, Excel assumes the currently active sheet.

 To find the address of the cell in row 2, column 3, you'd use this formula:

=ADDRESS(2,3)

![ADDRESS function in Excel](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/AddressFunction-ExcelFunctionsLittleKnown.png) 

 To find the address of the same cell using an absolute row and relative column, you'd use this formula:

=ADDRESS(2,3,2)

![ADDRESS function with an argument in Excel](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/AddressFunctionArgument-ExcelFunctionsLittleKnown.png) 

 To find the address of the same cell in the sheet named Sheet2, use the following formula. Note that the commas represent the blank arguments `type` and `style`.

=ADDRESS(2,3,,,"Sheet2")

![ADDRESS function with a sheet name in Excel](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/AddressSheet-ExcelFunctionsLittleKnown.png) 

##  PI for the Value of Pi

 If you need to use the value of pi for equations in your sheet, you can obtain it with the PI function.

 The syntax is simply `PI()` with no arguments. You can add more [elements to the formula](https://youtube-docs.techidaily.com/n-2024-automate-playlist-retrieval-from-youtube-directly/) if you want to use the value for a calculation.

 To return the value of pi, simply use the function's formula including the parentheses:

=PI()

![PI function in Excel](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/Pi-ExcelFunctionsLittleKnown.png) 

 To multiply the value of pi by 10, you'd use this formula:

=PI()*10

![PI function times ten in Excel](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/Pi10-ExcelFunctionsLittleKnown.png) 

##  ARABIC and ROMAN for Converting Numerals

 Another math function you may find handy is for converting to and from [Arabic](https://en.wikipedia.org/wiki/Arabic%5Fnumerals) and [Roman numerals](https://en.wikipedia.org/wiki/Roman%5Fnumerals).

 The syntax for each is `ARABIC(text)` and `ROMAN(value, form)` where the first argument is required for each.

 The optional argument for the ROMAN function specifies the type of Roman numeral from Classic to Simplified. Enter the number 0, word TRUE, or omit the argument for Classic. Use a 1, 2, or 3 for a more concise result. Or, enter the number 4 or the word FALSE for Simplified.

 To convert the Roman numeral MMIM to an Arabic number, use this formula making sure to include the text in quotes:

=ARABIC("MMIM")

![ARABIC function in Excel](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/Arabic-ExcelFunctionsLittleKnown.png) 

 To convert 2,999 to a Roman numeral, you'd use this formula:

=ROMAN(2999)

![ROMAN function in Excel](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/Roman-ExcelFunctionsLittleKnown.png) 

 To convert the same number in Simplified form, use one of these formulas:

=ROMAN(2999,4)

=ROMAN(2999,FALSE)

![ROMAN function with an argument](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/RomanArgument-ExcelFunctionsLittleKnown.png) 

##  REPT for Entering Repeating Text

 If you want to add a series of characters, symbols, or text as a placeholder or for a visual effect, use the REPT [text function](https://video-screen-grab.techidaily.com/updated-the-art-of-smooth-video-transitioning-for-2024/).

Related: [How to Add Text to a Cell With a Formula in Excel](https://buynow-reviews.techidaily.com/a-comprehensive-review-top-long-reach-routers-dominating-the-market-in-ebytes/) 

 The syntax is `REPT(text, number)` where both arguments are required. Enter the text argument within quotes and then the number of times to repeat that text.

 To repeat the word Excel 10 times in a cell, you'd use this formula:

=REPT("Excel",10)

![REPT function for the word Excel](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/ReptExcel-ExcelFunctionsLittleKnown.png) 

 To repeat an asterisk 20 times, you'd use this formula:

=REPT("*",20)

![REPT function for asterisks](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2022/12/ReptAsterisk-ExcelFunctionsLittleKnown.png) 

 We've covered many [Excel functions](https://extra-lessons.techidaily.com/kickstart-your-telegram-promotion-journey-tips-for-newbies/) at How-To Geek and try to walk you through using the most common options. Hopefully one of these out-of-the-ordinary functions is exactly what you need for math, engineering, statistical, lookup, or textual data.

| |  Mastering Excel Functions |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |  |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |  |
| Functions                    | [AVERAGE](https://win-able.techidaily.com/fixing-overwatch-startup-issues-how-to-get-rid-of-the-persistent-black-screen/) **·** [CONCATENATE](https://fake-location.techidaily.com/is-pgsharp-legal-when-you-are-playing-pokemon-on-xiaomi-redmi-13c-5g-drfone-by-drfone-virtual-android/) **·** [COUNT](https://android-location-track.techidaily.com/how-to-track-a-lost-xiaomi-redmi-note-12t-pro-for-free-drfone-by-drfone-virtual-android/) **·** [COUNTIF](https://win-forum.techidaily.com/complete-tutorial-clearing-out-windows-10-memory-dump-data/) **·** [DATEDIF](https://youtube-data.techidaily.com/n-2024-explore-the-best-historian-content-top-10-youtube-recommendations/) **·** [FILTER](https://youtube-sure.techidaily.com/024-approved-the-ultimate-guide-to-youtube-live-streaming/) **·** [FREQUENCY](https://digital-screen-recording.techidaily.com/new-ideal-low-impact-recording-devices-for-eco-conscious-filmmakers/) **·** [FV](https://on-screen-recording.techidaily.com/updated-2024-approved-enhancing-gaming-experience-with-steam-switch-control/) **·** [HYPERLINK](https://some-guidance.techidaily.com/updated-the-minimalists-guide-to-aerial-imagery-with-dji-spark/) **·** [IF](https://android-unlock.techidaily.com/in-2024-how-to-use-google-assistant-on-your-lock-screen-of-huawei-phone-by-drfone-android/) **·** [IFS](https://screen-recording.techidaily.com/updated-ultimate-techniques-for-precise-iptv-screen-imaging/) **·** [IMAGE](https://screen-mirror.techidaily.com/top-10-airplay-apps-in-xiaomi-redmi-note-12-5g-for-streaming-drfone-by-drfone-android/) **·** [INDEX](https://youtube-help.techidaily.com/in-2024-the-full-course-on-becoming-a-yt-creator-expert/) **·** [IS](https://win-amazing.techidaily.com/new-release-gtx-1650-super-driver-updates-compatible-with-windows-11/) **·** [LEN](https://extra-hints.techidaily.com/scalable-and-stylish-type-in-ae-with-top-choices/) **·** [MATCH](https://extra-guidance.techidaily.com/mirthful-missions-delving-into-the-goofy-movie-vhs-for-2024/) **·**[MEDIAN](https://some-techniques.techidaily.com/in-2024-from-novice-to-expert-the-complete-powerdirector-journey/) **·** [RAND](https://instagram-video-recordings.techidaily.com/updated-master-igtv-edits-top-10-tools-ranked/) **·** [ROUND](https://youtube-zero.techidaily.com/ed-2024-approved-the-quick-pathway-to-establishing-a-video-channel-on-your-phone/) **·** [RRI](https://vp-tips.techidaily.com/2024-approved-quick-cash-on-reddit-here-are-13-ways-for-new-users/) **·** [SORT](https://some-techniques.techidaily.com/2024-approved-gopro-versus-polaroid-editing-faces-vs-cameras-that-shoot-them/) **·** [SQRT](https://screen-video-capture.techidaily.com/in-2024-master-guide-ultimate-tips-for-maximizing-mobizens-screen-capture/) **·** [SUBSTITUTE](https://screen-sharing-recording.techidaily.com/updated-maiden-shoot-revelations-and-critique-for-2024/) **·** [SUBTOTAL](https://phone-solutions.techidaily.com/in-2024-prank-your-friends-easy-ways-to-fake-and-share-google-maps-location-on-oppo-a78-5g-drfone-by-drfone-virtual-android/) **·** [SUM](https://instagram-videos.techidaily.com/updated-steps-to-instagram-verification-and-fan-growth-in-under-150-characters/) **·** [SUMIF](https://on-screen-recording.techidaily.com/pinnacle-platforms-transforming-online-interaction/) **·** [TODAY](https://some-guidance.techidaily.com/2024-approved-unlock-spark-ars-full-potential-with-personalized-lut-implementations/) **·** [TRIM](https://graphic-issues.techidaily.com/regaining-access-to-nvidia-writable-displays/) **·** [TRUNC](https://windows11.techidaily.com/balancing-cpu-and-memory-use-after-news-downloads/) **·** [VLOOKUP](https://extra-tips.techidaily.com/integrate-sound-and-sight-web-studio/) **·** [WEEKDAY](https://youtube-tips.techidaily.com/n-2024-virtual-voyage-youtubes-premier-10-vr-video-experience/) **·** [XLOOKUP](https://android-transfer.techidaily.com/in-2024-5-ways-to-transfer-music-from-asus-rog-phone-7-ultimate-to-other-android-devices-easily-drfone-by-drfone-transfer-from-android-transfer-from-android/) **·** [YEAR](https://facebook-record-videos.techidaily.com/updated-in-2024-captivating-content-the-basics-of-removing-background-from-videos/) |  |
| Types                        | [Basic](https://visual-screen-recording.techidaily.com/in-2024-a-step-by-step-recorder-for-discord-enthusiasts/) **·** [Budgeting](https://easy-unlock-android.techidaily.com/in-2024-how-to-reset-a-realme-narzo-60-pro-5g-phone-that-is-locked-by-drfone-android/) **·** [Data Entry](https://vimeo-videos.techidaily.com/in-2024-high-end-downloads-best-10-apps-for-extracting-vimeo-videos/) **·** [Logical](https://extra-skills.techidaily.com/in-2024-spark-engagement-the-ultimate-list-of-video-text-effects/) **·** [Text](https://video-screen-grab.techidaily.com/updated-the-art-of-smooth-video-transitioning-for-2024/) **·** [Time and Date](https://extra-lessons.techidaily.com/kickstart-your-telegram-promotion-journey-tips-for-newbies/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |  |
| Explained                    | [Copying Formulas](https://extra-tips.techidaily.com/in-2024-converting-personal-memories-from-stillness-to-motion/) **·** [Evaluating Formulas](https://youtube-blog.techidaily.com/ed-the-role-of-youtube-images-in-video-promotion-and-discovery-for-2024/) **·** [Finding Functions](https://win11.techidaily.com/renaissance-pc-refresh-with-atlasos/) **·** [Fixing Formula Errors](https://extra-lessons.techidaily.com/step-into-premium-sound-quality-garageband-edition/) **·** [Functions vs Formulas](https://games-able.techidaily.com/is-premium-play-on-demand-worth-it/) **·** [Comparing Lookup Functions](https://tech-revival.techidaily.com/examining-codegpts-capabilities-in-tech-innovation/) **·** [Locking Formulas](https://some-guidance.techidaily.com/in-2024-unveiling-effective-sales-methods/) **·** [Structuring Formulas](https://youtube-docs.techidaily.com/n-2024-automate-playlist-retrieval-from-youtube-directly/) **·** [Translating Formulas](https://extra-tips.techidaily.com/techniques-to-reduce-nausea-while-in-vr/)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |  |

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
