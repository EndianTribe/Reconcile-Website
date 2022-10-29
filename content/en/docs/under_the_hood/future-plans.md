---
title: "Future Plans"
description: "Planned Features"
lead: ""
date: 2020-10-06T08:48:57+00:00
lastmod: 2020-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "under_the_hood"
weight: 400
toc: true
---

## Development Improvements

### CI/CD

Not having to manually deploy to Google Play Store for every new release would be nice.

### Code Style Enforcement

At the moment [linting](https://developer.android.com/studio/write/lint) is optional. One day I plan to clean up my code and enforce lint rules. One day.

### Error Handling

At the moment I am certain there are uncaught exceptions. I intend to catch them all.

### Replace Static Fields with String Resources

I plan to replace static string fields with `@StringRes` for better testability.

### Consolidate Modifiers

Consolidating [Jetpack Compose modifiers](https://developer.android.com/jetpack/compose/modifiers) would make them much easier to manage.

## Performance Improvements

### Data Paging

[Data paging](https://firebase.google.com/docs/firestore/query-data/query-cursors) should improve performance tremendously for large datasets.

### Server-Side Fair Use Limits

Since the backend uses Firebase Firestore, I will need to implement server-side fair use limits to make sure malicious users don't torpedo me into bankruptcy.

### Server-Side Permissions

It is a good idea to treat all clients as potentially malicious. [Server-side permissions](https://firebase.google.com/docs/firestore/security/overview) should keep naughty users at bay.

### Reauthenticate User Prior to Deletion

[Firebase Authentication](https://firebase.google.com/docs/auth) requires security-sensitive operations such as account deletion to take place within 5 minutes of authentication. Otherwise an exception is thrown. At this moment the user is advised to manually log out an then log back in before they attempt account deletion. I plan to implement an automated version.

## Usability Improvements

### Auto Suggestions on Entry Screen

It would be nice for the app to automatically suggest the frequently used counterparties when adding journal entries, wouldn't it?

### Add Duplicate and Negate Entry

If a user simply wants to duplicate or negate an existing journal entry, there should be an easy way to do that instead of having to type in all the required information on the new journal entry screen.

## Features

### Search

Search is currently actively being worked on.

### Detailed Statistics

In addition to cumulative sums, I plan to add other relevant statistics. For instance category breakdowns, running totals, average outstanding balance, etc.

### Automatic User Data Cleanup

When a user deletes their account, their data are immediately orphaned server-side and require manual cleanup. An automated server-side script or [Firebase Cloud Function](https://firebase.google.com/docs/functions) should take care of it automatically.

### Tutorial Mode

It would be nice to have a tutorial mode for new users instead of requiring them to read an oversized tome that is my user manual.

### Recurring Expenses

Recurring expenses are an almost unavoidable feature in long-term active relationships (e.g., roommates, partners, etc). Having an automatic way of entering regularly recurring expenses (e.g., rent, internet, etc) would be nice.

### Multiple Users

At the moment counterparties are simply strings. I intend to turn them into objects to enable more sophisticated operations with them.

### Payment Method Implementation

It would be most convenient if outstanding balances can be reconciled automatically among trusted parties, wouldn't it?
