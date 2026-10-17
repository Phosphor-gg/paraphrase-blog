---
title: "Which text-based editors generate AI speech? An audit"
date: 2026-10-17
description: "Most transcript editors can now put words in a voice that nobody recorded. Here is an audit of seven podcast and video editors, sorted by what their own pages say they do: generate speech, only cut your own audio, or not edit by transcript at all."
---

# Which text-based editors generate AI speech? An audit

**Bottom line:** of the five tools we checked that edit by transcript, four can generate speech:
**Descript** (Regenerate, custom voice clones, text to speech), **Riverside** (AI Voice, a voice
clone in beta, VideoDub), **Podcastle (now Async)** (over 1,000 AI voices, voice cloning, sentence
regeneration) and **CapCut** (an AI voice clone overdub in certain regions, plus text to speech).
**Paraphrase**, which we make, is the one whose edits can only remove or rearrange words you
actually recorded. **Cleanvoice** and **Audacity** do not edit by transcript at all, and the pages
we read for them do not describe generating speech.

This post sorts tools on one axis: can the editor produce audio of words that were never said? It
is an axis Paraphrase leads on by design, so we are saying up front that we chose it. Generated speech is
also genuinely useful, and there is a section below on when you should want it.

## The audit at a glance

| Tool | Category | Edits by transcript | How it generates speech | Consent step on its pages |
| --- | --- | --- | --- | --- |
| Descript | Generates speech | Yes | Regenerate, custom voice clones, text to speech, stock AI speakers | Recorded authorisation from the voice's owner |
| Riverside | Generates speech | Yes | AI Voice (text to speech in your voice), voice clone (beta), VideoDub | AI Voice limited to your own authenticated voice; legal disclaimer for guest tracks in VideoDub |
| Podcastle (now Async) | Generates speech | Yes, Text Mode | AI voices, voice cloning, regenerating sentences | "Voice Captcha" named, not explained |
| CapCut | Generates speech | Yes | AI voice clone overdub (certain regions), text to speech | Not documented |
| Paraphrase | Removes or rearranges only | Yes | Never | Not applicable |
| Cleanvoice | No transcript editing | No | Not documented | Not applicable |
| Audacity | No transcript editing | No, waveform | Not documented | Not applicable |

"Not documented" means the vendor pages we read did not say either way. It is not a claim that
the feature is missing.

## Why this axis matters

**Interviews.** When you publish an interview, listeners assume the guest said every word they
hear. Cutting, tightening and reordering is ordinary editing. A generated word is a new statement
in someone else's voice, and whether that is acceptable depends on who agreed to it.

**Anything presented as someone's own words.** A lecture, a testimonial, a quote you will be held
to. If the editor cannot generate speech, the export is edited but never added to.

**Consent.** A voice clone is a model of a person's voice. The vendors take this seriously, and
credit to them: Descript "requires explicit recorded authorization from the person whose voice
will be used before creating a voice clone", and Riverside's AI Voice works "only ... with your own,
authenticated voice". The open question is yours: who may use a clone, and whether a guest knows
their track could be changed.

## When you should want generated speech

Being fair: sometimes generation is the right answer. You misspoke a name, the take is otherwise
perfect, and re-recording is not an option. You are building a voiceover from typed script, which
Descript lists as a use for custom voices. You want intros, outros and sponsor reads without
re-recording, which are Async's own examples. Or you are dubbing into other languages: Riverside
describes AI Translation "into 30 languages, preserving each speaker's voice". If that is your work,
a tool that cannot generate speech is the wrong tool.

## Generates speech or clones voices

### Descript

Regenerate lets you highlight script, press D, type new words and get audio "in the assigned AI
speaker". The speaker must have "a custom AI speaker created and authorized for use in Descript",
stock voices are not supported, and "Regenerate only supports English audio", up to 250 characters
per action. Edit for Clarity can go further: with "Reword for flow" switched on it can "regenerate
the audio with AI speech so the edits sound seamless". Usefully, those AI-generated edits appear
in blue.

### Riverside

AI Voice will "use text to generate an audio sample that simulates your speaking voice", on Pro and
above, up to 2,000 characters per generation and 5,000 a month, and Riverside labels it
"experimental". A separate voice clone is "in beta and is being released gradually". VideoDub
"automatically adjusts both the audio and lip movements to match your corrected text", up to two
words at a time, and guest tracks need a legal disclaimer accepted first. The help centre also has
an article titled "Create an AI voice clone of a guest"; we read only the title.

### Podcastle (now Async)

Async offers "1000+ AI voices", narration in 15 languages, and "Regenerate only the sentences you
want to polish". Its voice cloning page says you can "clone your voice in just 3 seconds" from one
sentence or any uploaded audio, and describes the result, honestly, as "new speech you never
actually recorded".

### CapCut

CapCut's overdub page says its "AI voice cloning technology enables you to generate a precise and
accurate version of your voice", used to replace "incorrect audio with accurate voice-over by
editing the transcript". It adds: "This feature is only available in certain regions." Text to
speech, an AI voice generator, a voice changer and AI dubbing are listed as separate tools.

### The same tools also only cut, most of the time

In all four, the everyday cleanup features (filler words, silences, retakes) remove audio, and
generation is a separate step you choose. So whether an export contains generated speech depends on
who used which setting, not on what the tool can do.

## Cleanup only removes or rearranges your own audio

### Paraphrase

This is ours. Every edit, yours or the AI cleanup's, is a choice of which of your recorded words
stay and in what order. The cleanup proposes cuts for filled pauses, false starts, hedges and
repetition, and can move words; every cut shows struck through for you to restore. There is no
voice model, no overdub and no text to speech, so a word you never said cannot appear in an
export. [Why we built it that way](/blog/why-paraphrase-never-generates-speech).

The cost is real: Paraphrase cannot fix a misspoken word. You cut around it, or record a pickup
take into the same project and use the right word from that.

## No transcript editing at all

### Cleanvoice

Cleanvoice's FAQ says it "doesn't work based on the transcript-to-edit flow". You upload a file and
it removes filler words, stutters, mouth sounds and breaths, and shortens dead air. Where it cuts a
filler it "adds silence (room noise) to make the flow of the podcast more natural", which is room
tone, not speech.

### Audacity

Audacity is a waveform editor. Its optional Whisper plugin transcribes into a label track, but the
page does not describe editing the audio by editing that transcript. The OpenVINO plugin page lists
music separation, noise suppression, music generation, transcription and audio super resolution;
none of those is described as generating speech.

## Not documented

- **Cleanvoice and Audacity:** whether they can generate speech in any form. Nothing we read says
  they can; we are not claiming they cannot.
- **CapCut:** which regions get the voice clone overdub, and whether there is a consent step.
- **Podcastle (now Async):** what "Voice Captcha" involves, and which plans include voice cloning.
- **Riverside:** how guest voice clones work, beyond the article title.

## Why trust this audit

Every claim was read on the vendor's own pages on 17 October 2026: Descript's help centre articles
on Regenerate, Edit for Clarity and custom voice clones; Riverside's help centre articles on AI
Voice, voice cloning, VideoDub and AI at Riverside; Async's text to speech, voice cloning and
pricing pages (podcastle.ai now redirects there); CapCut's overdub tool page and pricing page
navigation; Cleanvoice's home page and filler words FAQ; and Audacity's transcription and OpenVINO
plugin pages. We did not use review sites or test the other tools hands-on.

We make Paraphrase, and this is the axis we lead on, so this is not a neutral audit. Instead we quote each vendor's own description, safeguards
included, and mark what we could not read. Paraphrase facts come from our own code. We have no customer
reviews to cite, because we have not collected any.

## Which should you use?

- **You need to fix or add words, or dub:** a generator. Descript documents its consent rules in
  the most detail, Riverside adds lip sync, and Async lists over 1,000 voices.
- **You publish interviews or other people's words:** an editor that cannot generate is the
  simplest guarantee. Otherwise, a generator with a clear rule about who may use it.
- **You only want sound cleaned up:** Cleanvoice, or Audacity if free matters most.

There is a wider [roundup of text-based editors](/blog/best-text-based-audio-editors-2026) if you
want more than this one axis. If an editor that can only ever cut your own words is what you want,
[make a free Paraphrase account](https://paraphrase.bot), no card needed, with 15 minutes of
transcription to try it on.
