---
title: "Audacity vs Descript vs Paraphrase: waveform, full suite, or words only"
date: 2026-10-17
description: "Audacity is a free, open source waveform editor, Descript is a full transcript editor with AI tools and voices, and Paraphrase cuts your own recording by its words. Here is who should pick which, from each tool's own pages."
---

# Audacity vs Descript vs Paraphrase: waveform, full suite, or words only

**Bottom line:** pick **Audacity** if your budget is zero or your work is on the sound itself: it is
free, open source, runs on Windows, macOS and Linux, and has real noise reduction,
compression and loudness normalisation, but you cut on a waveform. Pick **Descript** if you want to
edit audio and video by transcript with Studio Sound, captions, screen recording and AI voices in one
app. Pick **Paraphrase** if cutting speech is what eats your time and you want the cheapest way to do
it by the words: an AI cleanup you review word by word, free re-editing, and no generated speech.
Many people should pair Paraphrase with Audacity.

## Quick comparison

| | Audacity | Descript | Paraphrase |
| --- | --- | --- | --- |
| How you cut | Select a region of the waveform | Edit the transcript | Click words in the transcript |
| Runs on | Windows, macOS, Linux desktop | macOS and Windows apps, Chromium browsers | Browser |
| Transcription | Whisper plugin, built for 3.7.1 | Built in, around 25 languages | Built in, 25 European languages |
| AI filler and repetition cuts | Not in its documentation | Remove filler words (English only), Edit for Clarity | One AI cleanup: fillers, false starts, hedges, repetition |
| Generated speech | Not described | Regenerate, voice clones, stock AI speakers | Never |
| Noise reduction | Yes, from a noise profile | Studio Sound | No |
| Compressor, loudness normalisation | Yes | Loudness normalise on export | No |
| Plugins and effects | VST3, LV2, Audio Units | Not on the pages we read | No |
| Multitrack | Yes | Multitrack transcription | No |
| Video | Audio only on its pages | Yes | MP4, picture and sound cut at the same words |
| Lossless export | WAV, FLAC and more | WAV | WAV, FLAC |
| Price (checked 17 Oct 2026) | Free, GPL | Free plan; paid from $16 per person a month billed annually | Free 15 minutes; Premium £13.99 a month, about £4.99 on three years |

## What each one is for

**Audacity** is "the world's most popular free software for recording and editing audio", in its
own words, now at version 4.0.1. You record or import, see a waveform, and remove a section by
selecting it "by clicking and dragging in the waveform" and pressing Delete. Around that sit Noise
Reduction, a noise gate, a compressor, Loudness Normalization to podcast platform targets, effects,
third-party plugins and unlimited undo. Its footer credits Muse Group and contributors, and it is licensed
under the GNU General Public License.

**Descript** is an audio and video editor you drive by its transcript. It lists captions, screen
recording, Studio Sound, Remove Filler Words, Remove Retakes, Edit for Clarity, Regenerate,
translation and dubbing, and Rooms for remote recording.

**Paraphrase** transcribes your recording with a timestamp on every word, and every edit is a choice
of which of your words stay and in what order. The export is your original recording with pieces cut
out at word boundaries.

## Where they overlap

All three can take the ums and restarts out of a spoken recording. They differ in how you find them.

**In Audacity** you find them by listening. Its own Cut page suggests using Cut to "Remove ums,
coughs, and long pauses from spoken recordings". A waveform shows loudness, not words, so a false
start or a point made twice looks like any other sentence. Audacity does have transcription, through
the free OpenVINO plugin running Whisper locally, which writes words into a label track you can
search and export as SRT, VTT or text. But its download page warns "The OpenVINO plugins are not yet
compatible with the latest Audacity version", and the builds offered are for 3.7.1. Nothing on
Audacity's pages describes editing that text to cut the audio.

**In Descript** you cut by deleting text. Remove filler words lists each detected filler with a
timestamp and preview, for English transcripts. Edit for Clarity removes "unnecessary or off-topic
content" at Low, Medium or Heavy intensity, keeping cuts as text you can restore. Both use AI credits.

**In Paraphrase** you click a word to cut it, shift-click to cut a run, and drag a word to move it.
[Clean up with AI](/docs/ai-cleanup) has a language model read the transcript and propose cutting
filled pauses, false starts, hedges and repetition, including the same point made twice in different
words. There is no word list, every cut stays on screen struck through, and any word can go back.
It has been tested on English speech.

**Generated speech.** Descript's Regenerate types new words into an authorised voice clone.
Audacity's pages describe no speech generation. Paraphrase **never generates speech**:
a word you never said cannot appear in an export.

## Pricing

Checked on 17 October 2026. We have not converted currencies.

**Audacity** says it "has always been and will always remain free for everyone", with "No
subscription required". Money only comes in for optional extras: paid Audacity Cloud storage on
audio.com and paid MuseHub add-ons. We could not read those prices, so we do not quote them. See
[Is Audacity free?](/blog/audacity-pricing)

**Descript** shows `$` prices without naming the currency: a free plan, then Hobbyist $16 per person
a month billed annually or $24 monthly, Creator $24 or $35, Business $50 or $65, each with media hours
and AI credits that do not roll over. See [Descript pricing](/blog/descript-pricing).

**Paraphrase** is free for 15 minutes of transcription with 3 cleanups a day and no card. Premium is
£13.99 a month, £83.85 a year or £179.65 for three years (about £4.99 a month), with 120 hours of
transcription a month. Credits are spent only at transcription, so re-editing and re-exporting are
free. See [pricing](/pricing).

## What Paraphrase does not do

Audacity does most of this for free, and Descript does much of it too:

- No noise reduction, compression, loudness normalisation, EQ, effects or plugins.
- No multitrack, remote recording or separate per-speaker tracks.
- No speaker labels, captions, subtitles or translation.
- No desktop or mobile app; it runs in the browser.
- No collaboration, comments or share links.
- No AI voice, cloning, overdub or text to speech.

## Which should you pick?

**Your budget is zero, or your edits are light:** Audacity. It is mature and genuinely capable. Our
[Audacity review](/blog/audacity-review) covers it.

**You want one app for audio, video, captions and remote guests:** Descript. See our
[Descript review](/blog/descript-review).

**Cutting long interviews, lectures or voiceovers takes longer than recording them:** Paraphrase for
the cut, then Audacity for the sound. Export WAV from Paraphrase, then run Noise Reduction, a
compressor and Loudness Normalization in Audacity. Because re-editing is free, you can change the cut
later and run it through again. See [interview editing](/interview-editing) and
[podcast editing](/podcast-editing).

**You need certainty that no word was generated:** Paraphrase, which has no way to generate one.

The pairwise post is [Paraphrase vs Audacity](/blog/paraphrase-vs-audacity), and
[Paraphrase vs Descript](/blog/paraphrase-vs-descript) covers the other side.

## Why trust this comparison

Audacity facts come from audacityteam.org (home page, features, FAQ, download, OpenVINO download and
Audacity 4 pages) and support.audacityteam.org (editing, export, FFmpeg and noise reduction
articles). Descript facts come from descript.com/pricing and /features and its help centre articles
on filler words, Edit for Clarity, Regenerate, platforms and audio export. All were read on 17
October 2026, and we have used neither hands-on for this post.

Paraphrase is ours, so this is not neutral. Where it leads: it never generates speech, every cut its
AI proposes is reviewable word by word, and re-editing is free. Where it does not: it is the
narrowest product here, with no remote recording, no noise removal, no captions and no AI voice, and
unlike Audacity it is not free beyond the first 15 minutes. We have no customer reviews to cite,
because we have not collected any.

[Create a free account at paraphrase.bot](https://paraphrase.bot), no card needed, and cut one of
your own recordings by its words, then finish it in Audacity.
