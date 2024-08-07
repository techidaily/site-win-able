---
title: "Solve Your Kodi Network Problem: A Guide to Fixing Directory Information Failures"
date: 2024-08-04 17:42:31
updated: 2024-08-07 10:28:37
tags:
  - win11
  - win10
  - win7
categories:
  - ProgramIssues
description: "This Article Describes Solve Your Kodi Network Problem: A Guide to Fixing Directory Information Failures"
excerpt: "This Article Describes Solve Your Kodi Network Problem: A Guide to Fixing Directory Information Failures"
thumbnail: https://thmb.techidaily.com/a88de5655376206e2ee17661cb9dd03b46b68bf81e7fb9a2b0bcd4cf8d7ba0d8.jpg
---

## Solve ‘Configuration Server Connection Failure’ Effortlessly Today

Many Forza Horizon 4 players are reporting that they get the error message ‘**Unable to connect to the live configuration servers** ‘ on both Xbox and PC. If you’re also experiencing the same issue, you can try the following fixes.

![](https://images.drivereasy.com/wp-content/uploads/2021/05/network-error-1200x722.jpg)

 Before you try the following solutions, make sure you have an internet connection. If you’re experiencing internet issues, you can refer to[how to fix slow internet on a Windows PC](https://tools.techidaily.com/drivereasy/download/) .

## Try these fixes

* [1. Sign in again](https://tools.techidaily.com/drivereasy/download/)
* [2. Check the status of Teredo (Windows 10)](https://www.drivereasy.com/knowledge/unable-to-connect-to-the-live-configuration-servers-error/#h-2-check-the-status-of-teredo-windows-10)
* [3. Reinstall the Teredo Adapter](https://tools.techidaily.com/drivereasy/download/)
* [4. Turn on Windows Firewall](https://tools.techidaily.com/drivereasy/download/)
* [5. Enable Xbox Live Networking Service & Xbox Live Auth Manager](https://tools.techidaily.com/drivereasy/download/)

## 1\. Sign in again

 This error might be temporary and the fix can be as easy as signing in again. Just sign out of your current account on the main menu, and sign in again. This should fix the ‘Unable to connect to the live configuration servers’.

 If you’re on Steam, the**“Sign out”** option should appear when you start the game.

![sign out steam](https://images.drivereasy.com/wp-content/uploads/2021/05/sign-out.jpg)

 But if this method doesn’t do the trick, you can try the next fix below.

## 2\. Check the status of Teredo (Windows 10)

 If you’re getting the ‘Unable to connect to the live configuration servers’ error, it may be caused by a Teredo issue. Here’s how:

 1) Click the Start menu (the Windows logo key) in the lower-left corner of the main screen.

 2) Select**Settings** \>**Gaming** , and then select**Xbox Networking** .

![](https://images.drivereasy.com/wp-content/uploads/2021/05/Xbox.jpg)

 3) Select**Fix it** . Windows will try to detect and fix known issues with Teredo.

![](https://images.drivereasy.com/wp-content/uploads/2021/05/fix-it.jpg)

 4) Once complete, you will need to click the**Check again** button. If there’s no issue detected, you can launch your game to check if the ‘Unable to connect to the live configuration servers’ issue disappears.

## 3\. Reinstall the Teredo Adapter

 It’s possible that the method above doesn’t fix the Teredo-related issue, and you can try reinstalling the Teredo Adapter using Command Prompt. Here’s how:

 1) In the Search bar, type**cmd** and select**Run as administrator** .

![command prompt admin](https://images.drivereasy.com/wp-content/uploads/2021/05/run-as-admin-cmd.jpg)

 2) Type **the following command** and press **Enter** .

netsh interface Teredo set state disable

![](https://images.drivereasy.com/wp-content/uploads/2021/05/disable-Teredo.jpg)

 3) On your keyboard, press the**Windows + R** key at the same time, and type**devmgmt.msc** . Then press**Ente** r.

![uninstall graphics driver](https://images.drivereasy.com/wp-content/uploads/2021/03/device-manager.jpg)

 4) Click **View** \> **Show hidden devices** .

![](https://images.drivereasy.com/wp-content/uploads/2021/05/show-hidden-devices.jpg)

 5) Double-click on **Network adapters** .

 6) Right-click any Teredo adapter and select **Uninstall** .

 7) Go back to the**Command Prompt** (Admin) window, and enter the following command.

netsh interface Teredo set state type=default

 8) Now launch your game and check if the error message ‘Unable to connect to the live configuration servers’ is gone for now.

## 4\. Turn on Windows Firewall

 You may have turned Windows Firewall to prevent some games from crashing, but this game requires that Windows Firewall is turned on because it will need the Teredo IPsec connection.

 1) In the Search bar, type**cmd** and select**Run as administrator** .

![command prompt admin](https://images.drivereasy.com/wp-content/uploads/2021/05/run-as-admin-cmd.jpg)

 2) Type **the following command** and press **Enter** .

netsh advfirewall set allprofiles state on

3) Close the Command Prompt.

 Launch your game again to test the issue, and if this method doesn’t do the trick, check the one below.

## 5\. Enable Xbox Live Networking Service & Xbox Live Auth Manager

 To make sure your game runs properly, you’d better check the Xbox Live Networking and Xbox Love Auth Manager services are both running properly. Here’s how:

 1) On your keyboard, press the Windows key + R key at the same time, and enter**services.msc** .

![](https://images.drivereasy.com/wp-content/uploads/2020/01/services-run-box.jpg)

 2) Scroll down the bottom, and make sure**Xbox Live Auth Manager** and**Xbox Live Networking Service** are running. If not, right-click the service and click**Start** .

![](https://images.drivereasy.com/wp-content/uploads/2021/05/services-on.jpg)

3) Close the window and launch your game.

---

 Did the fixes above help you out? If the ‘Unable to connect to the live configuration servers’ error persists, you may need to hard reset your router or Xbox One, and uninstall and reinstall the game.

* [Application Errors](https://tools.techidaily.com/drivereasy/download/)
* [games](https://tools.techidaily.com/drivereasy/download/)
* [Xbox](https://tools.techidaily.com/drivereasy/download/)

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
