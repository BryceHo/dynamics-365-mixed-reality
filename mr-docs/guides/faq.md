---
author: BryceHo
description: FAQ about Dynamics 365 Guides (Preview)
ms.author: makamat
ms.date: 08/27/2019
ms.service: crm-online
ms.topic: article
title: FAQ about Dynamics 365 Guides (Preview)
ms.reviewer: v-brycho
---

# Frequently Asked Questions about Microsoft Dynamics 365 Guides (Preview)

[!INCLUDE [cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]
 
## How do I contact Support if I don't find an answer in this FAQ?

If you're not able to use [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides-preview](../includes/pn-dyn-365-guides-preview.md)], or if you have an issue that isn't answered in this FAQ or in the documentation, please contact Customer Support by using the following steps:

1. Go to [https://dynamics.microsoft.com/en-us/support/](https://dynamics.microsoft.com/en-us/support/).

2. Under **Customer Engagement help + support**, select **GET SUPPORT**.

3. Find a phone number or submit a support request through the Admin Center. 

## Why do I have to download two apps?

[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] includes two applications:

- PC authoring application

- [!include[pn-hololens](../includes/pn-hololens.md)] application, which includes modes for authoring and operating

If you plan to author guides, you’ll need to use both apps. If not, you’ll only need the [!include[pn-hololens](../includes/pn-hololens.md)] app.

## What languages is Dynamics 365 Guides available in?

As of the August 27 update, Dynamics 365 Guides is available in the following languages for both the PC app and the HoloLens app:

- English (US, UK)

- Chinese (People's Republic of China, Taiwan, Hong Kong SAR)

- German 

- Dutch (Netherlands)

- French (France, Canada)

- Italian

- Japanese

- Korean

- Spanish (Spain)

## Is there an out-of-the-box integration with Dynamics 365 for Field Service?

Yes, the preview version of [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)] integration was added in version 104.1907.19001.

## I get an error message when I try to sign in to the PC app or [!include[pn-hololens](../includes/pn-hololens.md)] app

The [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution package (which includes the built-in library of 3D content) needs to be installed on your [!include[pn-dyn-365](../includes/pn-dyn-365.md)] account. Every user must also have a license to use the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] product. If your organization is already subscribed to [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)], you or your admin can easily provide access to the apps. For more information, [see the Setup topic](setup.md).

## Where is the data stored and who has access to it?

The data is stored in Common Data Service in the tenant that you have admin privileges to. Please sign in to [!include[pn-dyn-365](../includes/pn-dyn-365.md)] using the credentials created during the sign-up process. For more information, [see the Setup topic](setup.md). 

## What file formats are supported?

The following table lists the formats supported for 3D content, images, and videos.

|Media|Supported formats|Best practice|
|----------|----------------------|-------------------------------------------------------------------------|
|3D content|glTF, GLB, and FBX|Make sure to optimize your 3D models as much as possible to maintain optimal performance on [!include[pn-hololens](../includes/pn-hololens.md)].|
|Images|PNG, JPG, JPEG, GIF, TIFF||
|Videos|MP4, MOV, WMV|Make sure to keep your videos less than 2 minutes long, and focused on one step at a time.|

## Will I lose any data if I close an app inadvertently?

Both apps automatically save your edits as you author a guide. We recommend pausing for a couple seconds after you’re done before closing the app to make sure the app has time to sync with the server.

Note that in the [!include[pn-hololens](../includes/pn-hololens.md)] application, if you use the bloom gesture to open the **Start** menu, the app goes on standby (doesn’t close). When you select the app tile, you’ll return to where you were before and no changes will be lost.

## What if the app crashes while authoring. Do I lose data?
Both apps automatically save your edits as you author a guide. Any loss of data due to a crash should be minimal.

## What keyboard shortcuts are available in the PC authoring app?

For a list of keyboard shortcuts, see the [Authoring Guide](pc-authoring.md).

## How can I improve visual clarity of holograms in the [!include[pn-hololens](../includes/pn-hololens.md)] app?

If holograms aren’t visually clear, [!include[pn-hololens](../includes/pn-hololens.md)] might not be properly calibrated for you. Calibration is crucial because [!include[pn-hololens](../includes/pn-hololens.md)] renders holograms based on the distance between your eye pupils (interpupillary distance or “IPD”). If [!include[pn-hololens](../includes/pn-hololens.md)] isn’t calibrated correctly, your eyes struggle to see the holograms in relation to the real world. 

To calibrate [!include[pn-hololens](../includes/pn-hololens.md)]:

1.	Use the bloom gesture to open the **Start** menu.

2.	Use the bloom gesture again to see all the installed apps. 

3.	Select the Calibration app, and then follow the instructions in the app. 

4.	After calibrating, select the [!include[pn-hololens](../includes/pn-hololens.md)] app again.

If the holograms are visually clear but too bright or too dim, use the buttons on the left side of the [!include[pn-hololens](../includes/pn-hololens.md)] headset to increase or decrease brightness.

## What should I do if the holographic instructions aren’t aligned to my work area?

Incorrect alignment of holograms can happen for two main reasons:

- Your IPD has not been set correctly on the [!include[pn-hololens](../includes/pn-hololens.md)]. Refer to the instructions on setting the IPD above to correct this.

- The guide needs to be realigned:

- If the guide is aligned using a **digital anchor**, the digital representation (3D representation laid over its corresponding physical area) is not aligned correctly. To realign the guide, select the **Anchor** button and then realign the digital representation to perfectly overlay the physical area. 

- If the guide is aligned using a **printed anchor**, the marker for the guide might not have been printed properly. Try realigning the guide by selecting the **Anchor** button. Alternatively, you can reprint the marker. Make sure that the printed marker lies flat in the work area before you realign.

For more information on anchoring methods, see the [Authoring Guide](pc-authoring.md).

## What does the Save button with the refresh icon mean? How does Save work?

The Autosave functionality enables authors to synchronize their changes across the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps when editing a guide at the same time in both apps. Edits are automatically saved and synced to the server every few seconds. The apps will also refresh automatically when they detect any changes made to the guide from another device. You can also select the **Save** button at any time if you want to be sure your edits are saved.

## I see this message: “Guide out of sync… refreshing” with a loading spinner. What’s going on?

This message is displayed when you or another user are editing the same guide on separate devices. The guide is automatically saved on the other device first, then updated on the server. When the current device learns of the update, it reloads the latest version of the guide from the server.

## I see this message: “Save failed”. What does this mean?

The PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps save your changes to the server 2 seconds after each change is made. If any of these save attempts fail, you will see this notification.

This might occur if you have a poor internet connection or if the server is down. The notification should go away automatically once the server connection is restored. However, if this message doesn’t go away, we suggest that you not make more edits during that session since the edits may be lost. Check the internet connection on your device or speak with your administrator to see if there are any connectivity issues.

## Can I add more than eight 3D models to a step?

There are only eight **3D parts** boxes in the bin, which limits the variety of 3D models you can add to a single step. When placing holograms on the [!include[pn-hololens](../includes/pn-hololens.md)], you can, however, place an unlimited number from the bin. For example, you can add up to eight different 3D models (arrows, boxes, nuts, drills, and so on) to the bin, but you can place as many arrows, boxes, nuts, and drills from each **3D Parts** box that you want when in [!include[pn-hololens](../includes/pn-hololens.md)]. To do this, either tap the asset bins to spawn 3D models or go to a 3D model’s **Edit** menu and select **Duplicate**.

## I see a triangle-shaped hazard sign when I load a step. What does that mean?

The hazard sign is a placeholder for 3D models, videos, or images that can’t be successfully loaded in the [!include[pn-hololens](../includes/pn-hololens.md)] app. Possible reasons for this:

- This might occur due to intermittent connectivity issues or because the file might be too large. If you see this, please relaunch the [!include[pn-hololens](../includes/pn-hololens.md)] app. If this doesn’t fix the problem, launch the PC app, find the file in question, and open it in preview mode. If preview loads, reinstall the [!include[pn-hololens](../includes/pn-hololens.md)] app and try launching the guide again. 

- If you can’t find the file in the PC app library, the reference (entity) to the 3D model/video/image is broken. Please upload the file again and re-author the guide.

- If the file exists in the library but the preview doesn’t load, there’s a problem with the file information in [!include[pn-dyn-365](../includes/pn-dyn-365.md)]. Please upload the file again, and then edit the guide to refer to this new asset wherever applicable.

### See also

[Known Issues in Dynamics 365 Guides in preview](known-issues.md)
