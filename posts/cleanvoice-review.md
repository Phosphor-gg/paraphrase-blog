---
title: "Cleanvoice review: what it is good at and where it stops"
date: 2026-10-17
description: "An honest review of Cleanvoice from a company that makes a different kind of speech editor. What it removes, how you get your edits back, what it costs, and where sound-based clean-up stops."
---

# Cleanvoice review: what it is good at and where it stops

**Bottom line:** Cleanvoice is a thorough, hands-off clean-up service. One pass can cut filler
words, stutters and long pauses and remove mouth clicks, breaths, background noise and echo, with
filler removal in more than 20 languages, from $11 (€10) a month. It detects sounds rather than
editing by transcript, and nothing on its pages describes cutting a false start, a hedge or a
point you made twice in different words; for that, add a transcript editor such as Paraphrase.

We make Paraphrase, a transcript-based editor, so treat this as an interested party's assessment.
**We have not used Cleanvoice hands-on for this review.** Everything about Cleanvoice below comes
from its own pages, read on 17 October 2026, and where we could not confirm something we say so
rather than guess.

## What Cleanvoice is

Cleanvoice is a browser-based AI service for spoken-word audio and video. You upload a file (or
several, or up to five tracks of one conversation), pick a template that says which fixes to apply,
and it processes the file and hands back a cleaned version. It describes its approach as "Clean,
then Enhance, then Edit", and it also has a REST API with Python and JavaScript SDKs.

## What Cleanvoice does well

**It removes things a transcript cannot see.** This is the big one. Mouth clicks, lip smacks and
saliva crackle; breaths, which you can mute or just reduce; hum, hiss, fans, wind, traffic, cafés,
audience chatter and room reverb; uneven loudness. None of those are words, so no transcript editor will
find them. If you record close to a sensitive microphone, or anywhere that is not a studio, this is
the work that takes hours by hand.

**The cuts are designed to sound natural.** When it removes a filler, Cleanvoice says it "adds
silence (room noise) to make the flow of the podcast more natural". Its silence remover shortens
pauses by context: a thinking pause gets shorter, while a longer pause at a change of topic stays.
Its stutter remover tries to "edit out the stutter without cutting the word out".

**It is honest about its own limits.** Its pages tell you that "not every um has to go" and that
removing all of them "can make speech sound clipped", that a few soft mouth clicks inside words may
remain because removing them could damage the word, and that a voice buried under very loud noise
can leave artefacts. Each one ends with the same advice: listen back, or preview, before you
publish. That is good advice, and unusual to see
on a product page.

**It respects video and multitrack timelines.** You can **mute edits instead of cutting them**
(Preserve Length), so a video or other footage stays in sync. Up to five tracks are edited
together and kept in sync.

**Languages are broad.** Filler removal works in more than 20 languages, including English,
German, French, Dutch, Spanish, Italian, Portuguese, Polish, Arabic, Turkish and Bulgarian, and the
sound fixes are language-agnostic. Because filler detection "works on how speech sounds, not on
text", Cleanvoice says it copes with accents too.

**Pricing is simple.** Every plan includes every feature, subscription hours roll over up to three
months' worth, and pay-as-you-go packs last two years. There is a separate breakdown of
[Cleanvoice pricing](/blog/cleanvoice-pricing).

**It does extra jobs around the edit.** Transcription in 99 languages with .srt export, summaries,
show notes, chapters and social posts, plus batch upload.

## Where Cleanvoice stops

**It listens for sounds, not for meaning.** Cleanvoice's own FAQ says it "doesn't work based on the
transcript-to-edit flow". That is a real design choice with real advantages, and it also sets the
ceiling. A false start ("so what we, what I mean is"), a hedge ("I think, sort of, maybe"), or the
same point made twice in different words can be clean, fluent speech as far as sound goes.
Deciding whether it should stay is a judgement about what you meant, and nothing in the Cleanvoice
documentation we read describes making that judgement. (Its stutter page mentions "repeated
words", while its help centre says removing repetitive words is "yet to go live", so we make no
claim either way about word-for-word repeats.)

**Changing individual edits happens elsewhere.** After processing, Cleanvoice's own guide describes
a report of how many fillers, stutters, breaths and pauses were removed, with playback and a toggle
between the original and the edited version. Its documented way to change specific edits is to
export markers or timestamps into Audition, Premiere, DaVinci Resolve, REAPER, Audacity or an EDL
editor and adjust them there. The timestamp export marks fillers, stutters and mouth sounds, but
not dead air. Its help centre also says you cannot choose time ranges to apply or skip edits, and
points to the same export instead. No page we read says outright whether you can restore a single
edit inside the web app, so we are not claiming either way. If you already work in one of those editors,
the export is a strength. If you do not, it is an extra application.

**Files are kept for seven days.** Original and edited files are deleted permanently after 7 days,
which is good for privacy and means going back to re-process an old episode needs your own copy.
Reprocessing is billed as a new edit, according to its help centre.

**Short files cost a little more than their length.** Billing rounds each file up to the minute,
with a one minute minimum.

## Where Paraphrase fills the gap, and where it does not

Paraphrase edits your recording by its transcript. Every word has a timestamp; you click a word to
cut it and click again to restore it, drag words to reorder them, and export your original audio
with the pieces cut out. The [Clean up with AI](/docs/ai-cleanup) button has a language model read
the transcript and propose a cut: filled pauses, false starts, hedges and repetition, including the
same point made twice in different words, and it can move words where a sentence reads better. It
has no word list; it judges each word in context. Every proposed cut shows struck through, and any word
can be put back.

Where it does not fill the gap, plainly:

- **No sound processing at all.** No noise removal, enhancement, levelling or EQ, and since every
  edit is a choice of which words stay, no mouth sound or breath removal.
- **Narrower languages.** Transcription covers 25 European languages, and the cleanup has been
  tested on English speech.
- **No multitrack, speaker labels, captions, summaries or public API.**
- **Free tier is small.** 15 minutes of transcription, three cleanups a day, projects up to 5
  minutes. Premium is £13.99 a month.

There is a [full comparison](/blog/paraphrase-vs-cleanvoice) of the two approaches, and a roundup
of [Cleanvoice alternatives](/blog/cleanvoice-alternatives).

## Who Cleanvoice is right for

Cleanvoice is right for you if your recordings have noisy rooms, close-mic clicks and breaths, lots
of ums, and you want them fixed with as little effort as possible, especially across many files,
many languages or several tracks. Audio engineers who already finish in Audition or REAPER get a
fast first pass they can refine in the tool they know.

It is not sufficient on its own if your edit is about the words: rambling, restarted sentences,
points made twice. That is a description of what sound-based clean-up is for rather than a
criticism, and running a transcript editor alongside it is a normal answer.

The quickest way to judge is on your own recording. Cleanvoice has 30 free minutes, and a
[free Paraphrase account](https://paraphrase.bot) gives you 15 minutes of transcription and three AI
cleanups a day, with no card. Run the same take through both and listen to what each one cuts.
