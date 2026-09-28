# Auto Record — Audio/Video Stream Interceptor

Automated recorder for **Suno** tracks and **YouTube** audio/video, using a dedicated isolated Firefox instance to capture only the selected browser's audio and, for video, its screen output.

**GUI + CLI · Linux (PulseAudio/PipeWire) · Windows (WASAPI)**

**Audio:** MP3 · AAC · OGG · FLAC  
**Video:** MP4 · MKV · WebM · AVI · MOV · FLV · 3GP

<p align="center">
  <img src="ScreenShots/AVSI_00.png" width="50%">
</p>
<p align="center">
  <img src="ScreenShots/AVSI_01.png" width="50%">
</p>
<p align="center">
  <img src="ScreenShots/AVSI_02.png" width="50%">
</p>

## License

AutoRecord-AVSI is licensed under the **MIT License**. See [`LICENSE`](LICENSE).

The Linux AppImage includes the **AppImage Type-2 runtime** and its statically linked third-party components under their respective upstream licenses. These components are part of the AppImage runtime and are not relicensed as AutoRecord-AVSI code.

See [`THIRD-PARTY-NOTICES.md`](THIRD-PARTY-NOTICES.md) for the bundled runtime components, their licenses, and the external runtime dependencies used by the application.

### External dependencies

The current AppImage does **not** bundle the following runtime dependencies:

- Python 3 and Tkinter
- FFmpeg
- PulseAudio/PipeWire and related system utilities/libraries
- Firefox
- `wf-recorder` (optional, for Wayland screen recording)
- geckodriver (obtained separately at runtime)

These remain separate software components and are subject to their respective upstream licenses.

### AppImage build tool

`appimagetool` is used only during AppImage creation and is not included as application payload. Its license is therefore separate from the licenses of software actually contained in the resulting AppImage.

For details, see [`THIRD-PARTY-NOTICES.md`](THIRD-PARTY-NOTICES.md).

---

Donate $5 to buy food for a cat:
<br>
USDT(TRC20): TWEmMHfc5DbQuDru8oaXNoXxTNkqYJbsYv<br>
BTC(BEP20): 0x147d19ae0e1b50ca6c87d32b2f716068e6ba5b17<br>
SOL(SOL): j3kkX7VuKfchcnH8Y9bUCbqjjA4ssLpspvsw4YZi8ia<br>
