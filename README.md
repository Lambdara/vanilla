Vanilla Reprise
================

Vanilla Reprise is a modified fork of [Vanilla Music](https://github.com/vanilla-music/vanilla), a GPLv3 licensed MP3/OGG/FLAC/PCM player for Android.

This fork is not the official Vanilla Music project. It keeps the original copyright notices, license text, and in-app acknowledgements, while using a distinct app name, package id, and launcher icon so it is not confused with upstream Vanilla Music.

Fork Identity
-------------

* App name: Vanilla Reprise
* Android application id: `lambdara.vanillareprise`
* Upstream project: [vanilla-music/vanilla](https://github.com/vanilla-music/vanilla)
* License: [GNU GPLv3](LICENSE), with included MIT/Apache notices preserved where applicable

Notable Fork Changes
--------------------

* Renamed the app from Vanilla Music to Vanilla Reprise.
* Changed the Android application id so it installs separately from upstream Vanilla Music.
* Replaced the launcher icon with distinct Vanilla Reprise artwork.
* Fixed media-session notification metadata so the lock screen shows the current song title and album art.

Features Inherited From Vanilla Music
-------------------------------------

* multiple playlist support
* grouping by artist, album or genre
* plain filesystem browsing
* [ReplayGain](https://en.wikipedia.org/wiki/ReplayGain) support
* headset/Bluetooth controls
* accelerometer/shake control
* cover art support
* [Simple Last.fm Scrobbler](https://github.com/tgwizard/sls) support

Plugins
=======

Vanilla Reprise currently keeps Vanilla Music plugin compatibility where practical. Existing Vanilla Music plugins may still identify themselves using the upstream Vanilla plugin API names:

* [Cover fetcher](https://play.google.com/store/apps/details?id=com.kanedias.vanilla.coverfetch)
* [Lyrics search](https://play.google.com/store/apps/details?id=com.kanedias.vanilla.lyrics)
* [Tag editor](https://play.google.com/store/apps/details?id=com.kanedias.vanilla.audiotag)
* [Headphone detector](https://play.google.com/store/apps/details?id=ch.blinkenlights.android.vanillaplug)

Attribution
===========

Vanilla Music was created and maintained by Adrian Ulrich and contributors. This repository is a downstream fork and does not claim to be the official Vanilla Music app.

The original upstream community and issue tracker are:

* Website: https://vanilla-music.github.io/
* Source and issues: https://github.com/vanilla-music/vanilla
* Community: https://www.reddit.com/r/vanillamusic

Please report Vanilla Reprise-specific issues to this fork rather than upstream Vanilla Music.

Building
========

To build you will need:

* A Java compiler compatible with Java 1.8 or newer
* The Android SDK with the configured compile SDK installed

Building from command line:

```sh
./gradlew build
```

Install a debug build to a connected device:

```sh
./gradlew installDebug
```

Documentation
=============

Javadocs can be generated using:

```sh
./gradlew javadoc
```
