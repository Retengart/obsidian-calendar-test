+++
title = "Google Calendar in Obsidian"
template = "index.html"
+++
Obsidian Calendar Test connects Google Calendar to desktop Obsidian through the third-party Google Calendar Tasks Sync plugin. You sign in to your own Google account and choose whether to grant calendar access.

## What you can do

View, create, edit and delete events in selected calendars from Obsidian. Changes are exchanged through Google Calendar. After synchronization, they are also available on a phone using the same account and calendar.

Use **Sync now** to refresh the calendar in Obsidian. It retrieves changes that have already reached Google. Uploading changes from your phone depends on the Google Calendar settings on that phone.

## How access works

The connection is set up in the plugin on your device. Google issues separate access tokens for each user. This website does not sign you in to Google or receive your calendar contents.

This setup uses [Google Calendar Tasks Sync 1.7.0](https://github.com/PubCyBerry/obsidian-google-cal-sync/tree/1.7.0). It is intended for **Calendar only**: keep task mirroring disabled and do not grant Tasks access. The stock plugin still requests Calendar and Google Tasks permissions, so its authorization request is broader than this setup needs. The Calendar permission is also broad; read Google's description before approving it. Selecting calendars inside the plugin does not limit that permission.

## Before you connect

Read the [Privacy Policy](@/privacy.md) and [Terms of Use](@/terms.md) for details about data access, local storage and revoking permissions.

This is an independently configured connection using a third-party plugin. It is not an official Google or Obsidian product. This website does not imply that Google has verified the application.
