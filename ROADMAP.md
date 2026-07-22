# Grand Media Station — Roadmap

What's coming to GMS, in three buckets. No dates — items ship when
they're ready. Want something moved up? **👍 its issue** (or open one):
votes genuinely reorder the Proposed list.

_Last updated: 2026-07-22._

## Shipped highlights ✅

Already in the app today:

- Smart renaming with preview, profiles, and full undo (Track Record)
- Library management: browse, organize, playlists, duplicate & quality
  scanning, storage insights
- **Caption Car** — on-device AI subtitle generation (nothing uploaded),
  with a review queue, confidence highlighting, and audio-sync tools
- Transcoding with GPU acceleration, savings analysis, and safe
  replace-or-keep-both output
- Media-server integration (Plex / Jellyfin) with library sync
- Fully offline-capable — online features are optional

## In progress 🔨

- **Subtitle translation + multilingual generation** — generate or
  translate subtitles into multiple languages in one pass, on-device
- **Subtitle accuracy analysis** — score how well a subtitle matches the
  spoken audio, and jump straight to the mismatched sections
- **Auto-playlists** — build playlists from franchises/collections and
  folders, and push them to your media server
- **Deep verification** — a stronger "is this file really that episode?"
  check for library audits

## Planned 📋

- **Dialogue boost** — audio normalization that lifts quiet dialogue
  without blowing out loud scenes
- **Multi-version awareness** — first-class handling of multiple cuts /
  qualities of the same title
- **Local automation API** — a local REST API + MCP server so tools and
  AI assistants can drive GMS on your machine
- **Tdarr integration** — hand off transcode jobs to an existing Tdarr
  setup
- **Multi-server support** — manage libraries across more than one media
  server

## Proposed 💭 (vote!)

Ideas under consideration — 👍 the matching issue to push one up:

- **Cross-device pipelines** — pair two of your GMS installs and run
  heavy steps (transcode, subtitles) on the stronger machine
- **Worker nodes** — distribute big batch jobs across spare machines on
  your network
- **Server-side push companion** — a small headless helper that delivers
  finished files to your media server box

---

**How this list is maintained:** items graduate Proposed → Planned → In
progress → Shipped. When something ships, its issue gets the `shipped`
label and the release notes name it. Bugs aren't tracked here — see the
[issue list](https://github.com/grandmediastation/gms-public/issues).
