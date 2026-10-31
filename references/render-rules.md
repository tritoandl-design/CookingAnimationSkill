# Render rules

## Muse first, within the weekly token allowance

- Render image and video with Muse only within the weekly token allowance.
- A weekly allowance top-up kept as reserve is not for everyday rendering, unless the owner says otherwise.
- If Muse video returns a region restriction, for example 403 `video_not_available` ("Video generation isn't available in your country or region"), that is a long-lasting restriction, not a temporary error. Stop using that tool for the film. Do not retry it through the same tool, do not try scenes 2-6 after scene 1 fails that way, and do not assemble a final from failed renders.

## Google Flow fallback

- When Muse cannot render (DNA, poster or scene), go into the owner's Google Flow yourself and bring the file back. Do not hand the owner a prompt block and wait, except when Flow is also unavailable or refusing after a rewrite.
- Account in the proven workflow: tritoandl@gmail.com. Never create an account and never pay. If Flow credit runs out, report to the owner for another account.
- Render 360p, download upscaled to 720p. This saves credit and still gives a 720p output.
- Render scenes in order, one at a time. Verify the real downloaded file exists, is about 10 seconds and 720x1280, before starting the next scene. A report that says "downloaded" without a real file does not count.
- Chain by last frame: scene 2 uses scene 1 as reference, scene 3 uses scene 2, and so on. Once a last frame exists, do not add a separate close-up face reference.
- Uploads to Flow that are allowed by default: character DNA, last frames for scene chaining, posters and other images needed for Flow media rendering. That permission covers Flow rendering only.
- Check frames for character and dish drift before assembly. Drifted frame = re-render, do not deliver.

## Final assembly (when the user asks for it)

- Pad each scene to exactly 10.000 seconds (video pad, audio pad), concatenate, and re-encode Android-safe:
  - Video: `-vf format=yuv420p -c:v libx264 -profile:v high -level 4.0`
  - Audio: `-c:a aac -b:a 128k -ar 48000 -ac 2`
  - Flags: `-movflags +faststart`
- Verify with ffprobe before delivering: duration, resolution, yuv420p, AAC stereo 48kHz, faststart.
- Give every new final version a new filename. Never overwrite a previous final.
- A file in an "approved" folder does not by itself mean approved. Only the owner's explicit approval counts.
