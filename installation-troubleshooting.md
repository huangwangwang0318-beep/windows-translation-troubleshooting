---
layout: default
title: Installation Troubleshooting
---

# Installation and Startup Troubleshooting on Windows

Treat downloading, verifying, installing, and launching as four separate stages. Repeating the installer without knowing which stage failed can overwrite evidence and make the original problem harder to reproduce.

## 1. Verify the download completed

Open the browser download list and confirm that the file is complete rather than paused, interrupted, or renamed as a partial download. Compare its filename and approximate size with the publisher's current information. Avoid installers copied from third-party download portals when a publisher-controlled source is available.

For an application-specific example, use this independent [Windows installation troubleshooting guide](https://trans-youdao.com/youdao-windows-install-guide/) and compare every download detail with the publisher's current documentation.

## 2. Inspect the file before running it

Right-click the installer, open **Properties**, and inspect the **Digital Signatures** tab when present. Check that the signer matches the expected publisher and that Windows reports a valid signature. A missing signature is not automatic proof of malware, but it is a reason to stop and verify the source.

Do not bypass a SmartScreen or antivirus warning merely to complete the installation. Record the exact warning and verify the file through the publisher or your administrator.

## 3. Check space and permissions

Confirm that the system drive and the chosen application drive have adequate free space. Use a normal user account first. If the publisher specifically documents that elevated installation is required, close unrelated programs and use the standard Windows elevation prompt rather than changing broad security settings.

## 4. Separate installer failure from startup failure

If installation completes but the program will not open, restart Windows once and test again. Then record whether a process appears briefly in Task Manager, whether a window is blank, and whether an error is shown.

A blank account or sign-in panel can indicate a WebView2 Runtime problem. A crash before any window appears may instead involve a damaged package, missing runtime, security product conflict, or corrupted application data.

## 5. Repair before removing user data

Use the application's documented repair option or Windows **Installed apps** controls when available. Preserve dictionaries, terminology files, user templates, and logs before uninstalling. Avoid deleting application-data folders unless the publisher specifically recommends it and a backup exists.

## 6. Validate the repaired installation

Test one basic text translation first, then sign-in, image OCR, and document upload separately. Restore optional integrations only after the core workflow works. Recording each result makes future updates easier to diagnose.

## What to include in a support request

- Windows edition and build
- Application version
- Installer filename and signature result
- Exact error message
- Whether the failure occurs during install or launch
- Whether WebView2 content displays
- Which repair steps were tested

This document is an independent reference and is not an official support channel for any software vendor.
