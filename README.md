# Lyt

**A privacy-focused web browser for Windows, built on Chromium.**
Pronounced "light". *Your browser. Your business.*

> **Status: early development.** Lyt is an experimental alpha being built now. There is no public download yet. This page shows what is being made; it is not the source code.

---

## What Lyt is

Lyt is a native desktop browser, a real fork of current Chromium rather than a skin over another browser. It aims to be private by default without needing hours of setup, while keeping the website compatibility and extension support people expect from a Chromium browser.

## Progress

**30 October 2026: the first real Lyt build is running.** It is built on Chromium 157 and passes all 12 of its automated checks. These include:

- **Full uBlock Origin works.** It installs cleanly, blocks a tracker request before it leaves the browser, hides ads on the page, and runs alongside a modern (Manifest V3) extension.
- **Memory Saver is on by default.** An idle tab is put to sleep to free memory and comes back when you return to it. Tabs you are using are left alone: the one you are looking at, one playing audio, one using the camera, one with unsaved form input, and sites you have exempted.
- **Private defaults are in place.** Third-party cookies are blocked, search suggestions are off, and page preloading is off.

These are automated tests on a developer build. It is not a release, and it has not yet had a hands-on review or wider testing.

**Next up (designed, not built yet):**

- **Lyt's own look.** Floating rounded tabs and a flat, rounded address bar, in a warm charcoal and orange colour scheme called "Ember". The first build looks too much like Chrome, so this comes next.
- **A lightweight Lyt new-tab page.** A clock and date, your shortcuts, and optional weather. Weather is off until you choose a town, and only then does it fetch a forecast, using a rounded, approximate location and at most once an hour.
- **Privacy Badger alongside uBlock Origin.** Planned, not done yet. It is not part of the build today.

## Planned for the first alpha

- **Full uBlock Origin, built in.** The complete uBlock Origin, not the "Lite" version, ready from first launch, with its dashboard and element picker.
- **Privacy Badger, built in (planned).** EFF's tracker-learning blocker will sit alongside uBlock Origin, handling trackers that filter lists miss.
- **Private defaults.** Third-party cookies blocked. No search-as-you-type sent to a search engine. No speculative page preloading. No usage telemetry. No account required.
- **Memory Saver on by default.** Idle tabs release memory and reload when you return to them. You choose how aggressive it is and which sites are exempt.
- **A compact, dark interface.** A slim tab strip and toolbar that give the page more of the screen, with Lyt's own look and new-tab page (see Progress above).
- **Your extensions.** Chrome Web Store extensions are supported, and popular ones are tested individually.

## Further out

- **Lyt Shield:** one place to see and control what each site can do (cookies and storage, fingerprinting protection, "forget this site", and temporary fixes for broken sites).
- Stronger protection against cross-site tracking and fingerprinting, guided by measurement rather than marketing claims.
- An installer with signed, verified updates.

## Principles

- **Honest claims.** Lyt will only claim the protections it has tested, and will say what it does not protect against.
- **Security first.** Chromium's sandbox, site isolation and certificate checks stay intact. Privacy is never bought by weakening security.
- **Local first.** No browsing data leaves your device for Lyt's benefit.

## Status

| Milestone | State |
| --- | --- |
| Product design and privacy feature research (120 items) | Done |
| Build tooling and pinned Chromium source | Done |
| First native build | Done: passes all 12 automated checks (30 Oct 2026) |
| Lyt's own look and new-tab page | Designed, not built yet |
| Privacy Badger bundled | Planned |
| Usable developer alpha | Not yet |
| Public download | Not yet |

## Credits

Lyt is built on [Chromium](https://www.chromium.org/) by The Chromium Authors. It bundles [uBlock Origin](https://github.com/gorhill/uBlock) by Raymond Hill and contributors, and plans to bundle [Privacy Badger](https://privacybadger.org/) by the Electronic Frontier Foundation. Both are GPL-3.0 projects and are credited under their own licences. Their inclusion does not imply endorsement by their authors.

## Licence

Lyt is **not open source**. Copyright (c) 2026 the Lyt author. All rights reserved. See [LICENSE.md](LICENSE.md).
