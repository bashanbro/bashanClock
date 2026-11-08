# bashanClock · Mathematical Harmonic Clock

**bashanClock** is an offline-capable mathematical clock made with plain HTML, CSS, and JavaScript. The hour dial uses twelve mathematical expressions instead of ordinary numerals. Each hour corresponds to an audio harmonic of 110 Hz.

> bashanClock 是一个无需后端、无需构建工具、可离线运行的数学谐波时钟。支持九种界面语言和六套表盘主题。

## Features / 功能

- Accurate live analog and digital time sourced from the device clock.
- Twelve mathematical hour expressions, including Euler's identity, the Riemann zeta function, Fibonacci numbers, combinations and infinite series.
- Hourly harmonics at `f = k × 110 Hz`, with a twelve-harmonic chord at noon/midnight based on amplitudes `1/k`.
- Nine interface languages: 简体中文 / 繁體中文 / English / 日本語 / 한국어 / Français / Español / Português / Русский.
- Six dial themes, responsive desktop/mobile layout, tick style customization, time-zone selection, and 12/24-hour display.
- Interactive audio playback using the browser Web Audio API and a live mathematical waveform.
- Settings stored locally in the browser where storage is available.
- One standalone `index.html`: no dependencies, no package installation, and no build step.

## Run locally / 本地运行

Open `index.html` directly in a modern browser. For a local development server:

```sh
python -m http.server 8000
```

Then visit `http://localhost:8000/`.

Browser audio requires a user gesture; turn on sound or press a playback control first. Browsers may pause timers or audio while a tab is in the background, so this is not a reliable background alarm clock.

## Deploy to GitHub Pages / 部署

1. Create a **public** repository named `bashanClock` under your GitHub account.
2. Upload `index.html`, `README.md`, and `.nojekyll` to its `main` branch (upload individual extracted files, not the ZIP).
3. Open **Settings → Pages**.
4. Choose **Deploy from a branch**, `main`, `/(root)`; save.
5. Open **https://bashanbro.github.io/bashanClock/** once Pages finishes publishing.

GitHub Pages hosting from private repositories depends on your GitHub plan. The public repository option is easiest for a free, public demo.

## Integration with Bashan Lab

The same version of bashanClock is also preserved at:

- https://bashanbro.github.io/playground/bashan-clock/

Once your independent repository is restored, you can link its GitHub URL on the Bashan Lab homepage.

## Math notes / 数学说明

- `−e^(iπ) = 1`
- `Σ 2^(−n), n=0…∞ = 2`
- `⌊π⌋ = 3`, `⌈π⌉ = 4`
- `4.9̅ = 5`, `3! = 6`, `4²−3² = 7`, `F₆ = 8`, `1³+2³ = 9`
- `C(5,2) = 10`, `1011₂ = 11`
- `−1/ζ(−1) = 12`, where `ζ(−1) = −1/12` via analytic continuation.

## Attribution

Project owner: [bashanbro](https://github.com/bashanbro). No license is declared by this recovery package; all rights remain with the project owner until a license is added.
