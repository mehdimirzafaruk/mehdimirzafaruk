### Hi, I'm Mehdi 👋

I build small, **local-first** desktop tools — mostly Python and JavaScript, mostly for Windows.
The rule I keep coming back to: your data stays on your machine unless you explicitly send it somewhere.

---

## Selected work

**[AI Limit Tray](https://github.com/mehdimirzafaruk/ai-limit-tray)**
Electron tray app that tracks Codex and Claude usage limits without opening a browser tab.
Shows remaining quota per account and per window, live session context, and compaction events,
plus a click-through overlay pinned to the active editor window.
`JavaScript` · `Electron` · **55 tests** · [`v0.1.0` release](https://github.com/mehdimirzafaruk/ai-limit-tray/releases)

**[AI Seçim Studio](https://github.com/mehdimirzafaruk/background-remover)**
Photo cutout editor. `rembg` produces the first mask, then you refine it by hand with brushes,
lasso, polygon and a magic wand, and export a transparent PNG. I built it because every tool I
tried gave you either no AI step or an AI mask you couldn't touch up.
`Python` · `Tkinter` · `rembg`

**[CS2 Voice Chat Translator](https://github.com/mehdimirzafaruk/cs2-voice-translator)**
Always-on-top overlay that transcribes speech **locally** with `faster-whisper` and shows the
translation in a screen corner. Push-to-translate hotkey; audio never leaves the machine.
`Python` · `faster-whisper` · `Tkinter`

**[MP4 Watermark Remover](https://github.com/mehdimirzafaruk/watermark-remover)**
Removes a static watermark by inpainting the covered area frame by frame. Finds the box
automatically from per-pixel temporal variance intersected with a Canny edge map.
`Python` · `OpenCV` · `ffmpeg`

<details>
<summary><b>More tools</b></summary>

<br>

- **[Görsel İşleme Aracı](https://github.com/mehdimirzafaruk/file-converter)** — batch image and document converter with AI background removal, 5 UI languages, everything local
- **[Anti-Theft Alarm](https://github.com/mehdimirzafaruk/anti-theft)** — Telegram message the moment your laptop's charger is unplugged; the earliest theft signal there is
- **[Auto Clicker](https://github.com/mehdimirzafaruk/auto-clicker)** — hold-to-click, 1–50 CPS; filters out its own synthetic input using the `WH_MOUSE_LL` `LLMHF_INJECTED` flag
- **[Sleep Preventer](https://github.com/mehdimirzafaruk/sleep-preventer)** — keeps Windows awake via `SetThreadExecutionState`, no cursor jiggling

</details>

---

## How I work

**Local-first, always.** Background removal, speech recognition, file conversion — none of it
uploads anything. When a cloud step is unavoidable (translation), it only ever sees text I
already had on disk, never the raw audio or image.

**Commit messages that explain the bug, not the diff.** "`hook callback`'ini modül seviyesinde
tut, yoksa `ctypes` GC ediyor ve crash" tells you far more than "fix hook". I write them for
whoever debugs this next — usually me, six months later.

**Comments where the reason isn't obvious.** The code says *what*; the comment should say *why*.
If the answer is "because Windows does something surprising here", that belongs in the file.

## Toolbox

`Python` · `JavaScript` · `Node.js` · `Electron` · `Tkinter` / `CustomTkinter` · `OpenCV` ·
`ctypes` / Win32 · `ffmpeg` · `SQLite`
