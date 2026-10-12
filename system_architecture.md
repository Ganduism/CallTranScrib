# CallScribe 1.0.0

The Windows executable runs a loopback HTTP server and opens a browser startup menu. Windows DPAPI protects the user's Sarvam key in Local AppData. The server invokes Saaras v4 in codemix mode, with speaker diarization and optional speaker count; the browser receives only review data and a temporary local session capability.

Imports are hashed and retained unchanged. Audio decoding is streamed through PyAV to produce waveform peaks; no local speech model is shipped. Cloud job IDs are persisted before uploading and used for Resume. Review structures, context and checked flags are saved to atomic JSON files. TXT, JSON and portable HTML exports retain provenance and review status. Restoring a portable HTML review verifies its embedded audio hash and preserves its annotations.

The UI reuses the accepted waveform/transcript layout, dark mode, speaker names, timed box editor and context recorder. A small service adapter adds server persistence across restarts. The distribution has no project recordings, personal key or model weights; it includes its source and dependency license notices.
