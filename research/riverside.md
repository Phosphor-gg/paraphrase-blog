# Riverside: facts posts may state

Every fact below was read on Riverside's own pages on 17 October 2026 (written
"read 2026-10-17"). Help centre articles were read through the help centre's
public article API (`support.riverside.com/api/v2/help_center/en-us/articles/<id>.json`)
because the HTML pages returned 403 to automated fetches; the content is the
same article body the linked page shows. Each article showed "updated
2026-10-15" or "2026-10-16" unless noted.

Anything under "Unverified or contradictory" must not be stated as fact.

Re-verified 2026-10-17 (fact-check pass): every help centre article below was
re-read through the API; the pricing page was re-read both as raw HTML and
**rendered in headless Chromium**, which matters because the prices are filled
in by JavaScript. Corrections from that pass are folded in below.

## Pricing page

Source: https://riverside.com/pricing (read 2026-10-17; HTML comment says
"Last Published: Fri Oct 16 2026").

**How the page gets its prices.** The served HTML contains fallback dollar
figures, and a script then loads the visitor's prices from Riverside's API
(`https://riverside.com/api/v4/pricing/plans` answered
`{"currency":"gbp","countryCode":"GB"}` for us;
`https://riverside.com/api/v1/plans/pricing` returns the plan prices). The
earlier version of this file was written from the unrendered HTML and quoted
the fallback dollar figures; those are not what a visitor sees.

### Prices as rendered for a UK visitor (read 2026-10-17)

| Plan | Monthly billing | Yearly billing |
| --- | --- | --- |
| Free | £0 | n/a |
| Pro | £35 a month | £24 a month, "Billed £288 annually" |
| Grow | £45 a month | £34 a month, "Billed £408 annually" |
| Webinar | £99 a month | £79 a month, "Billed £948 annually" |
| Business | "Contact Sales" | "Contact Sales" |

- The pricing API returns the same numbers (Pro month 35, year 24; Grow
  month 45, year 34; Webinar month 99, year 79) under its `usd`, `eur` and
  `gbp` keys alike. We only saw the page render in pounds; we did not see it
  render for a US or EU visitor.
- The page's FAQ text (static, not localised) still says: "Annual billing
  saves you up to 20% - Pro drops from $29 to $24/month, Grow from $39 to
  $34, and Webinar from $99 to $79." The banner says "Up to 20% off Yearly
  plans". Neither matches £35 to £24. See "Unverified or contradictory".
- Pro, Grow and Webinar cards: "Start 14-day free trial". Business: "Book a
  demo".

### Free plan (pricing page wording)

- "Try 2 hours of multi-track recordings (Separate audio and video tracks)".
  The phrase "2 hours (one-off)" appears only in the page's unrendered
  fallback comparison table, not on the rendered page; see Unverified.
- "Full suite of editing tools".
- "Up to 720p video quality", "44.1 kHz audio quality".
- "Riverside watermark on all your things".
- "Unlimited single track recording and editing".
- "Magic Clips".
- "Video calls. As long as you want!"

### Pro

- "Up to 4K video", "48kHz audio", "No watermark".
- "Teleprompter for host", "In-person multi-cam recording".
- "Unlimited text-based editing", "AI editing & repurposing agent",
  "AI B-roll, eye contact, remove silences & filler words",
  "Unlimited transcriptions", "Magic clips & show notes", "Audio enhancement".
- "Podcast hosting & analytics", "Publish to YouTube, Spotify, Apple,
  Instagram, LinkedIn & more".
- "1 studio", "15 hrs of separate track downloads".

### Grow (everything in Pro, plus)

- Social media scheduling, newsletter, creator website, podcast hosting for 2
  shows, publish video to Apple Podcasts, video hosting, AI thumbnails,
  Riverside MCP, custom studio links.
- "Full HD 1080p live streaming", multistream to unlimited destinations,
  custom RTMP, multi-aspect ratio streaming, Omnichat, saved scenes, backstage
  speaker management.
- "2 studios", "20 hrs of separate track downloads".

### Webinar (everything in Grow, plus)

- Webinars with up to 100 registrants, pre-record and stream as live,
  recurring webinars, lead capture, registration forms, embeds, email
  reminders, Q&A, polls, webinar analytics, HubSpot integration.
- "3 studios", "25 hrs of separate track downloads".

### Business (everything in Webinar, plus)

- Unlimited studios, "Unlimited separate track downloads", up to 10,000
  webinar registrants, unlimited video storage, custom branding, async
  recording, producer mode, teleprompter for host and guests, custom frame
  rates, production workspaces and custom roles, "Collaborative editing",
  "Non-destructive timeline exports", video enhancement, API access, SSO,
  SOC2 and ISO27001, "Dedicated CSM" (the page does not expand CSM).

### Rendered comparison table (read 2026-10-17)

- Shown as tabs with per-plan detail. The block with "1 studio" (Pro) lists
  "Separate audio & video tracks downloads: 15 hours/month", "Clips export
  quality: Up to 4K", "Transcription hours: Unlimited", "Supported
  transcription languages: 100+", "Filler word removal" and "AI Voice:
  text-to-speech" ticked. The "2 studios" block (Grow) lists 20 hours/month;
  Business lists Unlimited. The tab price headers rendered as "$0 /month"
  (broken), so prices are taken from the plan cards only.

### Pricing page FAQ

- Separate track downloads: "(15 hrs on Pro, 20 on Grow, 25 on Webinar)
  refer to downloading individual audio/video tracks per participant - the
  studio-quality files. Recording itself is unlimited. If you hit the cap,
  you can still access your content but won't be able to download new
  separate tracks until the next billing cycle or if you upgrade."
- Editors: "On Pro, Grow, and Webinar, an additional editor seat is available
  as an add-on. Business is the only plan with collaborative editing and
  custom roles built in."
- AI Credits: "Al Credits power select features like Al Translation, Al
  B-Roll, and Animated Clips. Pro users start with 2000 free credits;
  Business starts with 12000. Once credits are used, you can purchase more.
  Core Al features like Magic Clips, Magic Audio, and the Al Co-Creator don't
  require credits."
- Studio: "Pro gives you 1 studio, Grow gives you 2, Webinar gives you 3, and
  Business gives you unlimited."

## Help centre

### Currency

https://support.riverside.com/hc/en-us/articles/31732683630621 (read
2026-10-17): "Riverside accepts payments in US Dollars (USD), Euros (EUR), and
British Pounds (GBP)." "We adjust pricing by region to account for factors
like local taxes, currency exchange rates, and processing costs." The GBP
prices above are what the pricing page rendered for us in the UK.

### Free trial

https://support.riverside.com/hc/en-us/articles/22576984609949-Can-I-try-Riverside-for-free
(read 2026-10-17): "Start a free 14-day trial of any Riverside plan. You'll
need a credit card to begin, but you won't be charged until the trial ends,
and you can cancel anytime."

### Separate tracks and local recording

- https://support.riverside.com/hc/en-us/articles/5260432295581-Download-high-quality-tracks
  (read 2026-10-17): "High-quality tracks are recorded locally on each
  participant's computer or device. Slow internet should not affect their
  quality." Formats offered: raw video, aligned video, raw audio, compressed
  audio.
- https://support.riverside.com/hc/en-us/articles/5260131045917-Video-and-audio-file-formats-Overview
  (read 2026-10-17): each session creates high-quality tracks (recorded
  locally), edits and clips, and cloud recording tracks. Raw tracks are MP4
  or WAV; compressed audio track MP3; Magic Audio track WAV; editor exports
  are "MP4, WAV, or MP3".
- https://support.riverside.com/hc/en-us/articles/22296539458973-About-download-hours
  (read 2026-10-17): download hours are "hours of high-quality individual
  tracks you have available to download per month". Regardless of plan you
  always have "Unlimited Recording Time", "Unlimited Editing" and "Unlimited
  exports of high-quality recordings and clips ... (just not the separate
  tracks!)". "Your monthly allowance for separate track downloads resets each
  month"; unused hours do not roll over; "The number of participants in the
  recording does not impact how many hours are used". Also: "Live streaming
  does count towards your download hours." The same article says the option
  disappears "once you have recorded over 15 hours", i.e. it is counted
  against hours recorded, not hours downloaded (see Unverified).

### Text-based editing and transcription

- https://support.riverside.com/hc/en-us/articles/14488573075741-Remove-a-word-or-phrase-from-the-recording
  (read 2026-10-17): "Riverside's text-based editing lets you make precise
  edits and trim your recording using the transcription". Plan: "All plans".
  Click a word or drag to select, press Delete or Backspace. Removed text is
  "shown in gray with a strikethrough". With overlapping speakers it asks
  which speaker to remove. Words can also be muted rather than cut.
- https://support.riverside.com/hc/en-us/articles/16673658517277-Riverside-editor-Overview
  (read 2026-10-17): editor includes timeline trimming and splitting,
  transitions, per-track volume, "Copy and paste text to move or duplicate
  media content" ("Rearrange the recording with the transcript"), remove
  crosstalk, rename a participant, captions and caption presets, comments,
  VideoDub, Magic Audio, smart mute, eye contact, enhance video, colour
  correction, aspect ratio and layouts, music and sound effects library,
  motion graphics, export of edited timeline to Premiere Pro, Final Cut Pro
  or AAF, normalise audio, remove background noise, version history, "Share
  an edit for review and comments" ("Anyone can review and leave comments
  using a link").
- https://support.riverside.com/hc/en-us/articles/9173731506589-Which-languages-can-Riverside-transcribe
  (read 2026-10-17, article updated 2026-01-24): transcribes "dozens of
  languages"; the list has 97 entries (counted 2026-10-17) including English,
  Spanish, French, Arabic, German, Chinese, Japanese, Hindi, Welsh, Yoruba.
  The rendered pricing comparison table says "100+". "Around 100" is safe.
- https://support.riverside.com/hc/en-us/articles/17525247619229-Are-transcriptions-organized-by-speaker
  (read 2026-10-17): "Riverside labels each speaker with the display name they
  use in the Studio." Not if two people share one audio input.

### Filler words, pauses, Find Fluff

- https://support.riverside.com/hc/en-us/articles/13364581561245-Remove-filler-words
  (read 2026-10-17): Plan: "All plans". Riverside "detects filler words and
  highlights them in the transcript, so you can listen to each one in context
  and decide whether to remove it or keep it. You can also remove them all at
  once." Filler types: filler words ("um," "uh," and "hmm"), contextual
  fillers ("like," "you know," "I mean," "flagged only when used as a
  filler"), noises (breaths), screen share and media, "Harsh cuts" (fillers
  that may clip nearby words). Accept or discard per card, "Remove all",
  "Restore all", restore single words. "Some filler words may not be
  recognized by the system as such."
- https://support.riverside.com/hc/en-us/articles/13993078729245-Remove-pauses-and-silences
  (read 2026-10-17): Plan: "All plans". One click, slider for "the amount of
  pauses included", "Revert to original".
- https://support.riverside.com/hc/en-us/articles/24643949984157-Apply-AI-suggestions-with-Find-fluff
  (read 2026-10-17): Plan: "All paid plans". Co-Creator "automatically
  reviews your recording and adds comments suggesting segments to remove,
  like redundant takes, chatter, and technical discussions"; it runs "When a
  new edit loads" or from AI tools; Apply or Discard each. "Non-business
  users cannot invite others to collaborate directly within Riverside". "Co-Creator comments are supported in
  all languages. Suggested cuts are explained in English."

### AI voice, voice clone, VideoDub, AI Twin

- https://support.riverside.com/hc/en-us/articles/18251355319325-Convert-text-to-speech-with-AI-Voice
  (read 2026-10-17): "Use text to generate an audio sample that simulates
  your speaking voice." Plan: Pro, Grow, Webinar and Business. Up to 2,000
  characters per generation, "up to 5,000 total characters a month", "only
  ... with your own, authenticated voice". "AI Voice is experimental".
- https://support.riverside.com/hc/en-us/articles/38619450422685-Create-your-AI-voice-clone
  (read 2026-10-17): voice clone, "in beta and is being released gradually",
  Pro and above, uses AI credits, scripts up to 5,000 characters, up to 5
  clones per studio on Pro, Grow and Webinar.
- https://support.riverside.com/hc/en-us/articles/39640475250461-Create-an-AI-voice-clone-of-a-guest
  (read 2026-10-17): Plan: "Business". The guest records a consent video
  reading a fixed script before their clone can be used.
- https://support.riverside.com/hc/en-us/articles/26099013514013-Generate-audio-and-sync-lips-to-correct-recording-VideoDub
  (read 2026-10-17): VideoDub "automatically adjusts both the audio and lip
  movements to match your corrected text". Pro and above. "You can apply
  VideoDub to up to two words at a time. If two words are selected, they will
  be replaced with a single dubbed word."; "Full sentence dubbing isn't
  supported at this time." Guest tracks need a legal disclaimer accepted.
- https://support.riverside.com/hc/en-us/articles/28812004829853-AI-credits
  (read 2026-10-17): 200 credits = 1 minute of AI Twin video; 200 credits =
  1 hour of voice clone audio; 100 credits = 1 minute of AI translation; 100
  credits = 5 seconds of AI B-roll. "AI credits are purchased separately
  from your subscription and do not renew monthly." The Credits row "appears
  in the account menu on paid plans only".
- https://support.riverside.com/hc/en-us/articles/20173322157341-AI-at-Riverside-Everything-you-need-to-know
  (read 2026-10-17): AI Twin creates "an AI Avatar of yourself"; AI
  Translation "into 30 languages, preserving each speaker's voice". Riverside
  "leverages third-party AI sub-processors and our own in-house AI"; named
  sub-processors include OpenAI, Eleven Labs, Heygen, Auphonic, Hedra and
  Pika (named in the data-retention FAQ); sub-processors are under Data
  Processing Addendums "to ensure that: They do not use customer data to
  train their own models."

### Uploads and exports

- https://support.riverside.com/hc/en-us/articles/12728608106653-Upload-video-or-audio-file-for-editing
  (read 2026-10-17): Plan: "All plans". Upload a file recorded outside
  Riverside to transcribe and edit it; choose number of speakers.
- https://support.riverside.com/hc/en-us/articles/12728645414941-Supported-external-media-file-types-and-requirements
  (read 2026-10-17): up to 4 hours per file, up to 25 GB.
- https://support.riverside.com/hc/en-us/articles/27728436340125-What-are-the-limits-for-uploading-external-files
  (read 2026-10-17): Pro, Grow, Webinar: 15 hours of external uploads a
  month; Business unlimited. Free not listed.
- https://support.riverside.com/hc/en-us/articles/5261062677021-Export-options-Overview
  (read 2026-10-17): audio export default "WAV HD", MP3 option; "Toggle
  Remove watermark (All paid plans)" and "Toggle Remove audio watermark (All
  paid plans)", i.e. removal is a toggle at export; optional normalise and
  remove background noise.
- https://support.riverside.com/hc/en-us/articles/5545973795357-What-is-the-Created-with-Riverside-watermark
  (read 2026-10-17): video exports get a small "Created with Riverside"
  watermark; audio-only exports get a "Powered by Riverside" audio track at
  the beginning. "Your separate, high-quality tracks do not include the
  watermark." Live streams carry a small Riverside logo "on all Riverside
  plans", which can be removed.
- https://support.riverside.com/hc/en-us/articles/5589868837405-Remove-watermark-from-media-in-the-editor
  (read 2026-10-17): watermark removal: Pro, Grow, Webinar, Business. "You
  can choose whether to include the watermark"; toggle "Remove watermark" at
  export.

## Unverified or contradictory (do not state as fact)

- **US dollar and euro prices.** The served HTML and the FAQ say Pro $29 a
  month or $24 billed yearly, Grow $39 or $34, Webinar $99 or $79. The live
  pricing API returns 35/24, 45/34 and 99/79 for USD too, so the $29 and $39
  monthly figures look stale. We did not see the page render in dollars or
  euros. **Do not quote dollar or euro prices.** Quote the GBP figures with
  "as shown to a UK visitor".
- **"Up to 20%" annual saving.** Banner and FAQ say up to 20%; £35 to £24 is
  about 31%. Do not quote a percentage.
- **Separate track hours.** Resolved on the rendered page: plan cards, FAQ
  and the rendered comparison table all give 15 hours (Pro), 20 (Grow);
  cards and FAQ give 25 (Webinar). The "5 hours per month" (Pro) row in the
  earlier version of this file comes from the unrendered fallback HTML only
  and is not shown to visitors. Posts no longer need a "table differs"
  caveat.
- **"One-off" for the Free plan's 2 hours.** Only in the unrendered fallback
  table. The rendered card says "Try 2 hours". Do not say "one-off" or
  "once" as Riverside's wording; "a 2-hour trial" is fair from "Try".
- **Download hours mechanics.** The help articles say the allowance "resets
  each month" and also that the option to download disappears "once you
  have recorded over 15 hours", referring to "lifetime recording hours", and
  that live streaming counts. Posts may say the articles describe it both
  ways and that it is counted against recorded hours; do not describe the
  exact mechanics beyond that.
- **Webinar annual total.** Resolved: the rendered page says "Billed £948
  annually" (= £79 x 12). The "$408" was in the unrendered fallback only.
- **Free trial on Business.** The help centre says "any Riverside plan"; the
  pricing page shows a trial button only on Pro, Grow and Webinar.
- **Filler word removal on Free.** Help centre says "All plans"; the pricing
  page lists "remove silences & filler words" under Pro. Posts say the help
  centre lists it on all plans and the pricing page presents it as a Pro
  feature.
- **Transcription on Free.** Pricing lists "Unlimited transcriptions" on Pro;
  Free limits on transcription were not stated. Not claimed.
- **External uploads on Free.** Upload article says "All plans" but the upload
  limits article does not list Free. No Free upload limit is claimed.
- **EUR prices.** Not seen rendered. Not stated.
- **Hands-on behaviour.** None of this was tested in the product.

## Other tools (alternatives table only)

- **Descript**, https://www.descript.com/pricing (read 2026-10-17): Free plan
  at $0, paid plans Hobbyist, Creator, Business, Enterprise; text-based
  editing; "Remove Filler Words"; AI speech with custom voice clones on paid
  plans (limited on Free). The pricing page also has a "Remote recording"
  row (recording session hours per drive: 2 / 5 / 15 / 25 a month).
  https://www.descript.com/rooms (read 2026-10-17): "Descript Rooms is a
  remote recording studio that runs in your browser. Everyone records locally
  in up to 4K"; "Every participant gets a separate file, recorded on their own
  machine". So Descript **does** record remote guests on local separate
  tracks; the earlier "check their site" was wrong.
- **Podcastle**, https://podcastle.ai/pricing (read 2026-10-17): redirects
  (308) to https://async.com/pricing, branded Async. That page lists a Free
  plan, "Remote video & audio recording", "Remote multitrack recording",
  "Text-based audio editing", "AI Silence removal", "1000+ AI voices" and
  voice cloning. Prices did not render in the text read; not stated.
  https://async.com/podcast-studio (read 2026-10-17) is headed "Formerly
  Podcastle", which supports "Podcastle (now Async)".
- **CapCut**, https://www.capcut.com/ (read 2026-10-17): "AI-Powered Photo &
  Video Editor for Everyone"; automatic captions; AI text to speech; "Try
  online for free". Text-based editing and filler removal not mentioned on
  that page; not claimed.
- **Cleanvoice**, https://cleanvoice.ai/pricing/ (read 2026-10-17): AI audio
  cleanup: filler words, background noise, mouth sounds and breaths, silence,
  echo; pay as you go and subscriptions; free trial with no card. Header
  price ("from €10/month") and listed USD prices disagree; prices not stated.
- **Audacity**, https://www.audacityteam.org/ (read 2026-10-17): free, open
  source, Windows, macOS and Linux; "free software for recording and editing
  audio".
