+++
title = "Privacy Policy"
description = "What data the Google Calendar connection uses, where it is stored and how to revoke access."
template = "page.html"
+++
Last updated: November 14, 2026.

This policy applies to the **Obsidian Calendar Test** OAuth application and the Google Calendar Tasks Sync 1.7.0 configuration for desktop Obsidian described on the [home page](@/_index.md). Contact the OAuth application owner at [calendar-plugin-obsidian-beta@googlegroups.com](mailto:calendar-plugin-obsidian-beta@googlegroups.com).

## Access to Google data

After you grant permission, the plugin accesses your calendar list and Google Calendar events. This includes calendar and event identifiers, titles, dates, times, time zones, locations, descriptions and recurrence details. Google API responses may include additional event fields, such as organizer and attendee information. The plugin uses this data to display calendars and synchronize events on your device.

This registration is intended for Calendar-only use. Keep task mirroring disabled and do not grant Google Tasks access. The stock plugin nevertheless includes Tasks in its authorization request, even when task mirroring is disabled. That request is broader than this configuration needs.

The current Calendar permission permits viewing, editing, sharing and permanently deleting calendars you can access, within your Google account's rights. The reviewed calendar integration uses calendar-list and event operations; it does not use this permission to delete calendars or change sharing. Selecting calendars inside the plugin controls synchronization but does not narrow the Google permission itself. Read the full permission description on Google's consent screen before approving access.

## How data is used

Calendar data is used to view, create, edit, delete and synchronize events in response to your actions and the plugin's refresh schedule. The OAuth application owner does not receive this data through a server of their own and does not use it for advertising, sale of data or model training.

Obsidian Calendar Test will handle and transfer information obtained through Google APIs in accordance with the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including Limited Use. These data uses are limited to the calendar functions described here.

## Transfer and local storage

The plugin on your device exchanges data with Google for authorization and Calendar API operations. This setup has no separate server operated by the OAuth application owner that receives calendar contents. The GitHub Pages website does not receive calendar data or tokens either.

The event cache is stored in Obsidian's local storage on your device. The plugin does not encrypt this cache. Local protection depends on your device, operating system, account permissions and storage security.

Plugin settings contain desktop OAuth client parameters, calendar identifiers and names, and an account identifier that may be your Google email address. New logins store the refresh token in encrypted form using the sync passphrase. The passphrase is stored through Obsidian's keychain facilities; its actual protection depends on your operating system and its settings. Older imported settings can contain a legacy unencrypted token until a passphrase is applied.

If you separately enable synchronization of Obsidian vault files, their transfer is governed by the settings of your chosen service. This policy does not cover the independent services provided by Obsidian or Google, or other plugins you install.

## Retention, revoking access and deleting local data

The plugin has no automatic expiry period for cached events. Entries remain until removed by synchronization, a cache-clearing action or removal of the relevant local storage. Plugin settings and the saved sync passphrase also remain until removed. Copies in backups or separately synchronized files follow the retention settings of those services.

You can revoke permissions in your [Google account connections](https://myaccount.google.com/connections). Revocation prevents further authorized API access; it does not by itself erase local caches, settings or backups.

The plugin's **Log out** command attempts to revoke the device's refresh token, removes the stored token and clears event caches for calendars still listed in the plugin settings. If there is no network connection or an error occurs, check that access has been revoked in your Google account settings. **Clear cache** also clears event caches for calendars currently listed in the settings. While the connection remains active, the next synchronization may create them again.

Cached data for a calendar removed from the plugin's list earlier can remain in local storage. **Log out** also leaves the sync passphrase in Obsidian's keychain. Complete local removal therefore requires removing remaining plugin settings, old cache entries and the saved passphrase on each device, as well as any backups or synchronized copies you control. Contact support if you need instructions for your operating system.

Clearing the cache or logging out of the plugin does not delete the events in Google Calendar. You can delete those separately in the calendar.

## Visiting this website

This website consists of static HTML pages and local CSS. It has no JavaScript, data collection forms, analytics, advertising pixels, external fonts or embedded third-party content. The website code does not set cookies or use browser storage.

GitHub Pages processes requests to serve these pages. GitHub states that it logs and stores visitors' IP addresses for security purposes. See [GitHub Pages data collection](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages#data-collection) and the [GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

External links lead to separate services when you choose to follow them. The website code does not load their contents when you open a page.

## Support requests

When you email support, Google Groups processes your sender address, your name if provided, the message and any attachments. Messages are accessible to members of the private support group. This information is used to respond to your request.

This project currently has no automatic deletion schedule for support correspondence. Messages remain in the private group until manually removed. To request deletion of messages held by the support group, write to the support address. Deleting a group message does not necessarily remove copies already delivered by email or copies retained by the service provider under its own policies.

Do not send passwords, tokens, your sync passphrase, the complete plugin settings file or calendar contents. A description of your actions and an error message with personal information removed is usually enough to investigate a problem.

## Policy changes

This page and its revision date will be updated if the described data processing changes. Before Google data is used for a new purpose or a new data type is accessed, users will be informed and asked for consent. If the requested access is unclear, contact support before authorizing the connection.
