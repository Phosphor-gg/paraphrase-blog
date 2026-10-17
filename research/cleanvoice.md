# Cleanvoice: the facts posts may state

Every fact below was read on Cleanvoice's own pages on 17 October 2026
(read 2026-10-17). Pages were fetched as raw HTML and read directly, including
the structured plan data embedded in the pricing page. Anything marked
**UNVERIFIED** must not be stated in a post.

Re-verified 2026-10-17 by a second pass: every cited page re-fetched and each
quote matched; the pricing page was also rendered in headless Chromium with
the Yearly and EUR toggles clicked. The help centre (help.cleanvoice.ai) did
render in headless Chromium on the second pass, and the articles cited below
as help.cleanvoice.ai were read then.

## What it is

- An AI audio clean-up and editing service for spoken word, used in the
  browser ("Cleanvoice runs in your browser on desktop and mobile, so there's
  nothing to download").
  https://cleanvoice.ai/remove-background-noise/ (FAQ "Is Cleanvoice
  web-based?"), read 2026-10-17
- Describes itself as following "Clean, then Enhance, then Edit".
  https://cleanvoice.ai/llms.txt, read 2026-10-17
- Not transcript-driven. Homepage FAQ, verbatim: "No, unlike other AI podcast
  editors, Cleanvoice doesn't work based on the transcript-to-edit flow. You
  only need to upload your files and we will transcribe video or audio
  automatically." https://cleanvoice.ai/ (FAQ), read 2026-10-17
- Help centre, verbatim: "No. We don't work on text or transcription-based
  editing. That means, our AI directly detects unwanted fillers, stutters,
  mouth sounds, etc. from your file and automatically removes them." (Question:
  "Do You Use Transcription of My Audio or Video or Allow Keywords to Edit My
  File?")
  https://help.cleanvoice.ai/en/articles/66-do-you-edit-audio-and-video-based-on-transcription,
  read 2026-10-17
- Note for posts: Cleanvoice is not transcript-*driven*, but it does produce
  transcripts (see "Also included"). Do not say it has no transcript.
- Filler detection is acoustic: "Detection works on how speech sounds, not on
  text, so it also copes with accents and with languages that sound similar."
  https://cleanvoice.ai/filler-words/ (FAQ), read 2026-10-17
- Has a REST API with official Python and JavaScript SDKs, plus Make.com and
  n8n integrations. https://cleanvoice.ai/llms.txt and
  https://docs.cleanvoice.ai/llms.txt, read 2026-10-17

## What it removes or changes (the "Edit" side)

- **Filler words** (um, uh, er, ah and equivalents in other languages). "Our AI
  identifies the context of the audio and adds silence (room noise) to make the
  flow of the podcast more natural." https://cleanvoice.ai/filler-words/,
  read 2026-10-17. The API docs describe `fillers` as removing "um", "uh",
  "like", etc. https://docs.cleanvoice.ai/llms.txt, read 2026-10-17
- **Stutters**: "We first try to identify the stutter. Once we identify it, we
  try to edit out the stutter without cutting the word out."
  https://cleanvoice.ai/stutter-remover/ (FAQ), read 2026-10-17. The same
  page's meta description says "Remove stutters and repeated words"; the API
  docs describe `stutters` as "remove repeated word fragments".
- **Repeated words: conflicting.** The help centre says: "Do You Remove
  Repetitive Words? Currently, we can detect repetitive words. But the feature
  is yet to go live."
  https://help.cleanvoice.ai/en/articles/64-what-type-of-filler-words-can-you-remove,
  read 2026-10-17. Posts must not claim either way whether Cleanvoice removes
  repeated words. Nothing read describes cutting false starts, hedges, or the
  same point made twice in different words; posts may say only that its pages
  do not describe that, not that it cannot.
- **Hesitations**: API option `hesitations`, "remove short hesitation sounds
  that aren't full filler words". https://docs.cleanvoice.ai/llms.txt,
  read 2026-10-17
- **Mouth sounds**: "Lip smacks, saliva crackle, mouth clicks and the harsh
  part of breaths." Caveat on their page: "Some clicks sit inside words, where
  removing them could damage the word, so a few soft ones may remain. Listen
  back before you publish." https://cleanvoice.ai/mouth-sounds/ (FAQ),
  read 2026-10-17
- **Breaths**: separate breath remover, mute or reduce.
  https://cleanvoice.ai/breath-remover/, read 2026-10-17. API modes true,
  "legacy", "natural". https://docs.cleanvoice.ai/llms.txt, read 2026-10-17
- **Long silences / dead air**: shortened based on context ("When the speaker
  is thinking, the pause gets shorter. When the speaker changes topic, a longer
  pause stays.") https://cleanvoice.ai/deadair-remover/, read 2026-10-17
- **Mute instead of cut** ("Preserve Length", API `muted`) so a video or other
  timeline stays in sync. https://cleanvoice.ai/filler-words/ (FAQ) and
  https://cleanvoice.ai/ (FAQ "Can I mute edits instead of removing them?"),
  read 2026-10-17
- Other "What should I watch out for?" FAQs: background noise, "If a voice is
  buried under very loud noise, some artifacts can remain, so preview the
  result before you publish" (https://cleanvoice.ai/remove-background-noise/);
  dead air, "Removing every pause makes speech sound rushed ... Listen back
  before you publish" (https://cleanvoice.ai/deadair-remover/); breaths,
  "removing breaths can make the delivery feel rushed. Listen back before you
  publish" (https://cleanvoice.ai/breath-remover/). All read 2026-10-17.
- Their own caution: "Not every um has to go. Removing all of them can make
  speech sound clipped, so listen back before you publish."
  https://cleanvoice.ai/filler-words/ (FAQ), read 2026-10-17

## Audio processing (the "Clean" and "Enhance" side)

- **Background noise**: "Steady noise such as hum, hiss, buzz, fans and air
  conditioning, and changing noise such as wind, traffic, cafés, audience
  chatter, kids and neighbours. It also removes mic noise and mouse clicks."
  Clean Audio also "removes the noise and balances loudness" and "removes room
  reverb". Optional Keep Music. https://cleanvoice.ai/remove-background-noise/
  (FAQ), read 2026-10-17
- **Audio enhancer / Studio Sound**: background noise, distortion, echo and
  reverb, equalisation, level/volume. https://cleanvoice.ai/audio-enhancer/,
  read 2026-10-17
- **Echo and reverb remover**, listed. https://cleanvoice.ai/llms.txt,
  read 2026-10-17
- **Loudness normalisation**, default target -16 LUFS in the API.
  https://docs.cleanvoice.ai/llms.txt, read 2026-10-17

## Also included

- **Transcription** in 99 languages (API: Whisper), exportable as .srt for
  subtitles. https://cleanvoice.ai/podcast-transcript/ (FAQ) and
  https://docs.cleanvoice.ai/llms.txt, read 2026-10-17
- **Summaries, show notes, chapters with timestamps, social media posts,
  titles/keywords.** https://cleanvoice.ai/podcast-summarization/,
  read 2026-10-17
- **Video**: cleans the audio of a video; supports mp4, AVI, WebM, MOV.
  Does not burn in subtitles. https://cleanvoice.ai/video-podcast-editing/
  (FAQ), read 2026-10-17
- **Multitrack**: up to 5 tracks, edited together in sync ("You can upload up
  to 5 tracks, for example one per speaker"; stutter FAQ: "You can upload up
  to 5 audio tracks. If you require more tracks, just write us").
  https://cleanvoice.ai/filler-words/ and https://cleanvoice.ai/stutter-remover/
  (FAQ), read 2026-10-17
- **Batch upload**: "You can upload more than one podcast episode
  simultaneously." https://cleanvoice.ai/ (FAQ), read 2026-10-17
- **Templates**: pick a default or custom template choosing which edits to
  apply. https://cleanvoice.ai/ (FAQ "Can I choose what edits I want to
  apply?"), read 2026-10-17
- Free browser tools (trimmer, volume changer, joiner, mic test, audiogram,
  etc.). https://cleanvoice.ai/llms.txt, read 2026-10-17

## Languages

- Filler-word removal: "20+ languages, including English, German, Romanian,
  French, Dutch, Spanish, Italian, Portuguese, Polish, Arabic, Turkish and
  Bulgarian." https://cleanvoice.ai/filler-words/ (FAQ), read 2026-10-17
- Noise, silences, normalisation, mouth sounds, breathing and stutters are
  "language-agnostic". https://docs.cleanvoice.ai/llms.txt, read 2026-10-17
- Transcription: 99 languages. https://cleanvoice.ai/podcast-transcript/,
  read 2026-10-17

## Reviewing edits: what you get back

- The core flow is upload, process, download: "Upload your audio or video
  file to Cleanvoice, turn on filler-word removal and start. The AI finds and
  cuts the fillers, and you download the edited file within minutes."
  https://cleanvoice.ai/filler-words/ (FAQ), read 2026-10-17
- After processing, per Cleanvoice's own blog (published 2026-02-15, modified
  2026-03-25): "a report dashboard shows: Number of filler words, stutters,
  breaths, and dead air removed; Playback preview and toggle to compare
  original vs. edited recording", then Download Audio or Export Options for
  Audacity, Adobe Audition or Reaper.
  https://cleanvoice.ai/blog/how-to-edit-voice-recording/, read 2026-10-17
- Help centre detail of the review screen: "you can see the number of filler
  words, breaths, stutters, and mouth sounds removed. You can also note the
  seconds of deadair removed"; a waveform with a toggle to enable or disable
  Cleanvoice's edited version, zoom 1x to 3x, unwanted sounds highlighted in
  red. Also reachable later from the History page (while files are stored).
  https://help.cleanvoice.ai/en/articles/87-can-i-review-what-was-edited-from-my-audiovideo,
  read 2026-10-17
- Help centre: "No, you cannot choose the time period on which you can apply
  edits ... Though we do not support time-based editing options, you can
  export the timelines or markers of your edited file to other editing tools.
  You can then modify your edits in such editors easily."
  https://help.cleanvoice.ai/en/articles/61-can-i-cut-some-specific-seconds-to-not-apply-editing-on-it,
  read 2026-10-17
- To change edits, export them: "Either you can export the timestamps or
  markers of edited parts. You can export them to your preferred editing tools
  like Audacity, Audition, Reaper, etc. And edit and customize manually."
  https://cleanvoice.ai/ (FAQ "What if I want to change the edits?"),
  read 2026-10-17
- Supported editors: "Adobe Audition, Adobe Premiere, Davinci Resolve, Reaper
  and Audacity. And also anything which supports .EDL". Markers show where it
  edited (load onto the cleaned audio); Timestamps show what it would edit
  (load onto the raw audio and delete manually). "we mark the filler words,
  stutters and mouth sounds in the timestamp. We don't highlight deadair in the
  timestamp". https://cleanvoice.ai/integrations/ (FAQ), read 2026-10-17.
  The help centre's export article lists fewer editors ("Currently, we provide
  export options for Audacity, Audition, and Reaper").
  https://help.cleanvoice.ai/en/articles/48-how-can-i-export-edits-instead-of-downloading-the-file,
  read 2026-10-17. Posts naming editors should follow the integrations page
  and not imply every editor is a one-click export.
- **UNVERIFIED, do not state:** whether Cleanvoice's web app lets you undo or
  restore an individual edit inside the app. No page says so explicitly either
  way. The help centre (which did render on the second pass) says you cannot
  choose time ranges to apply or skip edits and points to the timeline/marker
  export for modifying edits (article 61 above), which is consistent with no
  per-edit restore but does not state it. A third-party listing claimed a
  "timeline editor" for approving suggestions; not used. Posts may say that
  the documented route for changing individual edits is the export, that the
  help centre says time-based editing is not supported, and that we have not
  used the app hands-on.

## Formats, files and data

- Input: "Most audio and video formats, including WAV, MP3, M4A, FLAC, OGG,
  AAC, MP4, MOV and WebM. There's no length limit. With an account, files can
  be up to 3 GB each, or 8 GB in total for a multitrack upload."
  https://cleanvoice.ai/mouth-sounds/ (FAQ), read 2026-10-17
- Audio output formats (API): mp3, wav, flac, m4a, opus, aac; video jobs keep
  the original container. https://docs.cleanvoice.ai/llms.txt, read 2026-10-17
- Retention: "We store both your original and edited files for 7 days. After
  7 days, we remove your files permanently." https://cleanvoice.ai/pricing/
  (FAQ); feature page FAQs word it "We store your original and edited files
  for 7 days. After that, we delete them permanently." Read 2026-10-17
- Reprocessing is charged again: "Each audio processing run is billed
  separately. If you choose to reprocess your file, it will count as a new
  edit and incur an additional charge." (Support may give a credit if you are
  unhappy with a result.)
  https://help.cleanvoice.ai/en/articles/103-can-i-reprocess-my-audio-without-being-charged-again,
  read 2026-10-17
- "GDPR compliant", "Data stored in the EU", "ISO 27001 certified".
  https://cleanvoice.ai/, read 2026-10-17

## Pricing (https://cleanvoice.ai/pricing/, read 2026-10-17)

The page has an EUR / USD toggle (the server-rendered default is USD). Prices
"are listed without VAT"; "Sales tax or VAT may be charged, depending on where
you live. Companies from Europe can use their VAT ID (UID number) to purchase
without VAT." Sales run through Paddle ("all major Credit Cards, PayPal &
Apple Pay"). Every plan, including the free trial, includes "all features".
The rendered price cards show no "/month" or "/year" suffix; the period
follows from the Monthly/Yearly toggle and the per-hour figure (e.g. yearly
$110 at $0.92/hour = 120 hours).

**Free trial:** "30 minutes Processed Audio for Free", "No credit card
required". Homepage FAQ: "You get an additional 30 minutes of free credits
once you sign up." https://cleanvoice.ai/ (FAQ), read 2026-10-17. The word
"additional" is ambiguous; the help centre says "you get 30 minutes of free
credits when you sign up", with "no expiration date for these credits", and
no card needed.
https://help.cleanvoice.ai/en/articles/5-do-i-get-free-credits-to-try-cleanvoice
and .../26-what-is-the-difference-between-guest-upload-and-free-credits, read
2026-10-17. State 30 minutes; never add them up to 60.
**Guest upload** (no sign-up): homepage "Try without sign-up. No credit card
required." Help centre: guest audio over 30 minutes or video over 10 minutes
is trimmed, you review a section, and you must sign up to download full
results; batch upload and custom templates are not available to guests.
llms.txt: 1.5 GB file limit for guests. Same help articles, read 2026-10-17.

**Pay as you go** (one-off credits, "Credits purchased are valid for 2 years";
help centre: "valid for 2 years (from the purchase)"; the plan data also lists
"Unused credits roll over" as a feature of each pack). Page quirk: the rendered
pack cards say "Processed Audio per Month." although these are one-off packs.

| Hours | USD | EUR | USD per hour | EUR per hour |
| --- | --- | --- | --- | --- |
| 5 | $11 | €10 | $2.20 | €2 |
| 10 | $20 | €18 | $2.00 | €1.80 |
| 30 | $45 | €40 | $1.50 | €1.33 |

**Subscription** (hours per month):

| Hours a month | Monthly USD | Monthly EUR | Yearly USD | Yearly EUR |
| --- | --- | --- | --- | --- |
| 10 | $11 | €10 | $110 | €100 |
| 30 | $28 | €26 | $300 | €260 |
| 100 | $90 | €85 | $900 | €850 |

Per-hour figures shown on the page (rendered and in the plan data):
monthly $1.10 / $0.93 / $0.90 and €1 / €0.87 / €0.85; yearly $0.92 / $0.83 /
$0.75 and €0.83 / €0.72 / €0.71. (Corrected on re-check: the earlier note
said the 100h yearly figure was not shown and the EUR monthly figures were
implied; both are shown.)

**Custom plan:** "Starting at $0.01 / minute", "200+ Hours Processed Audio",
custom API endpoints, priority support, "Custom Pricing and Billing"; "Need
200+ hours per month?"; book a call.

**Credit rules (pricing FAQ):**
- Unused subscription credits roll over, "up to 3 × your monthly credit
  budget" (example on the page: on the 10h plan "you get 10h credits each
  month and on top of that you can roll over up to 30h credits from previous
  months"). Plan card: "Credits are usable anytime within the subscription
  period. Unused credits roll over, up to three times your plan limit." Help
  centre adds "(If you stay subscribed)".
  https://help.cleanvoice.ai/en/articles/15-what-happens-to-my-unused-credits-do-they-get-carried-forward
- Subscription credits are used first, then pay-as-you-go credits.
- "Billing is based on the duration of the audio files, the minimum processing
  time for billing is 1min. We round credit upwards. If you process a 10min
  20sec audio file, we bill 11 minutes."
- Multitrack: "we currently don't charge extra, however in the future, this
  will change."
- Cancel, upgrade or downgrade any time; on cancellation unused subscription
  credits last until the end of the billing period.
- Failed uploads are not charged ("you will not be charged if the uploads
  fails").
- Startup programme: up to 200 hours of free API credit on application.

**UNVERIFIED, do not state:** llms.txt says "A 200-hour pay-as-you-go pack is
€180"; no such pack appears on the pricing page read the same day. Not used.

## Other tools (for the alternatives post), read 2026-10-17

Only these, from each tool's own homepage. No prices were read for any of them;
posts must not state prices for them.

- **Descript** (https://www.descript.com/): "AI Video & Audio Text-based
  Editor". Features listed include Remove Filler Words, Studio Sound, Remove
  Retakes, Edit for Clarity, Captions, Translation, Rooms (remote recording),
  and "AI speech: Easily create a realistic voice clone or pick from our stock
  AI voices". Free to start ("Get started for free").
- **Riverside** (https://riverside.com/): record "up to 4K video and
  uncompressed audio in separate tracks", "text-based editor", AI audio that
  "removes noise", Magic Clips, captions, live streaming, hosting. "Free plan
  available."
- **Podcastle**: https://podcastle.ai/ redirected to https://async.com/ on
  2026-10-17, branded **Async**. Its page lists removing "filler, pauses,
  repeats, bad takes", Clean Audio "Remove background noise" (Magic Dust),
  generated voice and music, captions and clips, and says "AI can make
  mistakes. Please review all edits." Re-read 2026-10-17: "Formerly
  Podcastle"; Video Editor "Tell Async what to cut, pace, or polish"; Audio
  Editor "Edit your episode by editing the transcript, like a doc"; Recording
  Studio "Record remote guests in 4K".
- **CapCut** (https://www.capcut.com/): video editor (desktop, online,
  mobile) with Reduce noise, Enhance voice, Auto captions and Text to speech
  among its listed tools. "Try online for free".
- **Audacity** (https://www.audacityteam.org/): "Free, Open Source Audio
  Editor and Recorder", runs on Windows, macOS and Linux, supports third-party
  plugins. It also has a built-in Noise Reduction effect (Effect > Noise
  Reduction; "Eliminate hiss, hum, fan noise, and buzzing").
  https://www.audacityteam.org/features/noise-reduction/, read 2026-10-17
- Riverside re-read 2026-10-17: "Capture up to 4K video and uncompressed audio
  in separate tracks, unaffected by internet connection."
  https://riverside.com/
