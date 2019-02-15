---
description: Information to use the Target Visual Experience Composer (VEC) Helper browser extension to load websites reliably in iframe.
keywords: vec;visual experience composer; vec;iframe;extension;browser
seo-description: Information to use the Adobe Target Visual Experience Composer (VEC) Helper browser extension to load websites reliably in iframe.
seo-title: Adobe Target Visual Experience Composer (VEC) helper extension
solution: Target
title: Visual Experience Composer helper extension
topic: Standard
---

# Visual Experience Composer helper extension

The [!DNL Adobe Target] [!UICONTROL Visual Experience Composer] (VEC) Helper browser extension for Google Chrome can be used to reliably load websites that might otherwise be problematic.

Reasons why some websites might not open reliably in the VEC include:

* Website has strict security policies.
* Website is in an iframe.
* at.js is not yet implemented on the website.
* Customer's QA and/or stage site is not available to the outside world (the site is internal).

The VEC Helper browser extension for Chrome solves site-loading issues for which customers now rely on the [!DNL Target] [!UICONTROL Enhanced Experience Composer] or third-party extensions, such as Requestly

Benefits of using the VEC Helper extension include:

* All iframe busting headers, such as X-Frame-Options and Content-Security-Policy, are implicitly removed from the website. There is no more need to create complicated Requestly rules to do this.
* If a webpage does not yet contain the [!DNL Target] at.js JavaScript library, you can use the extension to inject the library so you can author experiences for the website. You can then create activities and QA them using preview links.
* Mobile Viewports are supported even without the [!UICONTROL Enhanced Experience Composer] (EEC).
* Customers new to [!DNL Target] can use the extension to experiment with [!DNL Target] even if their IT developers have not yet implemented [!DNL Target] on their websites.
* Partners servicing multiple customers' websites and [!DNL Target] accounts now have one simple mechanism to support VEC loading, instead of managing multiple rules in third-party tools

## Obtain and install the VEC Helper browser extension

1. Navigate to the [Adobe Target VEC Helper browser extension in the Chrome Web Store](https://chrome.google.com/webstore/detail/adobe-target-vec-helper/ggjpideecfnbipkacplkhhaflkdjagak).
1. Click [!UICONTROL Add to Chrome > Add Extension].
1. To use the extension, click the VEC Helper browser extension icon ( ![VEC Helper icon](/help/c-experiences/c-visual-experience-composer/r-troubleshoot-composer/assets/vec-help-extension.png) ) in your Chrome browser's toolbar while in the VEC or QA Mode.

## Notes

* The [!UICONTROL Inject Target libraries] flag in the extension is OFF by default. You can enable this flag if you want to use the VEC on a site that has not yet been implemented for Target.
* If you attempt to load a website that fails to load, a message displays in the VEC suggesting that you install the VEC Helper browser extension.
* If at.js is not yet implemented on the website, a message displays in the VEC suggesting that you install the extension.
* If the extension is enabled and is powering the loading, messages display when the extension injects the at.js library (if necessary) or helps open the website reliably within the VEC.
* To use the extension in [QA Mode](/help/c-activities/c-activity-qa/activity-qa.md), you need to have another Chrome tab authenticated into the [!DNL Adobe Experience Cloud] org.