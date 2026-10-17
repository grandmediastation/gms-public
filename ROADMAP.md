# Grand Media Station — Roadmap

What's coming to GMS. No dates: items ship when they're ready. Want
something moved up? **👍 its issue** (or open one): votes genuinely
reorder the Proposed list.

_Last updated: 2026-10-17._

## Shipped highlights ✅

Already in the app today:

- Smart renaming with preview, profiles, and full undo (Track Record)
- Library management: browse, organize, playlists, duplicate and quality scanning, storage insights
- **Caption Car**: on-device AI subtitle generation (nothing uploaded), with a review queue, confidence highlighting, and audio-sync tools
- Transcoding with GPU acceleration, savings analysis, and safe replace-or-keep-both output, with a profile picker that explains each profile and estimates the output size
- Media-server integration (Plex / Jellyfin) with library sync, Match Checker and Missing Episodes, and playlists pushed to one server or several
- Renaming rules for photos, music and other files, right on the Rename tab, without setting up a pipeline
- Organise files into season, show and genre folders, with preview and undo
- A confidence score on every show and film match, with a review list for the unsure ones; your own corrections are kept
- GMS notices what a show or film is missing (description, artwork, episode titles), fetches it when online, and says when it last ran
- Duplicates: the recommendation says when deleting a copy would cost a subtitle, and can save that subtitle first
- Drop unused audio and subtitle tracks from a file (Track Surgeon)
- Pipelines with per-step conditions, fallbacks and watch folders
- Photos and Home media: grouping with fold-away headers, side-by-side photo compare, hover preview, and converting photos to any size, web formats or icons
- Trash with restore, and back up and restore from Settings (local or your own cloud storage)
- Cleanup: folder names, duplicates, unreadable files, integrity, naming
- Fully offline-capable: online features are optional

## In beta 🧪

On the beta channel now, being finished:

- **Subtitle translation and multilingual generation** — Translate a subtitle into another language on your own computer, keeping every line's timing. Available now on the beta channel while it is finished. ([#24](https://github.com/grandmediastation/gms-public/issues/24))
- **Audio quality: find quiet dialogue and tune it** — GMS listens for scenes where the dialogue sits too low under the music and effects and lets you tune the track. Available now on the beta channel while it is finished. ([#25](https://github.com/grandmediastation/gms-public/issues/25))

## In progress 🚧

Being built:

- **Auto-playlists from franchises and collections** — Build playlists from franchises and collections, with a review step before anything is created. Grouping a playlist by folder and pushing it to your media servers already ships. ([#26](https://github.com/grandmediastation/gms-public/issues/26))

## Planned 📋

Next up, in no particular order:

- **Build your own file names from pieces, and see every field you can use** — On the Rename tab, assemble a name from chips: free text, the date taken, today's date, dimensions, camera, the original name, a counter, or any other field GMS knows about the file, and drag them into the order you want with a live preview. A reference page lists every field available for shows, films, photos and music, with an example value from your own library, so nobody has to type a field name from memory. ([#4](https://github.com/grandmediastation/gms-public/issues/4))
- **Find a subtitle's timing offset automatically, for many files at once** — Audio Sync already analyses one subtitle against its audio. The batch version works out the offset for every selected file, applies it when it is confident, and puts the rest in a review list with the suggested shift and a one-click preview. ([#7](https://github.com/grandmediastation/gms-public/issues/7))
- **A real search for shows and films** — Replace the single show-name box with a search that covers shows and films, shows year and artwork so you can tell two same-named titles apart, remembers recent searches, and finds a title typed in its original script, so Example Show written in Japanese or Chinese matches the same way as its English name. ([#8](https://github.com/grandmediastation/gms-public/issues/8))
- **Faster indexing over a network share, and never hogging the connection** — Indexing a large library on a network share would first list what is there, then read file details in a second pass, and cap itself below your link speed so the rest of the house keeps working. ([#11](https://github.com/grandmediastation/gms-public/issues/11))
- **Move a library root to a new path without a rescan** — When a drive letter changes or a share moves, point the library root at its new location and keep every match, Track Record entry and setting, instead of re-indexing from scratch. ([#20](https://github.com/grandmediastation/gms-public/issues/20))
- **Subtitle text check and corrector** — Before a generated subtitle is saved, the words GMS was least sure of are highlighted so you can check them; click a word to hear that moment and edit in place. For a subtitle you already have, GMS listens to the audio and highlights the words that disagree with the text, and jumps you straight to them. ([#27](https://github.com/grandmediastation/gms-public/issues/27))
- **Hand off conversions to an external transcode runner you already run** — If you already run a transcode runner on your network, let GMS hand conversion jobs to it instead of converting on this machine, and pick up the finished files. ([#29](https://github.com/grandmediastation/gms-public/issues/29))
- **Local automation API** — A local REST API and MCP server so your own tools and AI assistants can drive GMS on your machine. Nothing leaves your computer. ([#31](https://github.com/grandmediastation/gms-public/issues/31))
- **Multi-server support** — Manage libraries across more than one media server from one GMS, with each server's matches and paths kept separate. ([#32](https://github.com/grandmediastation/gms-public/issues/32))

## Proposed 💡 (vote!)

Ideas under consideration. 👍 the matching issue to push one up:

- **Sonarr and Radarr integrations** — Let GMS work alongside Sonarr and Radarr. GMS would keep a flat, one-folder-per-title layout of the files already in your library that those tools read cleanly, while GMS does the matching for files their own parsers give up on, such as dot-separated names with stray numbers in front. ([#2](https://github.com/grandmediastation/gms-public/issues/2))
- **Fix one wrong match, and fix the others that went wrong the same way** — Every match already carries a confidence score and the unsure ones sit in a review list. Next: when you correct one wrong match, GMS looks for the other files that were matched wrongly for the same reason and offers to fix them in one go, and can re-check matches on a schedule and tell you what it changed. ([#3](https://github.com/grandmediastation/gms-public/issues/3))
- **Cut ad breaks and intros out of a video** — Detect ad breaks, intros and outros across a selection as a batch job, review the detected segments on a timeline with play-from-here, adjust the edges, then cut the kept ranges together into a clean file with no re-encode, undoable like every other change. ([#5](https://github.com/grandmediastation/gms-public/issues/5))
- **Compare two subtitles side by side** — Open two subtitle files for the same video next to each other, for example an existing one and a freshly generated one, step through them cue by cue with the video, and pick the better line or the better timing into the one you keep. ([#6](https://github.com/grandmediastation/gms-public/issues/6))
- **Keep two GMS installs in sync on your home network** — Pair a desktop and a server install from one screen, and GMS keeps the library, Track Record and settings the same on both. Changes made on one appear on the other; the data travels only across your own network. ([#9](https://github.com/grandmediastation/gms-public/issues/9))
- **Choose how much of your computer GMS uses, and let it work while you are away** — A Resource limits setting (all cores, half, one, or background only) for scans, conversions and subtitle generation, and an Away mode that notices when you have stepped away and lets the heavy jobs run at full speed, dropping back when you return. ([#10](https://github.com/grandmediastation/gms-public/issues/10))
- **A visual pipeline editor and an activity feed** — Lay pipeline steps out on a canvas and connect them, instead of a top-to-bottom list, and follow every run in an activity feed where a failed run can be cancelled or retried from the step that failed. ([#12](https://github.com/grandmediastation/gms-public/issues/12))
- **Browse your library as files and folders** — A Files view that shows every file GMS has indexed, with the details it knows (codec, resolution, size, duration, music tags, camera and date for photos), with search and filters, alongside the TV, Movies and Home media views. ([#13](https://github.com/grandmediastation/gms-public/issues/13))
- **Photo health check** — Find photos that are damaged and say whether anything can be recovered: a truncated image whose top part still decodes, a damaged metadata block on an intact image, or a surviving embedded thumbnail. ([#14](https://github.com/grandmediastation/gms-public/issues/14))
- **A map of where your photos were taken** — Photos that carry location data appear on a map, clustered by place, and you can find photos by where they were taken rather than by file name or date. ([#15](https://github.com/grandmediastation/gms-public/issues/15))
- **Remove or set location and other embedded tags** — See the tags embedded in a file (location, camera, dates, author), remove any or all of them for a selection, or set a value for the files chosen right now. A set value never lingers, so it cannot stamp an old location on the next batch. Undoable from Track Record. ([#16](https://github.com/grandmediastation/gms-public/issues/16))
- **Slideshow videos from photos, and albums beside playlists** — Turn a set of photos into a slideshow video, and group photos into albums that sit next to playlists. ([#17](https://github.com/grandmediastation/gms-public/issues/17))
- **An editing queue that hands photos and videos to your editor** — Send one item or many to a review queue and work through them one at a time, the way a photographer works a shoot. Sending an item on can also move it into a folder your photo or video editor watches. ([#18](https://github.com/grandmediastation/gms-public/issues/18))
- **Silent file damage detection and an integrity catalogue** — Record a full content fingerprint for each file, re-check it on a schedule, and report any file whose bytes changed without a rename or edit, before you find out from a playback failure. ([#19](https://github.com/grandmediastation/gms-public/issues/19))
- **Find your media server automatically, and go deeper with statistics apps** — Pick your Plex, Jellyfin or Emby server from a list GMS finds on your network instead of typing an address, see at a glance whether each server is reachable, and map server paths to local paths with a guided setup. Deeper Tautulli integration, and support for its Jellyfin counterpart, would bring watch statistics into GMS. ([#21](https://github.com/grandmediastation/gms-public/issues/21))
- **Measure real video quality, not just the label** — A deep scan that samples a few seconds of each file to measure how good it actually looks, so a file that says 1080p but was encoded badly is ranked honestly in duplicate and quality decisions. ([#22](https://github.com/grandmediastation/gms-public/issues/22))
- **GMS in your language** — An interface language picker, with renaming that handles the small words and the East Asian name variants of each language correctly. ([#23](https://github.com/grandmediastation/gms-public/issues/23))
- **Identify a mislabelled episode from what is said in it** — Match the dialogue in a subtitle against episode descriptions to confirm a file really is the episode its name claims. ([#28](https://github.com/grandmediastation/gms-public/issues/28))
- **Multi-version awareness** — First-class handling of several cuts or qualities of the same title, so they are grouped as versions rather than flagged as duplicates. ([#30](https://github.com/grandmediastation/gms-public/issues/30))
- **Cross-device pipelines** — Pair two of your GMS installs and run heavy steps such as conversion and subtitle generation on the stronger machine. ([#33](https://github.com/grandmediastation/gms-public/issues/33))
- **Worker nodes** — Distribute big batch jobs across spare machines on your own network. ([#34](https://github.com/grandmediastation/gms-public/issues/34))
- **Server-side push companion** — A small headless helper that runs next to your media server and applies the fixes GMS decided on, so the desktop app does not have to stay open. ([#35](https://github.com/grandmediastation/gms-public/issues/35))

---

**How this list is maintained:** items graduate Proposed → Planned → In
progress → In beta → Shipped. When something ships, its issue gets the
`shipped` label and the release notes name it. Bugs are not tracked here;
see the [issue list](https://github.com/grandmediastation/gms-public/issues).
