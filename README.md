# Windows Translation Troubleshooting

This repository is a practical, product-neutral handbook for diagnosing Windows desktop translation tools. It is intended for users and support staff who need to separate download, installation, startup, network, proxy, embedded-browser, OCR, and document-processing failures without immediately reinstalling the application.

The material is deliberately organized by failure stage. A translation program can have a working home screen while its sign-in page, installer host, document-upload service, OCR endpoint, or translation API is unavailable. Testing those layers separately preserves evidence and usually shortens the repair process.

## Use this handbook safely

- Work with a non-sensitive test sentence or a small redacted document.
- Record the exact error message and the time it occurred.
- Change one variable at a time.
- Do not disable antivirus protection or certificate validation to make a test pass.
- Do not upload confidential files to an unknown service.
- Verify installers with the publisher's current documentation and digital signature information.

## Troubleshooting map

1. If the download never starts or stays at zero, begin with the browser download panel, proxy configuration, and network path.
2. If the installer will not run, verify the file, Windows security prompts, free disk space, and permissions.
3. If the application opens to a blank sign-in window, check WebView2 or the embedded browser runtime.
4. If plain text works but PDF or OCR fails, test a small document and isolate file-format, upload, and recognition problems.
5. If the application fails only after an update, preserve logs and compare the installed version with the publisher's current release information.

## Contents

- [Installation troubleshooting](installation-troubleshooting.md)
- [Network and proxy troubleshooting](network-troubleshooting.md)
- [Public handbook page](index.html)

## Independent-reference notice

This is an independent troubleshooting project. It is not affiliated with a translation-software vendor and is not an official support channel. Product names may be used only to identify the software being discussed. Always verify downloads and account or privacy requirements with the relevant publisher.

