---
layout: default
title: Privacy Policy
description: Tallyist for Android does not collect your data. Nothing you log reaches the developer.
permalink: /privacy/
---

# Tallyist Privacy Policy

**For Tallyist on Android. Last updated: September 11, 2026**

Tallyist does not collect your data. Nothing you log reaches the developer.

This page stays in English even where the app's interface is translated, so that
what it claims can be checked against the app's manifest and its Google Play
Data safety declaration.

## What Tallyist stores

- The drinks you log. One row for each drink: when it was, the beverage type if
  you picked one, the size, the strength, and two housekeeping timestamps.
- The days you record as alcohol-free. One row for each: the date, and the same
  two timestamps.
- Your settings. Five values: the region whose standard-drink definition your
  totals use, the light or dark appearance choice, two display switches, and
  whether the introduction has been seen.

All of it is stored on your device, in the app's own private storage. No account
is required. Tallyist asks for no sign-in, and has no permission to use the
internet.

There is no name in any of it, no email address, no device identifier and no
advertising identifier. The app never reads the advertising ID or any hardware
identifier. Each drink carries a random identifier generated on your device,
which identifies the row and nothing else.

The app has no text fields of its own. Drinks are logged by tapping and by
dragging a slider, and times and dates are set on a clock face and a calendar.
The one keyboard Tallyist can show belongs to Android's standard date picker,
whose dialog offers to take a date as digits instead of taps. That accepts digits
only, and what gets saved is the resulting date, never the characters typed. No
string you type is written to the database, to your settings, or to a backup.

## Where your data can go

Three paths, and they are the only three.

**Android's own backup.** The app keeps a second copy of your log as a file in
its own storage, `files/backup/log.json`, so that your record survives a move to
a new phone. That file is written deliberately into the one directory Android's
backup system is allowed to take. If backup is turned on for your device, Android
copies the file into your Google account's backup, and Android's device-to-device
transfer carries it to a replacement phone during setup.

The file holds every drink row and every recorded alcohol-free day, including
rows behind entries you have deleted. Your settings are not in it, and neither is
the database itself, so a restored phone comes back with the whole log and with
every setting at its default, including the introduction.

Android performs this copy. Tallyist holds no permission to use the internet, so
it does not and cannot contact Google, and the developer never receives the file
and has no way to ask for it. On current versions of Android the backup is
encrypted with a key derived from your device screen lock, which Google does not
hold. Whether it happens at all is a system setting, under Google, then Backup.
Tallyist cannot read that setting and cannot change it.

**Share images.** A month, a year, or a year in review can be rendered as a
picture. A month card carries four figures and a day-by-day grid of that month,
each day shaded by how much was logged. A year card carries twelve such grids, so
it is a day-by-day picture of a year. Each image is made on your device, only when
you ask for one, and goes only where you send it through the system share sheet.
Once an image is in another app, it belongs to that app.

The app writes one image into its cache, replaces it with the next card, and
empties the folder at every launch. The image carries no identifier and no
embedded metadata, and the app does not record whether or where anything was
shared.

**The home screen widget.** If you place the widget, today's count is drawn by
your launcher, which is a different app on your own device. It shows one number
and a caption. No dates, no history, no totals, no per-drink detail. There is no
widget unless you place one. It is excluded from the lock screen.

## What the rest of your phone can see

These are not things Tallyist does. They are things Android does with any app,
and this section is here because a policy that left them out would be describing
a device that does not exist.

- **The app switcher.** Android photographs the last screen of every app when it
  goes to the background, and shows it in recents. For Tallyist that is usually
  today's count or the calendar. Tallyist does not suppress this.
- **On-screen text.** Android can route the text on screen to a system service,
  for features like assistant, autofill, translation and screen search. On many
  phones that service is made by the phone's manufacturer or by Google. Tallyist
  takes no step to opt out of it.
- **The app's own presence.** The name and the icon say what the app is for. They
  are visible on the home screen, in the app drawer, in recents, in Android's
  Settings under Apps, and to anyone who picks up an unlocked phone.
- **USB backup on older Android.** On Android 8 through 11, a computer connected
  by USB can extract the backup file described above after a confirmation on the
  phone. Android 12 closed this.

## What Tallyist does not do

- No analytics, and no crash-reporting SDKs.
- No advertising, and no tracking of any kind.
- No selling, sharing, or transfer of your data to anyone, because the developer
  never has it in the first place.
- No servers. There is no service the developer runs for this app to talk to, and
  no code in the app that could talk to one.
- No network requests at all. The app does not hold `android.permission.INTERNET`,
  which means Android refuses it a network connection at the operating system
  level. This is not a promise about what the app does with a connection. It
  cannot open one.
- No runtime permissions. Not location, camera, contacts, storage, microphone,
  sensors, calendar, or notifications. The app asks you for nothing. Its manifest
  declares one permission, which the build adds so the app can register a
  receiver with itself. It is signature-level and scoped to this app, and it
  grants access to nothing.
- No health integration. Nothing is read from or written to Health Connect or any
  other health app.
- No notifications, and no background scheduling.
- No purchases. This version is free and contains no billing code.
- No AI, and nothing sent anywhere to be processed.
- No data from anyone else. The comparison figures on Trends and on the year view
  are published population statistics that ship inside the app. They are not data
  from other Tallyist users, and the comparison is worked out on your device.

The only third-party library Tallyist asks for is Vico, which draws the charts on
your screen. The rest is Android's own libraries and the Kotlin language runtime,
together with three small utility libraries that arrive alongside them and that
the release build strips back out. No Google Play Services, no Firebase, and no
networking library is in the build. The app also removes one Android component
that would otherwise ask Google Play Services for an emoji font, because that
request is one the app never asked to make.

The developer collects nothing, receives nothing, and holds no copy of anything
you log. The one path by which any of it leaves your device is Android's own
backup, described above, and that goes to your Google account rather than to the
developer.

## Deleting your data

Three steps, and only the first is inside the app.

1. **In the app.** Any drink can be deleted, one at a time, from Today, from
   History, or from a day in the calendar. A recorded alcohol-free day can be
   cleared the same way. A deletion of this kind hides the entry everywhere in the
   app, but the row stays in storage with the time of the deletion, so that a
   restored backup does not bring the drink back. Its details stay in that row,
   and in the backup file, until step 2. There is no single control in this
   version that erases everything at once.
2. **On the device.** Uninstalling removes all of it: the database, your
   settings, the backup file, and any unreadable backup the app has set aside.
   The same result without uninstalling is in Android's Settings app, under Apps,
   then Tallyist, then Storage and cache, then Clear storage.
3. **In your Google account.** A backup Android has already taken outlives both
   of the above. Clearing the app's storage does not clear it, and an emptied app
   will not overwrite it, because Tallyist does not write an empty log over an
   existing backup. That copy is removed in Android's Settings under Google, then
   Backup, or in the Google One app under Storage, then Backups, by deleting that
   device's backup or by turning backup off.

Because the developer holds no copy of anything, there is nobody to send a
deletion request to. Deletion is in your hands and the platform's.

One retention detail worth stating. If the app ever finds a backup file it cannot
read, it moves that file aside rather than overwriting it, so that a damaged
record is never silently destroyed. Files set aside this way are not deleted by
the app. Step 2 removes them.

## Changes to this policy

This policy describes the app as it ships today. If a future version ever
collects data, for example if a server component or an optional cloud backup is
added, this policy and the Google Play Data safety declaration will change before
that version ships. This page is published in a public repository at
<https://github.com/semmes/TallyistAndroid>, and every change to it, with its date, is
visible in that repository's history.

## Contact

Questions about this policy can be raised as an issue on the app's public issue
tracker: <https://github.com/semmes/TallyistAndroid/issues>.
