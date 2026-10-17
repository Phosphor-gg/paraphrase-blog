---
title: "Is Audacity free? What it costs and what it does not do"
date: 2026-10-17
description: "Audacity is free and open source, with no paid tier for the editor. Here is what is genuinely free, where money can come in (cloud storage, MuseHub add-ons), and what the free editor does not do for spoken word."
---

# Is Audacity free? What it costs and what it does not do

**Bottom line:** yes. Audacity is free and open source under the GNU General Public License, with
no paid version of the editor and no subscription, and its noise reduction, compression and
loudness tools are all included. The places money can come in are optional: extra cloud storage
on audio.com and paid plugins on MuseHub. What free does not buy you is a faster way to cut speech,
because editing is still done on the waveform.

Audacity's own homepage is direct about it: "Audacity has always been and will always remain free
for everyone." The FAQ adds that "Audacity is licensed under the GNU General Public License", and
the project describes itself as open source, with its source code "open to anyone to view or
modify". All checked on 17 October 2026.

## What Audacity costs

Nothing, for the editor. There is no paid edition and no subscription for Audacity itself. You
download it for Windows, macOS or Linux and keep using it. The current version is 4.0.1,
and older releases back to 3.0.0 are still on the download site.

The February 2024 announcement about audio.com put the commitment in writing: "Audacity will, of
course, always remain 100% free and open source."

## What you get for free

More than most paid tools in this space, on the processing side:

- **Recording and multitrack editing.** Record, import, cut, split, trim, move clips between
  tracks, mix and pan. Unlimited undo during a session.
- **Noise Reduction.** Select a few seconds of background noise, get a noise profile, then apply it
  to the rest. Audacity says it works best on steady noise: hiss, fan noise, 50 or 60 Hz hum,
  buzzing.
- **Noise Gate and Notch Filter**, for quiet gaps and a hum at one frequency (documented in the
  Audacity 3 manual).
- **Compressor**, as a destructive or realtime effect, with factory presets.
- **Loudness Normalization** to a LUFS target, which Audacity's manual describes as the loudness
  "required by podcast platforms".
- **Other effects**: reverb, echo, delay, distortion, pitch, speed, reverse and vocal remover.
- **Plugins.** Audacity 4 loads VST3, LV2 and Audio Units plugins.
- **Export** to formats including MP3, WAV, FLAC, Opus and M4A (AAC). M4A needs FFmpeg, which
  Audacity cannot bundle for patent reasons, so it is a separate free install.

## Where money can come in

None of these are required to use Audacity.

**Cloud storage on audio.com.** Audacity can save projects to audio.com, which Audacity calls its
"online companion", with backups, versioning and sharing. The February 2024 announcement said "we
will offer 5 projects completely free, but charge a small fee for usage beyond this amount", and
the FAQ refers to people who "signed up for additional Audacity Cloud storage". We could not read
audio.com's subscription page on 17 October 2026, so we are not quoting its current prices or free
allowance. Check it yourself if you plan to rely on cloud saving.

**MuseHub add-ons.** Audacity's site links to MuseHub, which it calls "the official distributor of
Audacity", and to plugins including the Soap Voice Clean & Capture Bundle (described as able to
"Clean up spoken voice and create instant transcripts"), Speaker Splitter Pro, Trinity EQ, MuseFX
and Graillon 3. We could not read the MuseHub pages to confirm their prices, so we are not stating
them.

**Your time.** This is the real cost for spoken word, and it is the next section.

## What Audacity does not do for spoken word

Free is not the same as quick. For editing speech, three things are worth knowing before you
commit an evening to it.

**You cut on the waveform.** To remove something, you select it by clicking and dragging in the
waveform, then delete it. Audacity's own Cut page lists removing "ums, coughs, and long pauses"
as a use for that command, which means finding each one yourself. On a long interview, that is a
lot of scrubbing and listening.

**Transcription is a plugin, and currently behind the latest version.** Audacity's transcription
feature page describes running Whisper "entirely on your own computer" via the free OpenVINO AI
plugin, with "no minute limits, no subscription", in 99 languages. That is genuinely generous. But
Audacity's own OpenVINO download page warns that "The OpenVINO plugins are not yet compatible with
the latest Audacity version", and the builds it links are for Audacity 3.7.1 on Windows and macOS.
If you want transcription today, you may need to stay on 3.7.

**The transcript does not drive the edit.** Whisper writes words into a label track you can "edit,
search, and export as SRT subtitles, VTT, or plain text". The feature page does not describe
deleting a word in that transcript and having the audio follow. The labels help you find things;
you still cut on the waveform.

None of this is a criticism. Audacity is a general audio editor, built for music, restoration,
podcasts and everything else. Word-level cutting of speech is a narrower job.

## How Paraphrase prices the narrower job

Paraphrase does that narrower job and nothing else: it transcribes your recording, you click words
to cut them or drag them to reorder, and it exports your original recording with those pieces
removed. It never generates speech. It also has none of Audacity's processing: no noise removal,
no levelling, no EQ, no effects.

It is paid, and it prices by transcription because that is where its cost is. One credit
transcribes one second of audio, spent once. Editing, AI cleanup and export do not use credits, so
re-editing and re-exporting are free.

| Plan | Price | What it includes |
| --- | --- | --- |
| Free | £0 | 15 minutes of transcription, no card, 3 AI cleanups a day, projects up to 5 minutes |
| Premium monthly | £13.99 a month | 120 hours of audio a month, 30 AI cleanups a day, projects up to 4 hours |
| Premium annual | £83.85 a year | About £6.99 a month, same allowances |
| Premium three years | £179.65 | About £4.99 a month, same allowances |

Credit packs are £3.99 for 4 hours, £12.99 for 13 hours 20 minutes and £34.99 for 40 hours, and do
not expire while your account is open. There is a seven day Premium trial on the monthly and annual
cycles, card required. Prices in GBP, checked 17 October 2026. Full details are on the
[pricing page](/pricing) and in [credits and plans](/docs/credits-and-plans).

## Comparing the two honestly

- **Audacity costs nothing.** If your edits are light, or your time is cheaper than a
  subscription, it is the right answer and you should not pay anyone, including us.
- **They are not buying the same thing.** Audacity gives you a full audio workstation for free.
  Paraphrase charges for a different way of cutting speech: by its words, with an AI pass that
  proposes the cuts.
- **Paraphrase does not replace Audacity's processing.** If your recording has hiss or hum, or
  needs levelling for a podcast platform, you still want Audacity or something like it.

Which is why the honest answer for many people is both: cut in Paraphrase, export WAV or FLAC
(both lossless), finish in Audacity. Our [Audacity review](/blog/audacity-review) covers what it
is like to use, [the alternatives roundup](/blog/audacity-alternatives) covers other options, and
[Paraphrase vs Audacity](/blog/paraphrase-vs-audacity) compares the two directly.

Want to see how long word-level cutting takes on your own recording? [Create a free account at
paraphrase.bot](https://paraphrase.bot): 15 minutes of transcription, no card.
