# Third-Party Notices

AutoRecord-AVSI is distributed under the MIT License. The MIT License in the
repository root applies to the original AutoRecord-AVSI source code.

This file documents third-party software relevant to the Linux AppImage build
and runtime. Third-party software remains under its respective upstream
license and is not relicensed by AutoRecord-AVSI.

## Components bundled into the AppImage

The Type-2 AppImage runtime is embedded into the final AppImage by
`appimagetool`. The runtime contains statically linked third-party code.

### AppImage Type-2 runtime

- Project: AppImage Type-2 runtime
- License: MIT
- Copyright: 2004-23 probonopd
- Source: https://github.com/AppImage/type2-runtime
- License: https://github.com/AppImage/type2-runtime/blob/master/LICENSE

The runtime license also identifies the following statically linked
third-party components:

- musl libc — license: https://git.musl-libc.org/cgit/musl/tree/COPYRIGHT
- libfuse — LGPL-2.1 — license:
  https://github.com/libfuse/libfuse/blob/master/LGPL2.txt
- squashfuse — license:
  https://github.com/vasi/squashfuse/blob/master/LICENSE
- libzstd — license:
  https://github.com/facebook/zstd/blob/dev/LICENSE
- zlib — license:
  https://zlib.net/zlib_license.html

These components are part of the AppImage runtime, rather than of the
AutoRecord-AVSI application source itself.

## External runtime dependencies

The following components are required by the current AutoRecord-AVSI
AppImage/runtime environment but are NOT bundled into the AppImage by the
project's current `build-appimage.sh` and `AppDir/AppRun`:

- Python 3
- Python Tkinter
- FFmpeg
- PulseAudio/PipeWire runtime and utilities (`pactl`, `parec`, and related
  system libraries)
- Firefox
- `wf-recorder` (optional, for Wayland screen recording)
- geckodriver (obtained separately at runtime; not bundled into the AppImage)

These components remain subject to their own upstream licenses. Users and
redistributors who separately install or redistribute them are responsible
for complying with those licenses.

## Build-time tool

### appimagetool

`appimagetool` is used to create the AppImage during the build process. It is
a build-time tool and is not itself part of the final AppImage payload.

- License: MIT
- Copyright: 2004-25 Simon Peter and the AppImage Team
- Source: https://github.com/AppImage/appimagetool
- License: https://github.com/AppImage/appimagetool/blob/master/LICENSE

The appimagetool project explicitly states that its license does not apply to
the contents of AppImages created with it. The licenses of the software
actually included in an AppImage therefore need to be considered separately.

## Scope

This notice covers the third-party components identified from the current
AppImage build configuration and AppRun. If the AppDir is changed to bundle
additional libraries, interpreters, binaries, fonts, icons, or other
third-party material, their corresponding licenses and copyright notices
should be added here before distributing the resulting AppImage.
