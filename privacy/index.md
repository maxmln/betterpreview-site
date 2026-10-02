---
title: Privacy Policy
---


**Last updated: 1 October 2026**

Better Preview does not collect any data about you.

That is the whole policy. The rest of this page explains how the app is built so you can
check the claim rather than take it on trust.

## No data leaves your Mac

Better Preview has no network access. The app is sandboxed, and its sandbox entitlements
grant it exactly one capability: read and write access to folders you choose yourself,
through the open panel or by dragging them onto the window. There is no entitlement for
outgoing or incoming network connections, so the app cannot contact a server even in
principle.

There are no analytics, no crash reporting services, no advertising identifiers, and no
third-party SDKs of any kind.

## No account

There is nothing to sign up for and nothing to sign in to. The app never asks for an email
address, a name, or any other personal detail.

## What the app writes to disk

Two things, both local:

1. **`.betterpreview.json`**, a hidden file inside the folder you open. It records which
   photos you picked, shortlisted, rejected or placed in your portfolio, which folders you
   hid from the sidebar, and the order of your portfolio. It contains file paths relative
   to the folder you opened, and nothing else. Delete it and every decision is gone; the
   photos are untouched.
2. **An exception log**, written only if the app hits an unhandled error, inside the app's
   own sandbox container at
   `~/Library/Containers/com.maxmln.betterpreview/Data/Library/Logs/`. It stays on your Mac.
   It is never transmitted anywhere.

## Your photos

Better Preview reads your image files in order to display them. It never modifies or
re-encodes them.

Files move on disk only when you explicitly ask for it, through one of two menu commands:
copying your portfolio out to a folder you choose, or moving a folder's rejected photos
into a `Rejected` subfolder. Both tell you how many files they touched.

## Apple

Apple may give the developer anonymous, aggregated sales and crash statistics for apps
bought through the Mac App Store. That reporting is Apple's, is not something the app
participates in, and is covered by
[Apple's privacy policy](https://www.apple.com/legal/privacy/).

## Changes

If this policy ever changes, the updated version will be posted on this page with a new
date at the top. A change that affected what the app does with your data would also require
a new version of the app, reviewed by Apple.

## Contact

Questions about this policy: **maxbogdanoff@gmail.com**
