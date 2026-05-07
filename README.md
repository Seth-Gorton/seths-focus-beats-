# seth's focus beats

A web-based focus music player. Streams real human-made music from listener-supported internet radio (SomaFM, FIP, NTS) and overlays a **16 Hz beta-range amplitude modulation** on top of it via the Web Audio API. The modulation rate is taken from [Woods et al. 2024](https://www.nature.com/articles/s42003-024-07026-3) — *"Rapid modulation in music supports attention in listeners with attentional difficulties"* — which found that 16 Hz AM produces the strongest sustained-attention benefit in EEG/fMRI studies, especially for listeners with attentional difficulties.

Single HTML file, no build step, no backend.

## Live

Once GitHub Pages is enabled, the app will be at:
**https://seth-gorton.github.io/seths-focus-beats-/**

## Run locally

Open `index.html` in any modern browser. That's it.

## Modes

| mode | freq | stations |
|---|---|---|
| **focus** | 16 Hz (beta) | Mission Control · Beat Blender · Cliqhop IDM |
| **flow** | 8 Hz (alpha) | Drone Zone · Deep Space One · Space Station |
| **house** | 16 Hz (beta) | The Trip · FIP Électro · NTS 1 |
| **energy** | 32 Hz (gamma) | Groove Salad · Secret Agent · DEF CON Radio |

`skip ⇥` cycles stations within the current mode. `👎` permanently swaps the current station for one from a backup pool (persisted in localStorage). Tracks also auto-rotate every 10–15 min.

## Features

- Real human-made music streamed from internet radio
- 16 Hz beta-range AM applied via Web Audio for entrainment
- Live track metadata (artist + title) for SomaFM stations
- Session logging persisted to localStorage
- Stats dashboard: sessions, streaks, peak hour, favorite station, GitHub-style activity heatmap
- Light/dark theme
- Master compressor + light saturation for a polished mix
- Wake Lock so the OS doesn't suspend the tab during long sessions

## Keyboard shortcuts

- `Space` — play / pause
- `→` — skip station
- `Esc` — close stats overlay

## Music sources

- [SomaFM](https://somafm.com) — listener-supported, commercial-free internet radio (San Francisco, since 2000)
- [FIP](https://www.radiofrance.fr/fip) — Radio France's electronic & groove streams
- [NTS Radio](https://www.nts.live) — London's underground electronic music station

All streams are free and public; this app is a player + entrainment overlay on top of them.

## License

MIT
