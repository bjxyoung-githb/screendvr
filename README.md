# ScreenDVR

A browser-based screen recorder that works like a TV DVR: record whatever is on your screen, pause or rewind while it keeps recording, bookmark moments, and play recordings back later.

**Live app:** https://bjxyoung-githb.github.io/screendvr/

## Features
- Capture a whole screen, a window, or a browser tab (with tab/system audio)
- DVR controls while recording: pause, rewind/forward 10 s or 30 s, jump to live
- Bookmarks (marks) to jump back to key moments
- Library with thumbnails: play, rename, pin, download (.webm), delete
- Playback at 0.5×–2× speed
- **Editor** with two modes — *Keep selection* (trim the ends) and *Cut out selection* (remove a middle section and join the rest). Drag start/end handles on a filmstrip timeline (or press I / O), preview, then save as a new copy or replace the original. Trims are instant and lossless; recordings made before v1.1.0 may need a short real-time re-record for an exact start.
- Auto-stop timer and storage cap (oldest unpinned recordings removed first)
- Recovers footage if the tab closes mid-recording

## Requirements
- Chrome or Edge on a desktop/laptop (phones and tablets can't capture the screen from a web page)
- HTTPS or a local file (screen capture is blocked on plain HTTP)

## Notes
- Recordings are stored locally in the browser (IndexedDB) — download anything you want to keep.
- DRM-protected streaming video (Netflix, Hulu, Disney+, Prime, etc.) records as a black screen; the browser blocks it.
- `BUILD_VERSION` in `index.html` is shown in the header badge — bump it each deploy.
