# Active audience: user-provided recording

The app now uses all **nine chronological reactions** extracted from:
`KITKAT_2026-09-14_08-50-34.mp4`

The recording visibly shows Kinoton's *Sitcom Laughter 9x, Small Audience* on Freesound (sound 383207), whose CC0 attribution is retained below. The app's active files were extracted from the supplied recording, not substituted with the earlier downloaded preview.

Files: `audience/audience-01.wav` through `audience/audience-09.wav`. Exact source cut times, output durations and checksums are in `audience/manifest.json`. Stereo 48 kHz/16-bit PCM WAV, normalized to -21 LUFS with short edge fades. The source recording is AAC; exporting WAV does not restore lossless source quality.

Rotation: heh = 09, 02, 06; audience = 04, 03, 08; big laugh = 05, 07; disbelief = 01. Suppressed triggers do not advance the rotation. The 0.99 spoken line is unchanged.

Reproduce with `python3 scripts/extract-recorded-audience.py` from the project root.

## Earlier preview cuts (retained, no longer selected by playback)

Source: **Sitcom Laughter 9x, Small Audience**, Kinoton, Freesound sound 383207, published 2017-03-07.

- Source page: https://freesound.org/people/Kinoton/sounds/383207/
- Licence: Creative Commons Zero (CC0 1.0), verified on the source page 2026-09-14.
- Licence URL: https://creativecommons.org/publicdomain/zero/1.0/
- Downloaded file: https://cdn.freesound.org/previews/383/383207_2247456-hq.mp3
- The publicly downloadable high-quality MP3 preview contains the full 43.354813 seconds. The original 48 kHz/24-bit WAV requires a Freesound login; it was not downloaded. These WAV cuts are decoded from the preview and do not recover the original lossless quality.

Edits (source start, duration):

| Output | Start | Duration | Target loudness |
| --- | ---: | ---: | ---: |
| heh.wav | 40.25s | 2.35s | -23 LUFS |
| audience.wav | 15.05s | 2.95s | -21 LUFS |
| big_laugh.wav | 24.00s | 4.60s | -19 LUFS |
| absolute_fucking_disbelief.wav | 0.00s | 6.75s | -18 LUFS |

Cuts include short fades, loudness normalization, and conversion to 48 kHz/16-bit stereo WAV. Reproduce with `python3 scripts/cut-audience.py` from the project root; the source preview is retained in `assets/audio-source/`.

`a_jebote.wav`: locally synthesized with the installed macOS Croatian **Lana** voice, speaking “A jebote…”. This is a synthetic Croatian stand-in, **not an authentic Dalmatian performance**. Replace it with an original approved recording for the intended delivery. The app supplies 1.4 seconds of silence before playback; that pause is not baked into the file.

No television-series audio is used. All runtime playback is local.
