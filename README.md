# VoiceLedger

Windows and Android local-first voice capture, transcription, translation, speaker attribution, and encrypted cross-device sync.

## Specification

The product and implementation specification is being prepared in `docs/spec/`.

- Native UI: WPF on Windows; Kotlin/Jetpack Compose on Android.
- Shared business core: proposed Rust library, subject to the cross-target build spike.
- Local-first: audio is persisted on-device before AI work; no dedicated VoiceLedger server is required.
- AI: hardware-aware model recommendations and adaptive local inference; recording-only mode always remains available.
- Sync: optional client-side encrypted WebDAV/S3 object storage.

See `AGENTS.md` and `docs/spec/` before implementation. Hardware/model/sync gates remain unverified until supported by test evidence.
