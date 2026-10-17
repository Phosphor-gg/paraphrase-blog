---
title: "Which text-based editors generate AI speech? An audit"
date: 2026-10-17
description: "Most transcript editors can now put words in a voice that nobody recorded. Here is an audit of five podcast and video editors, sorted by what their own pages say they do: generate speech, only cut your own audio, or not edit by transcript at all."
---

# Which text-based editors generate AI speech? An audit

**Bottom line:** of the four tools we checked that edit by transcript, two generate speech inside
the editor: **Descript** (Regenerate, custom voice clones, text to speech) and **Riverside** (AI
Voice, a voice clone in beta, VideoDub). **Adobe Podcast**'s FAQ says Enhance Speech "does not
generate or translate", but Adobe Firefly Pro, the plan new customers now buy to get Podcast
Premium, includes Firefly's Generate Speech. **Paraphrase**, which we make, is built so that its
edits can only remove or rearrange words you actually recorded. **Audacity** does not edit by
transcript at all: you edit on the waveform.

This post sorts tools on one axis: can the editor produce audio of words that were never said? It
is an axis Paraphrase leads on by design, so we are saying up front that we chose it. Generated
speech is also genuinely useful, and there is a section below on when you should want it.

## The audit at a glance

| Tool | Category | Edits by transcript | How it generates speech | Consent step on its pages |
| --- | --- | --- | --- | --- |
| Descript | Generates speech | Yes | Regenerate, custom voice clones, text to speech, stock AI speakers | Recorded authorisation from the voice's owner |
| Riverside | Generates speech | Yes | AI Voice (text to speech in your voice), voice clone (beta), VideoDub | AI Voice limited to your own authenticated voice; legal disclaimer for guest tracks in VideoDub; consent video for a guest's clone |
| Adobe Podcast | Generation comes with the plan | Yes, Studio (beta) | Firefly Pro, the plan that includes Podcast Premium, includes Firefly's Generate Speech | n/a |
| Paraphrase | Removes or rearranges only | Yes | Never | n/a |
| Audacity | No transcript editing | No, waveform | n/a | n/a |

## Why this axis matters

**Interviews.** When you publish an interview, listeners assume the guest said every word they
hear. Cutting, tightening and reordering is ordinary editing. A generated word is a new statement
in someone else's voice, and whether that is acceptable depends on who agreed to it.

**Anything presented as someone's own words.** A lecture, a testimonial, a quote you will be held
to. If the editor cannot generate speech, the export is edited but never added to.

**Consent.** A voice clone is a model of a person's voice. The vendors take this seriously, and
credit to them: Descript "requires explicit recorded authorization from the person whose voice
will be used before creating a voice clone", Riverside's AI Voice works "only ... with your own,
authenticated voice", and Riverside's guest voice clone needs the guest to record a consent video.
The open question is yours: who may use a clone, and whether a guest knows their track could be
changed.

## When you should want generated speech

Being fair: sometimes generation is the right answer. You misspoke a name, the take is otherwise
perfect, and re-recording is not an option. You are building a voiceover from typed script, which
Descript lists as a use for custom voices. Or you are dubbing into other languages: Riverside
describes AI Translation "into 30 languages, preserving each speaker's voice". If that is your work,
a tool that cannot generate speech is the wrong tool.

## Generates speech or clones voices

### Descript

To change what was said, Regenerate lets you highlight script, press D and type new words, and new
audio is generated in the assigned AI speaker. For that use the speaker must have "a custom AI
speaker created and authorized for use in Descript", stock voices are not supported, and
"Regenerate only supports English audio", up to 250 characters per action. Edit for Clarity can go
further: with "Reword for flow" switched on it can "regenerate the audio with AI speech so the
edits sound seamless". Usefully, those AI-generated edits appear in blue.

### Riverside

AI Voice will "use text to generate an audio sample that simulates your speaking voice", on Pro and
above, up to 2,000 characters per generation and 5,000 a month, and Riverside labels it
"experimental". A separate voice clone is "in beta and is being released gradually". VideoDub
"automatically adjusts both the audio and lip movements to match your corrected text", up to two
words at a time, and guest tracks need a legal disclaimer accepted first. A voice clone of a guest
is on the Business plan, and the guest has to record a consent video reading a fixed script before
it can be used.

### The same tools also only cut, most of the time

In both, the documented filler and silence removal tools remove audio, and generation is mostly a
separate feature you choose to use. The exception inside clean-up is Descript's Edit for Clarity,
which can generate speech when "Reword for flow" is on. So whether an export contains generated
speech depends on who used which setting, not on what the tool can do.

## Edits by transcript, with generation in the plan

### Adobe Podcast

Adobe Podcast Studio (labelled beta) edits by transcript: "simply delete text in the transcript to
remove the corresponding audio or video from your project", and you can cut, copy and paste. The
FAQ says Enhance Speech "does not generate or translate".

The plan is where generation comes in. Since 30 August 2026 Adobe no longer sells standalone
Podcast Premium to new customers; they get it through Adobe Firefly Pro, which includes Firefly's
"Generate Speech" (it uses generative credits). Adobe says it is bringing Podcast into Firefly to
"expand into new AI audio capabilities like generating music, sound effects, and speech". So
generated speech is part of what you pay for. See our
[Adobe Podcast review](/blog/adobe-podcast-review) and
[Paraphrase vs Adobe Podcast](/blog/paraphrase-vs-adobe-podcast).

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

### Audacity

Audacity is a waveform editor: you select a section by clicking and dragging on the waveform and
press Delete. Every cut is one you make by hand on audio you recorded or imported. See our
[Audacity review](/blog/audacity-review).

## Why trust this audit

Every claim was read on the vendor's own pages on 17 October 2026: Descript's help centre articles
on Regenerate, Edit for Clarity and custom voice clones; Riverside's help centre articles on AI
Voice, voice cloning, guest voice clones, VideoDub and AI at Riverside; Adobe Podcast's home page,
Enhance Speech and Studio pages, help centre FAQ, technical requirements, guides and Premium plan
change FAQ, and Adobe's UK Firefly plans page; and Audacity's editing support pages.

We make Paraphrase, and this is the axis we lead on, so this is not a neutral audit. Instead we
quote each vendor's own description, safeguards included. It does not lead on fixing a misspoken
word, which needs generation or a new take. Paraphrase facts come from our own code. We have no
customer reviews to cite.

## Which should you use?

- **You need to fix or add words, or dub:** a generator. Descript and Riverside both document
  consent rules for voice clones, and Riverside adds lip sync.
- **You publish interviews or other people's words:** an editor that cannot generate is the
  simplest guarantee. Otherwise, a generator with a clear rule about who may use it.
- **You only want sound cleaned up:** Adobe Podcast's Enhance Speech, or Audacity if free and open
  source matters most.

There is a wider [roundup of text-based editors](/blog/best-text-based-audio-editors-2026) if you
want more than this one axis. If an editor that can only ever cut your own words is what you want,
[make a free Paraphrase account](https://paraphrase.bot), no card needed: a new account gets 15
minutes of transcription to try it on.
