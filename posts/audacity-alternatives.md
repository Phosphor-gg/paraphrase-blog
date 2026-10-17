---
title: "Audacity alternatives: the honest options for editing spoken audio"
date: 2026-10-17
description: "Audacity is free, open source and has real audio processing. If you are looking at alternatives for editing speech, here is what each one replaces, what it costs you, and why many people keep Audacity anyway."
---

# Audacity alternatives: the honest options for editing spoken audio

**Bottom line:** none of the tools below is a free, open source like-for-like replacement for
Audacity, and for noise reduction, compression and effects you probably should not replace it at all. If
what you want is to stop cutting speech by dragging across a waveform, a transcript editor is the
real alternative: **Descript** if you also want AI voices and video tools, **Paraphrase** if you
want your own recording cut by its words and nothing generated. Many people end up using one of
those for the cut and Audacity for the polish.

Audacity describes itself as "the world's most popular free software for recording and editing
audio", and its homepage counts "100M+ downloads since 2000". It is free, it is GPL licensed, it
runs on Windows, macOS and Linux, and it has a wide set of manual audio processing tools. People looking for
alternatives are usually after one of three things, and only one of them is a reason to leave.

## Why people look for Audacity alternatives

**Editing speech on a waveform is slow.** In Audacity you remove a section by selecting it "by
clicking and dragging in the waveform" and pressing Delete. Audacity's own Cut page lists "Remove
ums, coughs, and long pauses from spoken recordings" as a use, and that is exactly how it works:
you find each um by ear and by eye, select it and cut it. For a long interview that is a lot of
listening.

**Transcription is a plugin, and the plugin is behind.** Audacity's transcription runs Whisper
locally through the free OpenVINO AI plugin, which writes the words into a label track. Audacity's
own plugin download page currently warns that "The OpenVINO plugins are not yet compatible with
the latest Audacity version", and the builds it offers are for Audacity 3.7.1 while the current
release is 4.0.1. Even when it is installed, the transcript is labels on a timeline; the feature
page does not describe cutting the audio by editing that text.

**It is desktop only.** Audacity's FAQ says it is "only available for desktop computers or
laptops" and that "There is no mobile version". If you want to edit from a machine you cannot
install software on, that matters.

What is usually **not** a reason to leave is cost or audio processing. Audacity is free, and its
processing tools are extensive. More on that below.

## The alternatives at a glance

| Tool | What it is | How you edit speech | Generates speech? | Free option |
| --- | --- | --- | --- | --- |
| Audacity | Free open source desktop audio editor | Select and cut on the waveform | No | Free, always |
| Descript | AI video and audio editor | Edit the transcript | Yes, AI voices and voice clones | Free plan |
| Riverside | Record, edit and repurpose platform | Text-based editor | Not covered here | Free plan |
| Podcastle (now Async) | Recording and AI editing | Removes filler, pauses, repeats | Yes, AI voices | Free to start |
| CapCut | Photo and video editor | Video timeline, plus transcript-based editing | Not covered here | Free online |
| Cleanvoice | Automatic voice cleanup | Cuts filler and pauses for you | Not covered here | 30 free minutes |
| Paraphrase | Transcript editor for your own recording | Click words to cut, drag to reorder | Never | 15 minutes free |

Feature descriptions for the other tools come from their own homepages (and, for CapCut, its
transcript editing page), read on 17 October 2026.
"Not covered here" means we did not check, not that the tool lacks it.

## Transcript editors

### Descript

Descript calls itself "an AI video and audio editor that lets you edit by editing text", which is
the headline difference from Audacity: you cut the words and the media follows. It also offers "a
realistic voice clone or pick from our stock AI voices" and "Regenerate audio & video", so it can
produce speech you did not record. There is a free plan with no card. If you want one tool that
also handles video and AI voices, it is the obvious place to look.

**Best for:** people who want a transcript editor plus generated voices and video tools. More in
our [Descript review](/blog/descript-review).

### Paraphrase

This is what we make, so weigh it accordingly. Paraphrase is a browser app that transcribes your
recording with a timestamp on every word, then lets you edit by choosing which words stay. Click a
word to cut it, shift-click to cut a run, drag a word to move it. The export is your original
recording with pieces cut out at word boundaries. It never generates speech: no voice cloning, no
overdub, no text to speech, so a word you never said cannot appear in the export
([why we built it that way](/blog/why-paraphrase-never-generates-speech)).

The **Clean up with AI** button reads the transcript and proposes cuts for filled pauses, false
starts, hedges and repetition, shown struck through so you can put any word back. It is tested on
English speech. Transcription covers 25 European languages, detected automatically.

It is **not an Audacity replacement for processing**. Paraphrase has no noise removal, no speech
enhancement, no levelling, no EQ, no music or sound effects, and no multitrack. See
[the full comparison](/blog/paraphrase-vs-audacity).

**Best for:** cutting spoken word by its words, then handing a lossless export to Audacity for the
polish.

### Riverside

Riverside describes itself as a platform to "record, edit, repurpose", with recording "solo or with
guests" in "separate tracks" and a "text-based editor". If your real need is recording remote
guests, that is a different job from what either Audacity or Paraphrase does.

**Best for:** recording guests remotely and editing in the same place. See our
[Riverside review](/blog/riverside-review).

## Automatic cleaners

### Cleanvoice

Cleanvoice's pitch is "Find every filler word and long pause, and cut them out", plus removing
background noise, mouth sounds and breaths. It hands back a cleaned file. You get 30 free minutes
after signing up. It takes the um-hunting you would do by hand in Audacity off your plate without
changing how you edit everything else.

**Best for:** automating filler and noise removal, then carrying on in your usual editor. See our
[Cleanvoice review](/blog/cleanvoice-review).

### Podcastle (now Async)

podcastle.ai now redirects to async.com. That page offers a recording studio, AI voices and voice
cloning, removing "filler, pauses, repeats, bad takes", and background noise removal "with Magic
Dust". It is a broader, AI-heavy product.

**Best for:** people who want recording, AI voices and cleanup in one subscription.

## Video editors

### CapCut

CapCut is an "AI-Powered Photo & Video Editor" with desktop, online and mobile versions, free to
try online. It also has "Transcript-based editing", which its own page describes as "a free online
transcript editor" that picks out filler words and speech gaps for you to remove. If your spoken
audio is really the soundtrack of short videos, a video editor may be what you need rather than an
audio one.

**Best for:** short-form video where the audio is secondary. See our
[CapCut review](/blog/capcut-review).

## What you will struggle to replace

Worth being plain about this. Several tools above offer noise removal (Descript lists "Studio
Sound" and background noise removal, Cleanvoice strips background noise, Async has "Magic Dust",
CapCut lists noise reduction), but **Audacity's hands-on set of processing tools is a different
thing, and Paraphrase has none of it.** Noise Reduction with a noise profile, Noise Gate, a
Compressor with factory presets, plus reverb, pitch, speed and third-party VST3, LV2 and Audio
Unit plugins. The Audacity 3 manual also documents a Notch Filter for mains hum and Loudness
Normalization to the LUFS target podcast platforms ask for. All free, all running on your own
machine.

And it is free and open source: no subscription, no credits. If that matters to you, nothing
else on this list is a like-for-like swap.

## Do you actually need to replace Audacity?

Usually not. The more useful question is whether you need something **next to** it.

If your recordings are clean and your edits are light, Audacity on its own is fine and free. If
what eats your time is finding and cutting ums, restarts and rambling in long spoken recordings,
a transcript editor lets you find and cut them by reading instead of scrubbing, and you can still
finish in Audacity. In Paraphrase
that looks like: cut by the words, export WAV or FLAC (both lossless), then open it in Audacity for
noise reduction, compression and loudness. We cover that in more detail in our
[Audacity review](/blog/audacity-review), and the costs in
[Is Audacity free?](/blog/audacity-pricing).

Paraphrase's free plan gives you 15 minutes of transcription with no card, three AI cleanups a day
and projects up to 5 minutes, which is enough to test it on a real recording. Premium is £13.99 a
month, or about £4.99 a month on the three year cycle, prices checked 17 October 2026. Details are
on the [pricing page](/pricing) and in the [editing docs](/docs/editing).

Try cutting one of your own recordings by its words: [create a free account at
paraphrase.bot](https://paraphrase.bot), no card needed.
