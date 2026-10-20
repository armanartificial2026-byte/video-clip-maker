# Video Clip Maker 🎬

**Cut short vertical clips from your long videos — free, right in your browser.**

Turn a 20-minute video into crisp 9:16 clips for YouTube Shorts, Instagram Reels and TikTok — without opening heavy editing software and without uploading your footage anywhere.

🌐 **Try it live:** https://estegysol.com/tools/video-clip-maker/

## Features

- ✂️ Mark in/out points on any video and export multiple clips at once
- 📱 Vertical 9:16 MP4 output (1080×1920) for Shorts / Reels / TikTok, or original aspect ratio
- 🎯 Adjustable crop position (left / center / right)
- 🔒 100% private — your video never leaves your device
- 🆓 Free forever, no signup, no watermark
- 🖥️ Works best on desktop Chrome / Edge

## How it works

Everything runs in your browser using [FFmpeg.wasm](https://ffmpegwasm.netlify.app/) — the WebAssembly build of FFmpeg. Your video file is processed locally; nothing is uploaded to any server.

## How to use

1. Drop your long video into the page (MP4, WebM or MOV)
2. Play it, press **Set start** / **Set end** at the moments you want, then **Add clip** — repeat for as many clips as you need
3. Choose **Vertical 9:16** (with crop position) or keep the original ratio
4. Click **Load video engine** once (~30 MB one-time download, then cached), then **Create clips**
5. Download each finished MP4

## Run it yourself

This is a single static HTML file — no build step, no server needed:

```bash
# serve the folder with any static server, e.g.
npx serve .
# then open index.html
```

The only external dependencies are CDN libraries loaded at runtime (FFmpeg.wasm).

## License

MIT — free for personal and commercial use. See [LICENSE](LICENSE).
