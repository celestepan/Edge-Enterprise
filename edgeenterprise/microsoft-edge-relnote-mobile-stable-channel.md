---
title: "Microsoft Edge release notes for Mobile Stable Channel"
ms.author: charlielin
author: dan-wesley
manager: alexyuan
ms.date: 06/12/2024
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge release notes for Mobile Stable Channel"
---

# Release notes for Microsoft Edge Mobile Stable Channel

These release notes provide information about new features that are available to work or school accounts, and non-security updates that are included in the Microsoft Edge for Mobile Stable Channel.

To understand Microsoft Edge channels, see the [Overview of the Microsoft Edge channels](./microsoft-edge-channels.md).

All the Stable channel security updates are listed in [Release notes for Microsoft Edge Security Updates](./microsoft-edge-relnotes-security.md).

> [!NOTE]
> For the Stable Channel, updates roll out progressively over one or more days. To learn more, see [Progressive rollouts for Microsoft Edge updates](./microsoft-edge-update-progressive-rollout.md). There might be a delay before the new release is populated to the App Store (iOS) and Google Play (Android).

## Version 125.0.2535.96 (Android and iOS): June 11, 2024

Fixed various bugs and performance issues.

## Version 125.0.2535.87 (Android and iOS): June 5, 2024

Fixed various bugs and performance issues.

## Version 125.0.2535.72 (Android and iOS): May 27, 2024

Fixed various bugs and performance issues.

## Version 125.0.2535.60 (iOS): May 23, 2024

Fixed various bugs and performance issues, provide general updates, add new features and policies.

### General updates

- MS Tunnel Tunnel SDK updated to 1.0.17.
- Upgrade Intune iOS SDK to 19.3.1, with working time support.

### New features

- Shared links feature will appear in overflow menu in work account. 
- PAC policy now supports fail-close.
- Support certificate pinning via Intune, currently only supports limited number of Microsoft domains. Pending on Intune's improvements to support customizable cert-domain pair.
- Support of new iOS 17 relay proxy via policy `com.microsoft.intune.mam.managedbrowser.ProxyRelayUrl`.

### New Policies

- `com.microsoft.intune.mam.managedbrowser.ProfileAutoSwitchToWork` to resolve the conflict between Intune auto identity switch and Edge allow/block URL policies.
- Introduce MDM policy [EdgeCopilotEnabled](/deployedge/microsoft-edge-mobile-policies#edgecopilotenabled), to globally disable Copilot in Edge mobile, including the personal context.

## Version 125.0.2535.51 (Android): May 21, 2024

Fixed various bugs and performance issues, provide a general update, add new features and policies.

### General updates

- Upgrade the Intune Android SDK to 10.3.0, with working time support.

### New features

- Edge Android now supports kerberos/negotiate authentication on Android via an [external SPNEGO authenticator app](https://github.com/google/android-kerberos-authenticator) integrated with Android account management framework.
- Shared links feature will appear in overflow menu in work account.

### New Policies

- Introduce the MDM policy [EdgeCopilotEnabled](/deployedge/microsoft-edge-mobile-policies#edgecopilotenabled), to globally disable Copilot in Edge mobile, including the personal context.


## Version 124.0.2478.105 (iOS): May 17, 2024

Fixed various bugs and performance issues.

## Version 124.0.2478.104 (Android): May 15, 2024

Fixed various bugs and performance issues.

## Version 124.0.2478.89 (iOS): May 8, 2024

Fixed various bugs and performance issues.

## Version 124.0.2478.87 (Android): May 7, 2024

Fixed various bugs and performance issues.

## Version 124.0.2478.71 (iOS): April 30, 2024

Fixed various bugs and performance issues.

## Version 124.0.2478.71 (Android): April 29, 2024

### Policy updates

- MDM policy  [edgenewtabpagelayout](/deployedge/microsoft-edge-mobile-policies#edgenewtabpagelayout) to manage New Tab Page layout settings.
- MDM policy [edgenewtabpagelayoutcustom](/deployedge/microsoft-edge-mobile-policies#edgenewtabpagelayoutcustom) to manage New Tab Page custom setting.
- MDM policy [edgenewtabpagelayoutuserselectable](/deployedge/microsoft-edge-mobile-policies#edgenewtabpagelayoutuserselectable) to manage whether the New Tab Page layout is selectable by users.

Fixed various bugs and performance issues.

## Version 124.0.2478.62 (Android): April 25, 2024

Fixed various bugs and performance issues.

### Bug fixes

- [Android] Fixed a bug where setting Edge as the default browser caused repetition, and the button became unresponsive.
- [Android] Fixed a bug in shared device mode where the sign-in process was getting hung on the loading screen.

## Version 124.0.2478.50 (Android and iOS): April 22, 2024

Made general updates, fixed various bugs and performance issues, added new features and policies.

### General updates

- [iOS] MS Tunnel updated to 1.0.15, added privacy manifest file to comply with Apple App Store requirements.
- [iOS] updated Citrix mVPN iOS SDK to 24.2.1
- [iOS] added 'protApp' parameter to Microsoft Bing Search resource token fetch request, so it is not blocked by the CA "requiring app protection" policy. This token is needed for Copilot in Edge
- [iOS] Intune SDK updated to 19.2.0

### Bug fixes

- [iOS] Fix disableFeatures policy bug for inPrivate mode, handle corner cases where inPrivate not disabled
- [Android] Fixed a bug in Guided switch

### New features

- [Android] Re-enable Kerberos authentication support on Android with an external Negotiate Authenticator app.
- [Android and iOS] Copilot in Edge mobile now properly supports school scenarios.
- [iOS] Shared Device Mode support
- [Android and iOS] In-flight, the "Shared Links" feature can be opened from the Edge overflow menu.

### Policy updates

- [Android and iOS] Introduce MDM policy [EdgeCopilotEnabled](/deployedge/microsoft-edge-mobile-policies#edgecopilotenabled), to globally disable Copilot in Edge mobile, including the personal context.
- [Android and iOS] MDM policy [HideFirstRunExperience](/deployedge/microsoft-edge-mobile-policies#hidefirstrunexperience), to hide first run experience.
- [Android and iOS] MDM policy [DefaultBrowserSettingEnabled](/deployedge/microsoft-edge-mobile-policies#defaultbrowsersettingenabled), to disable default browser settings pop-up.
- [Android] MDM policy [PreventTyposquattingPromptOverride](/deployedge/microsoft-edge-mobile-policies#preventtyposquattingpromptoverride), to prevent bypassing Edge Website Typo Protection prompts for sites.
- [Android] MDM policy [TyposquattingAllowListDomains](/deployedge/microsoft-edge-mobile-policies#typosquattingallowlistdomains), to configure the list of domains for which Edge Website Typo Protection won't trigger warnings.

## Version 123.0.2420.108 (iOS): April 19, 2024

Fixed various bugs and performance issues.

### Bug fixes

- Fixed a bug that pkpass files in binary data mime type were not handled correctly.

## Version 123.0.2420.102 (iOS): April 16, 2024

Fixed various bugs and performance issues.

## Version 123.0.2420.102 (Android): April 16, 2024

Fixed various bugs and performance issues.

## Version 123.0.2420.90 (iOS): April 11, 2024

Fixed various bugs and performance issues.

## Version 123.0.2420.90 (Android): April 10, 2024

Fixed various bugs and performance issues.

## Version 123.0.2420.74 (Android and iOS): April 2, 2024

Fixed various bugs and performance issues.

### General updates

- [iOS] Update Citrix mVPN SDK to version 24.2.1

### New features

- Start a flight to show Shared links entry point on the overflow menu

## Version 123.0.2420.61 (Android): March 25, 2024

Fixed various bugs and performance issues. This release includes general updates, and new policies.

### General updates

- [Android] Remove "https" scheme check for managed bookmarks to support URLs such as `edge://…`.

### Bug fixes

- [Android] Fix a bug that NLTM SSO policy doesn't work in some conditions.
- [Android] Fix issues for brand logo policy.

### Policy updates

- Introduce a policy to control the behavior of opening Intune unmanaged URL in work profile. Current behavior is "stay" and open the unmanaged URL in work profile. This policy allows admin to change behavior to switch to personal context and open the unmanaged URL.

  `com.microsoft.intune.mam.managedbrowser.ProfileAutoSwitch`
  - 0 (Default) - The URLs are opened in normal tabs with work profile
  - 1 - Edge respects Intune's protection policy, the behavior is based on the configuration of Receive data from other apps in Intune protection policy.
    - All apps - fall back to behavior for policy value 0
    - None or Policy managed apps
      - If personal profile is signed-in, the URLs are opened in normal tabs with personal profile
      - If personal profile isn't signed-in, the URLs are opened in InPrivate
      - If InPrivate is disabled, the URLs won't be opened
  - 2 (Android only) - Microsoft Edge checks **URLAllowlist** or **URLBlocklist**. Microsoft Edge opens allowed URLs in normal tabs with work profile. As for URLs in blocklist, they might or might not be opened in InPrivate or normal tabs with personal profile, it depends on how **openInPrivateIfBlocked** is configured.

## Version 123.0.2420.56 (iOS): March 25, 2024

Fixed various bugs and performance issues. This release includes general updates, new features, and new policies.

### General updates

- [iOS] Update MS Tunnel MAM SDK to 1.0.12
- [iOS] Update MS Intune MAM SDK to 19.1.0
- [iOS] "Save to OneDrive" option in Edge now has upload progress indicator.

### Bug fixes

- [iOS] URL Block policy also shows "Site blocked" alert for http POST requests.
- [iOS] Fix issues for new File upload block policy and idle timer policy.

### New features

- [iOS] Shared device mode public preview

### Policy updates

- [iOS] Introduces MAM policy to control the behavior the "Site Blocked" popup. This policy would let admins choose preferences between InPrivate and MSA if options are available.
`com.microsoft.intune.mam.managedbrowser.AutoTransitionModeOnBlock`
  - 0 (Default) - Always show choose popup windows
  - 1 - Only MSA account login, auto transition to MSA
  - 2 - When the MSA account login and InPrivate are enabled at the same time, auto transition to MSA
  - 3 - When the MSA account login and InPrivate are enabled at the same time, auto transition to InPrivate.

- [iOS] Introduce a policy to control the behavior of opening Intune unmanaged URL in work profile. Current behavior is "stay" and open the unmanaged URL in work profile. This policy allows admin to change behavior to switch to personal context and open the unmanaged URL.

  `com.microsoft.intune.mam.managedbrowser.ProfileAutoSwitch`
  - 0 (Default) - The URLs are opened in normal tabs with work profile
  - 1 - Edge respects Intune's protection policy, the behavior is based on the configuration of Receive data from other apps in Intune protection policy.
    - All apps - fall back to behavior for policy value 0
    - None or Policy managed apps
      - If personal profile is signed-in, the URLs are opened in normal tabs with personal profile
      - If personal profile isn't signed-in, the URLs are opened in InPrivate
      - If InPrivate is disabled, the URLs won't be opened

<!-- Version 122.0.2365.99 (Android and iOS): March 18, to 2024 Version 121.0.2277.84 (Android): January 29, 2024 -->
<!-- Version 120.0.2210.150: January 21, 2024 to Version 120.0.2210.59: December 12, 2023 -->
<!-- Version 119.0.2151.107: December 6, 2023 to Version 119.0.2151.46: November 7, 2023  -->
<!-- Version 118.0.2088.81: November 1, 2023 to Version 117.0.2045.53: October 6, 2023  -->
<!-- Version 117.0.2045.33: September 15, 2023 to Version 116.0.1938.64: August 30, 2023  -->
<!-- Version 116.0.1938.56: August 21, 2023, to Version 115.0.1901.183: July 22, 2023 -->
<!-- Version 114.0.1823.37: June 2, 2023 to Version 113.0.1774.50: May 18, 2023 -->
<!-- Version 113.1774.36: May 8, 2023 to Version 112.0.1722.36: April 7, 2023 -->
<!-- Version 111.0.1661.43: March 18, 2023 to Version 109.0.1518.70: January 26, 2023 -->
<!-- Version Version 109.0.1518.58: January 18, 2023 to Version 108.0.1462.45: December 8, 2022  -->
<!-- Version 108.0.1462.43: December 7, 2022 to Version 106.0.1370.47: October 17, 2022 -->
<!-- Version 105.0.1343.38: September 13, 2022 to Version 101.0.1210.32: April 29, 2022 -->

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
