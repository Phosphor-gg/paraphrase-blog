# Paraphrase: the facts posts may state

Checked against the code (paraphrase-backend, paraphrase-types,
paraphrase-website, paraphrase-audio-api) and the live Stripe account on
17 October 2026. Anything not here is not to be claimed until it is checked
and added.

## What it is

- A web app at https://paraphrase.bot. Runs in the browser; no desktop or
  mobile app.
- Made by Phosphor Technologies, a sole proprietor in the United Kingdom
  (also makes Supervisor, supervisor.gg).
- You record or upload into a **project**. Each recording (a **take**) is
  transcribed with a timestamp on every word. Every edit is a choice of which
  of your words stay and in what order. The export is **your original
  recording with pieces cut out**, cut at word boundaries and joined back up.
- **It never generates speech.** No voice cloning, no overdub, no text to
  speech, no regenerated words. A word you never said cannot appear in an
  export because there is no audio for it. This is a design decision, not a
  missing feature, and is the main point of difference from Descript-style
  tools that offer AI voices.

## Getting audio in

- Record in the browser. The recorder hands over a piece about every second
  and the take is uploaded while you record (paraphrase-website
  services/media.rs, CHUNK_MS = 1000), so losing the connection or closing
  the tab does not lose what was already sent.
- Upload an audio or video file (the browser accepts `audio/*` and `video/*`;
  the server reads it with ffmpeg, so most formats work).
- For a video, the sound is taken out in the browser and uploaded on its own;
  the picture is only uploaded if you export MP4.
- Paste a link to audio or video; the file is fetched server side.
- A project holds as many takes as you want, edited as one transcript.
- One recording can be from 0.5 seconds to 4 hours long.

## Transcription

- Model: NVIDIA Parakeet TDT 0.6B v3, run on Paraphrase's own GPUs.
- 25 European languages, detected automatically: Bulgarian, Croatian, Czech,
  Danish, Dutch, English, Estonian, Finnish, French, German, Greek, Hungarian,
  Italian, Latvian, Lithuanian, Maltese, Polish, Portuguese, Romanian,
  Russian, Slovak, Slovenian, Spanish, Swedish, Ukrainian.
- No speaker labels (diarisation), no translation, no subtitles or captions.

## Editing

- Click a word to cut it; click again to restore it. Cut words stay on screen,
  struck through.
- Shift-click to cut a run of words.
- Drag a word to move it (reorder); keyboard: focus a word, Shift + left or
  right arrow; touch: press and hold, then drag.
- Undo and redo (Ctrl+Z, Ctrl+Shift+Z; Cmd on a Mac).
- Saves as you go. Non-destructive: the original recording is never changed.

## Clean up with AI

- One button. A language model reads the transcript and proposes the cut:
  filled pauses (um, uh), false starts, hedges, repetition (including the same
  point made twice in different words), and can move words where a sentence
  reads better.
- No word list; it judges each word in context and keeps anything that
  carries meaning.
- It is a proposal: cuts show struck through and any word can be put back.
- Runs on machines Paraphrase operates; the transcript is not sent to a
  third-party model.
- Tested on English speech. Do not claim cleanup quality for other languages.
- Limits: 3 cleanups a day on the free plan, 30 a day on Premium, resetting at
  midnight UTC. A cleanup that fails is not counted.

## Exporting

- WAV, FLAC, MP3, M4A (AAC), Opus. WAV and FLAC are lossless, so a cut of a
  lossless master stays lossless.
- MP4 video when the project has a video take, with picture and sound cut at
  the same words. An audio-only take shows as black in an MP4 export.
- Re-exporting and re-editing cost nothing.
- No watermark on any export, on either plan: the backend's export path
  (paraphrase-backend media_service, project_edit_service) has no overlay,
  drawtext or watermark step; checked 17 October 2026.

## Not offered (do not imply otherwise)

- AI voice, voice cloning, overdub, text to speech.
- Noise removal, speech enhancement, levelling, EQ, music or sound effects.
- Remote recording studio, multitrack or separate per-speaker tracks.
- Speaker labels, captions, subtitles, translation.
- Collaboration, comments, share links.
- Screen recording.
- Podcast hosting or publishing to podcast directories.
- Summaries, show notes, chapters or any other generated text about the
  recording.
- A public API (exists internally, not offered).

## Pricing (live Stripe, checked 17 October 2026)

- **Credits:** one credit transcribes one second of audio. One model, no
  multiplier. Credits are spent once, at transcription. Editing, cleanup and
  export do not use credits.
- **Free plan:** every new account gets 15 minutes of transcription
  (900 credits), no card. 3 AI cleanups a day. Projects up to 5 minutes of
  recordings in total.
- **Premium:** £13.99 a month, £83.85 a year (about £6.99 a month) or £179.65
  for three years (about £4.99 a month). Includes 120 hours of audio a month
  (resets each billing period, does not roll over), 30 AI cleanups a day,
  projects up to 4 hours.
- **Free trial:** 7 days of Premium on the monthly or annual cycle (not the
  three year one), card required, one per account.
- **Credit packs** (either plan, never expire while the account is open):
  £3.99 for 4 hours, £12.99 for 13 hours 20 minutes, £34.99 for 40 hours.
- If a recording fails for a reason on Paraphrase's side, its credits are
  returned automatically (recording_service::refund_if_ours). A file that
  cannot be read at all is not refunded. Do not say "failed recordings are
  refunded" without that qualifier.
- Prices in GBP.

## Privacy

- Nothing submitted is used to train any model, Paraphrase's or anyone else's;
  not sold or licensed.
- The original recording is kept while it is in your account (that is what
  makes re-editing free); deleting a recording deletes it. Deleting a
  project, or the whole account, deletes every recording's files too
  (fixed 17 October 2026: account deletion used to leave the files).

## Pages to link

- `/pricing`, `/docs`, `/docs/getting-started`, `/docs/editing`,
  `/docs/ai-cleanup`, `/docs/exporting`, `/docs/credits-and-plans`,
  `/docs/your-data`
- Use cases: `/podcast-editing`, `/video-editing`, `/voiceover-editing`,
  `/interview-editing`, `/course-editing`, `/short-form-video`
- Sign up: https://paraphrase.bot (a free account, no card)
