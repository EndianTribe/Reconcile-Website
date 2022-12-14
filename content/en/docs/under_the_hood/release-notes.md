---
title: "Release Notes"
description: "Release Notes"
lead: ""
date: 2020-10-06T08:48:57+00:00
lastmod: 2020-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "under_the_hood"
weight: 300
toc: true
---

## Build 1020221207

* Added icons to each screen.
* Upgraded all dependencies and removed beta and alpha dependency channels.

## Build 1020221124

* Reverted back to "intest" version to ensure functionality.

## Build 1020221123

* The app now has an icon.
* [Fixed an issue with the ledger not updating after a large entry is made.](https://github.com/EndianTribe/Reconcile-Issues-Tracker-Public/issues/10)
* [Fixed a few issues with the share function.](https://github.com/EndianTribe/Reconcile-Issues-Tracker-Public/issues/14)
* Updated the search interface to be more user-friendly.

## Build 1020221122

* Database wiped to accommodate schema change (value is now stored as Int as opposed to BigDecimal).
* [Limited each individual journal entry value to 9,999,999.99. If you have more than that, please consider donating to yours truly.](https://github.com/EndianTribe/Reconcile-Issues-Tracker-Public/issues/9)
* [Value textfield now correctly formats to at most 2 decimal points (in addition to thousands comma separators).](https://github.com/EndianTribe/Reconcile-Issues-Tracker-Public/issues/8)
* Improved search box range slider value display.
* [Reimplemented debit and credit buttons.](https://github.com/EndianTribe/Reconcile-Issues-Tracker-Public/issues/11)

## Build 1020221119

* Fixed an issue with text alignment on ledger screen.

## Build 1020221118

* Fixed an issue with stats displaying incorrect color over 1k value.
* Fixedd an issue where add journal entry box is disabled after successful addition.
* Added snackbar message to successful journal entry completion.

## Build 1020221117

* Users can now long press on an expense item for additional actions (reverse, duplicate, and share).
* Users can now short press on an expense item for additional information (including notes), which implements [this feature request](https://github.com/EndianTribe/Reconcile-Issues-Tracker-Public/issues/5).

## Build 1020221116

* [Search button on top bar now becomes filled when a filter is active.](https://github.com/EndianTribe/Reconcile-Issues-Tracker-Public/issues/6)

## Build 1020221104

* Revamped the search process as well as search functionality.
* Enforced until dark mode color scheme is fixed.
* Disabled auto rotation.
* Changed populate dummy entry functionality to be closer to real use cases.

## Build 1020221103

* Added reauthentication process immediately prior to account deletion to avoid [FirebaseAuthInvalidCredentialsException](https://firebase.google.com/docs/reference/android/com/google/firebase/auth/FirebaseAuthInvalidCredentialsException).
* Fixed [an issue searching across multiple types](https://github.com/EndianTribe/Reconcile-Issues-Tracker-Public/issues/3).
* Added search UI for value. Functionality not yet implemented.
* Added UUID, Build, and Type on account page for easy debugging.

## Build 20221102

* Reverted back to no app obfuscation (which causes NPE, which will be investigated later).
* Added search functionality for categories.
* Fixed [an issue logging in with Google](https://github.com/EndianTribe/Reconcile-Issues-Tracker-Public/issues/1).

## Build 20221030

* Dramatically shrank app download size.
* Implemented search functionality for counterparties.

## Build 20220929

* Initial internal test release to Google Play Store.
