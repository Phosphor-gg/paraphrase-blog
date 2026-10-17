---
title: "Paraphrase vs Audacity: cutting speech by its words versus on the waveform"
date: 2026-10-17
description: "Audacity is a free, open source audio editor with real noise reduction and effects. Paraphrase is a transcript editor that cuts your own recording by its words. Here is an honest comparison, and why many people use both."
---

# Paraphrase vs Audacity: cutting speech by its words versus on the waveform

**Bottom line:** they do different jobs. **Audacity** is a free, open source audio editor with
noise reduction, compression, loudness normalisation and effects, and you cut by selecting regions
of a waveform. **Paraphrase** transcribes your recording and you cut by clicking words, with an AI
pass that proposes the cuts, but it does no audio processing at all. If your problem is the sound,
use Audacity. If your problem is the hours spent finding ums and restarts, use Paraphrase for the
cut and Audacity for the polish.

Audacity has been the default free audio editor for a long time, and for good reason. If you are
here because editing speech in it is slow, it is worth being clear about why, because that is
exactly where Paraphrase takes a different approach.

## Quick comparison

| | Audacity | Paraphrase |
| --- | --- | --- |
| How editing works | Select and delete regions of a waveform; clips, multitrack, unlimited undo | Click words to cut them, drag to move them; the export is your recording, cut |
| AI cleanup | None built in; its Cut page suggests removing ums by hand | **One button: fillers, false starts, hedges, repetition, reordering; every cut struck through and restorable word by word** |
| Generated speech and voice cloning | Not described on its pages | Never: an export only contains words you said |
| Noise removal and enhancement | **Noise Reduction, noise gate, notch filter, compressor, loudness normalisation** | No |
| Effects and plugins | **Reverb, echo, pitch and more; VST3, LV2, Audio Units, Nyquist** | No |
| Multitrack | **Yes** | No |
| Captions | **Whisper plugin labels export as SRT or VTT** | No |
| Collaboration | **Cloud projects on audio.com, shareable with collaborators** | No |
| Video export | Not covered on its pages | MP4, picture and sound cut at the same words |
| Export formats | MP3, Opus, M4A, WAV, FLAC, Wavpack (some need FFmpeg installed) | WAV, FLAC, MP3, M4A, Opus |
| Transcription languages | Optional Whisper plugin, 99 languages; plugin builds are for 3.7.1, not the current 4.0.1 | Built in, 25 European |
| Platforms | Windows, macOS and Linux desktop | Browser |
| Free plan | **The whole app, free and open source (GPL)** | 15 minutes of transcription once, no card |
| Entry price (checked 17 October 2026) | **Free** | £13.99 a month, or £6.99 a month billed yearly |
| Billing unit | **Nothing to pay; paid cloud storage is optional** | Per account; credits spent only at transcription, so cleanup, re-editing and export are free |

## What editing speech in Audacity actually is

Audacity edits sound. You record or import, and you see a waveform. To remove a section you select
it "by clicking and dragging in the waveform" and press Delete. Audacity's own Cut page suggests
using that command to "Remove ums, coughs, and long pauses from spoken recordings".

For speech, that means:

- Listening through the recording to find each filler, false start and tangent.
- Zooming in to place the selection edges cleanly.
- Cutting, checking, and moving on, with unlimited undo when a cut goes wrong.

Audacity does have transcription: the free OpenVINO AI plugin runs Whisper locally and writes the
words into a label track you can search and export as SRT, VTT or text. The labels are a guide:
nothing on Audacity's pages describes editing that text to cut the audio.

## Where waveform editing hits its ceiling for speech

A waveform shows loudness over time. It does not show words. An "um" and a short word can look much
the same; a false start looks like the rest of the sentence; the same point made twice looks like
two perfectly good paragraphs. To find them you have to listen, which for an hour long interview
means at least an hour of listening before you have cut anything.

That is not a fault in Audacity. It is a general audio editor, built for music, restoration and
everything else. Cutting speech by meaning is a narrower job.

## What Paraphrase does differently

Paraphrase starts from the words:

- **Every word has a timestamp.** Your recording is transcribed, and the transcript is the editor.
  Click a word to cut it, click again to restore it, shift-click to cut a run, drag a word to move
  it. Cut words stay on screen, struck through.
- **Clean up with AI proposes the cut.** One button. A language model reads the transcript and
  marks filled pauses, false starts, hedges and repetition, including the same point made twice in
  different words. It is a proposal: any word can be put back. It is tested on English speech.
- **The export is your recording, cut.** Pieces are removed at word boundaries and joined back up.
  WAV and FLAC are lossless, so a cut of a lossless master stays lossless.
- **It never generates speech.** No voice cloning, no overdub, no text to speech. A word you never
  said cannot appear in the export, because there is no audio for it.
- **Non-destructive and in the browser.** The original is never changed, edits save as you go,
  and there is nothing to install.

You can read more in the [editing docs](/docs/editing) and the
[AI cleanup docs](/docs/ai-cleanup).

## What Paraphrase does not do that Audacity does

If your recording has fan hiss or mains hum, needs levelling, or has to hit a podcast platform's
loudness target, Paraphrase will not help. Audacity will, for free. Paraphrase also has no
multitrack, effects, plugins or subtitles, and it is not free beyond the 15 minute allowance.

## Using both

This is the setup we would actually suggest for spoken word that needs real cleanup:

1. **Record or upload into Paraphrase**, or paste a link. Premium projects hold up to 4 hours of
   recordings.
2. **Cut by the words.** Run Clean up with AI, review what it struck through, put back anything
   that matters, and make your own cuts and reorders.
3. **Export WAV** (lossless) and open it in Audacity.
4. **Finish the sound in Audacity**: Noise Reduction from a noise profile, a Compressor preset,
   then Loudness Normalization to your platform's target.
5. **Export the final file** from Audacity in whatever format you publish.

Because Paraphrase is non-destructive and re-exporting costs nothing, you can go back and change
the cut later and run it through Audacity again.

## Why trust this comparison

Everything above about Audacity comes from Audacity's own pages, all read on 17 October 2026: the
home page, the features pages for cutting, noise reduction and transcription, the FAQ, the download
and Audacity 4 pages, the OpenVINO plugin download page, the AI plugins page, and the support
manual's pages on editing, saving and exporting, FFmpeg, the compressor and loudness normalisation.
Some of the manual still describes Audacity 3, and we have not tested every feature in 4.0.1.

We make Paraphrase, so this is not a neutral comparison. What we have done instead is bold
Audacity's wins in the table, and there are a lot of them.

Audacity's own pages disagree about transcription. The transcription feature page says "Free for
Windows, Mac & Linux" next to a 4.0.1 download button, while the plugin download page warns that
"The OpenVINO plugins are not yet compatible with the latest Audacity version" and offers builds
for 3.7.1 on Windows and macOS only. We went with the download page's warning. We could not read
audio.com's cloud storage prices, so we do not quote them.

**Where Paraphrase leads, and where it does not.** It never generates speech, so an export can only
contain words you said. Every AI cut is shown in the transcript and can be restored word by word.
Credits are spent only at transcription, so cleanup, re-editing and re-exporting are free. It is
also the narrower tool: no remote recording, no noise removal, no captions, no AI voice and no
collaboration, and unlike Audacity it is not free beyond its starting allowance.

We have no customer reviews, ratings or testimonials to show you, because we have not collected
any. Judge it on one of your own recordings instead.

## So which should you use?

Use **Audacity** on its own if your edits are light, your budget is zero, or most of your work is
on the sound itself. It is mature, free and genuinely capable, and our
[Audacity review](/blog/audacity-review) covers it in more depth.

Add **Paraphrase** when cutting speech is what eats your time: long interviews, lectures, courses
or voiceovers where finding the ums and restarts takes longer than recording did. The
[podcast editing](/podcast-editing) and [interview editing](/interview-editing) pages show it on
those jobs.

If neither fits, the [Audacity alternatives roundup](/blog/audacity-alternatives) covers the other
options, and [Is Audacity free?](/blog/audacity-pricing) covers what Audacity costs and where money
can come in.

Paraphrase's free plan gives you 15 minutes of transcription, three AI cleanups a day and projects
up to 5 minutes, with no card. [Create a free account at paraphrase.bot](https://paraphrase.bot)
and cut one of your own recordings by its words, then finish it in Audacity.
