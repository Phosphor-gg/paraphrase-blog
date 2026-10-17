---
title: "Audacity review: what it is good at and where it runs out for speech"
date: 2026-10-17
description: "An honest review of Audacity from a company that makes a transcript editor. Its free, open source audio processing, the Audacity 4 editing changes, the state of its Whisper transcription plugin, and where waveform editing gets slow for spoken word."
---

# Audacity review: what it is good at and where it runs out for speech

**Bottom line:** Audacity is the best free audio editor you can install, with genuine noise
reduction, compression, loudness normalisation and effects, open source and on every desktop
platform. Where it runs out is cutting long spoken recordings: you do it on the waveform, and its
Whisper transcription is a plugin that currently lags the latest release and does not drive the
edit. Keep it for the polish, and add a transcript editor if cutting speech is what takes your
time.

We make Paraphrase, a transcript editor, so treat this as an interested party's view. Every claim
about Audacity below comes from Audacity's own website, support manual and plugin pages, read on
17 October 2026. Where its pages disagree or we could not check something, we say so.

## What Audacity is

Audacity describes itself as "the world's most popular free software for recording and editing
audio". It is open source under the GNU General Public License, runs on Windows, macOS and Linux
(with x86_64 and ARM64 builds), and is desktop only: the FAQ says "There is no mobile version of
Audacity available." The current release is 4.0.1, which rebuilt the interface on Qt. Projects
from Audacity 3 open in Audacity 4 "exactly as you saved it", according to the Audacity 4 page.

## What Audacity does well

**It is free, properly.** "Audacity has always been and will always remain free for everyone." No
paid edition of the editor, no subscription. The optional costs are cloud storage on audio.com and
third-party plugins, covered in [Is Audacity free?](/blog/audacity-pricing).

**The noise tools are real and well documented.** Noise Reduction works from a noise profile: you
select a stretch of background noise, capture it, then apply the reduction to the rest. Audacity is
honest about its limits. It "works best" on steady noise like hiss, fan noise and mains hum; for
"traffic, crowd chatter, or background music" other tools usually do better; heavy settings can
sound watery; and it "cannot fully substitute for good recording conditions". The Audacity 3
manual also documents a Noise Gate, a Notch Filter for hum at a single frequency, and a tip that
mains hum is 50 Hz in most countries and 60 Hz in North and Central America. That is the kind of
detail most products leave you to discover.

**It does the podcast finishing steps.** A Compressor (destructive or realtime, with factory
presets) and Loudness Normalization to a LUFS target, which the manual ties directly to what
"podcast platforms" require. Plus reverb, echo, delay, distortion, pitch, speed and a vocal
remover, and third-party VST3, LV2 and Audio Units plugins.

**Audacity 4 made clip editing nicer.** Clips can be selected directly and several at once with
Shift+Click, trimmed and time stretched with handles, and split with a dedicated tool on the S key.
Trimming is non-destructive. Sync-lock has been replaced by ripple editing, so "Delete and close
gap (all tracks)" keeps a multitrack project in sync.

**Exports are flexible.** MP3, WAV, FLAC, Opus, M4A (AAC) and Wavpack among others, with FFmpeg as
a separate free install for M4A and WMA because of patent restrictions. Projects save as .aup3, or
to audio.com with backups and versioning.

**Transcription, where it works, is generous.** The Whisper plugin runs "entirely on your own
computer", with "no minute limits, no subscription", in 99 languages, and writes a label track you
can export as SRT, VTT or plain text. For subtitles from a local file, that is hard to beat for
free.

## Where Audacity runs out for spoken word

These are not flaws in a general audio editor. They are what happens when you use one for the
specific job of cutting speech.

**You edit sound, not words.** To remove a section you select it "by clicking and dragging in the
waveform" and delete it. Audacity's Cut page suggests using Cut to "Remove ums, coughs, and long
pauses from spoken recordings", and that is a manual hunt: listen, find, zoom, select, cut,
repeat. Unlimited undo helps you recover from a bad cut; it does not help you find the next one.

**The transcription plugin is behind the current release.** Audacity's own OpenVINO download page
says "The OpenVINO plugins are not yet compatible with the latest Audacity version". The builds it
offers are for Audacity 3.7.1, on Windows and macOS only, and the latest release on Intel's
GitHub is from December 2024. The transcription feature page, meanwhile, says "Free for Windows,
Mac & Linux" next to a 4.0.1 download button. We are reporting the download page's warning because
it is the more specific statement, but the two pages disagree.

**The transcript is a guide, not an editor.** Whisper's output lands in a label track you can
"edit, search, and export". Nothing on Audacity's pages describes deleting a word in the transcript
and having the audio cut to match. You can use the labels to jump to the right place, and then you
are back on the waveform.

**No automatic filler or repetition pass.** Audacity's noise tools clean the sound. Nothing we
found in its documentation proposes which words to cut: false starts, hedges or the same point
made twice. That is an editorial job, and in Audacity you are the editor.

**Desktop only.** If you edit on a machine where you cannot install software, Audacity is not an
option.

## Where Paraphrase fills the gaps, and where it does not

Paraphrase is built for exactly the narrow job above. It transcribes your recording with a
timestamp on every word, and every edit is a choice of which words stay:

- Click a word to cut it, click again to restore it. Shift-click to cut a run. Drag a word to
  reorder.
- **Clean up with AI** proposes the cut: filled pauses, false starts, hedges and repetition,
  including the same point made twice in different words. Cuts show struck through and any word can
  be put back. Tested on English speech.
- Non-destructive: the original recording is never changed. Exports are WAV, FLAC, MP3, M4A and
  Opus, or MP4 when the project has a video take.
- It never generates speech, so what you export is only what you said.
- It runs in the browser, so there is nothing to install.

Where it does not fill the gap, plainly:

- **No noise removal, speech enhancement, levelling, EQ, music or effects.** Everything in the
  "does well" section above is something Paraphrase does not do.
- **No multitrack** and no separate per-speaker tracks, and no speaker labels.
- **No subtitles or captions.** Audacity's Whisper labels can export SRT and VTT; Paraphrase
  cannot.
- **25 European languages**, against Whisper's 99.
- **It is paid beyond a small free allowance**: 15 minutes of transcription free, then £13.99 a
  month or about £4.99 a month on the three year cycle (checked 17 October 2026).
- **It needs a connection.** It is a web app, and transcription runs on Paraphrase's servers.

## Who Audacity is right for

Audacity is right for anyone who wants a capable audio editor at no cost: recording, multitrack
work, noise reduction, compression, loudness and effects, on any desktop. For spoken word with
light edits, it is all you need.

It is slow on its own if you regularly cut long recordings of speech, because the cutting is done
by hand on a waveform. The common answer is to use both: cut by the words in Paraphrase, export a
lossless WAV or FLAC, and finish the sound in Audacity. See
[Paraphrase vs Audacity](/blog/paraphrase-vs-audacity) for that workflow and
[Audacity alternatives](/blog/audacity-alternatives) for the other options. Our
[podcast editing](/podcast-editing) page shows the Paraphrase side.

To try word-level cutting on one of your own recordings, [create a free account at
paraphrase.bot](https://paraphrase.bot). No card needed.
