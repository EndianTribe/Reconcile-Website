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
