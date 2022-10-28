---
title: "Rules of Accounting"
description: "Why Reconcile is designed the way it is"
lead: "Why Reconcile is designed the way it is"
date: 2020-10-06T08:48:57+00:00
lastmod: 2020-10-06T08:48:57+00:00
draft: false
images: []
menu:
  docs:
    parent: "overview"
weight: 250
toc: true
---

## Entry Immutability

Once a journal entry is entered onto the ledger, it cannot be changed.

If you discovered a mistake on an existing journal entry, enter another journal entry with the opposite value to cancel it out. You can even add notes to the journal entry to remind yourself (and the other party) the reason.

## No Backdating

A journal entry's date is timestamped by the server and cannot be modified.

If you wish to document the time of the expense, use the notes field.

## Why?

* Eliminates the possibility of "book cooking" whereby factitious entries are entered and then later removed or modified.
* Eliminates the possibility of "book cooking" whereby factitious entries are inserted to a much earlier point in the ledger to avoid detection.
* Enables referential integrity to journal entries. You can be sure any referred journal entry will always be there, at the exact location in the ledger, and will never change.
