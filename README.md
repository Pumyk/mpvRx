# mpvRx

A libmpv-powered Android media player. This is a community build of the upstream
**mpvRx** project, with a set of features ported across from **REX-Player**.

This repository hosts that combined build. It is a merge, not the work of a single
author, and it stands entirely on the two upstream projects credited below.

| | |
|---|---|
| Package | `app.gyrolet.mpvrx` |
| Version | 3.0.2.1 (versionCode 30399992) |
| Min Android | 8.0 (API 26) |
| Target SDK | 36 |
| Architectures | `arm64-v8a`, `armeabi-v7a`, `x86`, `x86_64` |
| Licence | AGPL-3.0 |

## Credits

This app could not exist without the following projects. All credit for the
foundation and the ported functionality belongs to them.

### Base application

**mpvRx** — [github.com/Riteshp2001/mpvRx](https://github.com/Riteshp2001/mpvRx)

The complete application: player, UI, and the libmpv integration this build is
assembled on. mpvRx is the upstream and the source of the overwhelming majority of
the code here.

### Ported features

**REX-Player** — [github.com/mpvRex/REX-Player](https://github.com/mpvRex/REX-Player)

Several features and behaviour refinements were ported from REX-Player into the
mpvRx base to produce this build.

### Native libraries and components

- **mpv / libmpv** — the playback engine — [mpv.io](https://mpv.io)
- **FFmpeg** — decoding, demuxing, filtering — [ffmpeg.org](https://ffmpeg.org)
- **mpvlib** (`app.gyrolet.mpvlib`) — prebuilt libmpv/FFmpeg Android binaries
- **yt-dlp** — stream extraction — [github.com/yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp)
- **QuickJS-NG** — JavaScript engine used by yt-dlp — [github.com/quickjs-ng/quickjs](https://github.com/quickjs-ng/quickjs)
- **libtorrent4j** — torrent streaming — [github.com/aldenml/libtorrent4j](https://github.com/aldenml/libtorrent4j)
- **MediaInfoLib**, **libarchive**, **libzen** — media and archive inspection
- **AndroidX / Jetpack Compose** — Google

### Maintainer

**Mfoniso Udoma ([@Pumyk](https://github.com/Pumyk))** — undertook the merge of REX-Player
features into the mpvRx base, and maintains this combined build and its releases.

## Downloads

Grab an APK from the [Releases](../../releases) page.

- **universal** — all four ABIs, install this if you are unsure. Works on every
  supported device, including older 32-bit and x86 hardware.
- **arm64-v8a** — 64-bit ARM only. Smaller download, covers essentially all phones
  made in the last several years.

Both builds are the same application; they differ only in the native libraries
packaged inside them.

### A note on signing

The universal build is signed with this repository's own release key, so switching
between the two APKs requires uninstalling the one you currently have. If you were
running an earlier `arm64` build made outside this repository, uninstall it once
before installing anything from here.

## Licence

This project is licensed under the **GNU Affero General Public License v3.0**,
inherited from both upstream projects. See [LICENSE](LICENSE).

Because this is a combined work of two AGPL-3.0 projects, it must remain AGPL-3.0.
If you redistribute it or run a modified version as a network service, the AGPL
requires you to make the corresponding source available.

## Disclaimer

This is an unofficial community build. It is not affiliated with or endorsed by the
mpvRx or REX-Player maintainers. Do not report issues with this build to those
projects — report them here instead.
