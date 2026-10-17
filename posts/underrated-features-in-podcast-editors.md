---
title: "Underrated features in the podcast editors you already use"
date: 2026-10-17
description: "Six documented features inside Cleanvoice, Riverside, Descript, Podcastle (now Async), CapCut and Audacity that most people never switch on, each sourced from the vendor's own pages."
---

# Underrated features in the podcast editors you already use

**Bottom line:** the overlooked podcast editing feature we would switch on first is **Cleanvoice's
marker export**, which hands its automatic edits to Audacity, Audition, Reaper, Premiere, DaVinci Resolve
or anything that reads .EDL, so you can check and override them. Close behind are **Riverside**
asking which speaker to remove when voices overlap, **Descript's** per-word filler options and
"Avoid harsh cuts", **Podcastle (now Async)'s** remove all for any word, **CapCut's** transcript
fixes that carry into captions, and **Audacity 4's** delete that closes the gap on every track.

"Underrated" is a judgement, so each entry says what the feature does, quoted from the vendor's own
pages, and why we think people miss it. We make a competing editor, and none of the six entries is
ours.

## The list at a glance

| Feature | Where it lives | Why it is worth finding |
| --- | --- | --- |
| Marker and timestamp export | Cleanvoice | Review automatic edits in the editor you already use |
| Overlap-aware word removal | Riverside, all plans | Cut one speaker without taking the other |
| Per-word filler options, "Avoid harsh cuts" | Descript, English transcripts | Choose how each filler goes, skip the ones that would clip |
| Remove all, for any word | Podcastle (now Async), Text Mode | Your own verbal tic, not just the preset fillers |
| Transcript corrections carry into captions | CapCut | Fix a misheard word once |
| Delete and close gap (all tracks) | Audacity 4, free | Multitrack cuts that stay in sync |

## 1. Cleanvoice's marker export

Cleanvoice is usually described as upload, process, download, and that is its core flow. The part
people miss is what happens when you disagree with one of its edits. Its FAQ answers that directly:
"you can export the timestamps or markers of edited parts. You can export them to your preferred
editing tools like Audacity, Audition, Reaper, etc. And edit and customize manually."

Its integrations page names "Adobe Audition, Adobe Premiere, Davinci Resolve, Reaper and Audacity.
And also anything which supports .EDL", and offers two kinds of export. **Markers** show where it
edited, and load onto the cleaned audio. **Timestamps** show what it would edit, and load onto the
raw audio so you make each cut yourself. One limit it states plainly: "We don't highlight deadair
in the timestamp".

Why it is underrated: it turns an automatic tool into a list of suggestions. If you trust it on
mouth sounds and stutters but want to judge every filler yourself, timestamps on the raw file give
you exactly that. And if you edit video, its "Preserve Length" option mutes edits instead of
cutting them, so the picture stays in sync. Our [Cleanvoice review](/blog/cleanvoice-review) covers
the rest.

## 2. Riverside's overlap-aware word removal

Riverside's text-based editing is listed on "All plans": click a word or drag across several, press
Delete, and the removed text stays "shown in gray with a strikethrough". The detail people miss is
what happens when two people talk at once. When speakers overlap, Riverside asks which speaker to
remove, rather than taking both. You can also mute words instead of cutting them.

Why it is underrated: you only meet it when two voices collide, which is exactly where cutting by
transcript is hardest in an interview. Riverside is known for recording, with tracks "recorded
locally on each participant's computer or device"; this is the editing side, and it is easy to
miss. More in our [Riverside review](/blog/riverside-review).

## 3. Descript's per-word filler options and "Avoid harsh cuts"

Descript underlines common filler words in light blue, and its Remove filler words panel lists every
instance with a timestamp and an audio preview. It is tempting to press the button and move on. The
options are worth a look. Each filler can be:

- **Deleted.**
- **Deleted and replaced with a gap**, which keeps a pause where the filler was.
- **Ignored**, which "strikes through the filler word in the script but removes the audio".
- **Removed from the transcript** only, leaving the audio untouched.

Then there is the **"Avoid harsh cuts"** setting, which skips fillers that cannot be removed cleanly.

Why it is underrated: removing every filler can leave speech sounding clipped. Replacing some with a
gap keeps the speaker's rhythm, and "Avoid harsh cuts" stops the tool cutting where it would damage
the words around it. Two limits from Descript's own article: "This feature currently detects filler
words in English transcripts only", and it uses AI credits. See our
[Descript review](/blog/descript-review).

## 4. Podcastle (now Async)'s remove all, for any word

Async's Text Mode has a Filler tab with a preset list: "mmm, um, uh, uhm, uhh, umm, mm, mhm". Useful,
but everyone's real verbal tic is something else. The Words tab lets you search for any word and
**"Remove all"** of its instances.

Why it is underrated: preset filler lists catch sounds, not habits. If you say "basically" forty
times an episode, this is the quickest way to find every one. Listen before you commit, because a
word that is a tic in one sentence can carry meaning in the next. The Silences tab is worth knowing
too: it looks for silences longer than 0.5 seconds by default, "but you can adjust this length". Our
[Podcastle review](/blog/podcastle-review) has more.

## 5. CapCut's transcript corrections carry into captions

In CapCut's transcript-based editing, deleting transcript text removes the matching video, which is
what people expect. Less noticed is that "text corrections carry into the caption track". Fix a
misheard word in the transcript and the caption is fixed with it.

Why it is underrated: for short video with captions, that is one correction instead of two, and one
fewer place for a typo to survive into a published clip. CapCut's filler highlighting comes with
advice worth borrowing in any tool: "Treat highlighting as a shortlist, not a verdict." One caveat:
CapCut's own pages disagree on whether auto captions need Pro, so check in the app. See our
[CapCut review](/blog/capcut-review).

## 6. Audacity 4's "Delete and close gap (all tracks)"

Audacity 4 replaced Audacity 3's Sync-lock with ripple editing, documented in its transition guide
as **"Delete and close gap (all tracks)"**. You can also select several clips with Shift+Click.

Why it is underrated: if you edit a two-person recording on separate tracks, cutting a pause from
one track and not the other is how the conversation drifts out of sync. Closing the gap on every
track at once is the multitrack habit Audacity now builds in, and it is free, with "unlimited undo
throughout the editing session". Our [Audacity review](/blog/audacity-review) covers the rest.

## What we deliberately left off

**Audacity's local Whisper transcription.** It transcribes "locally with Whisper AI" into a label
track you can export as subtitles, which would otherwise be on this list. But the plugin download
page warns "The OpenVINO plugins are not yet compatible with the latest Audacity version", and the
builds offered are for Audacity 3.7.1, so we cannot recommend it to someone on 4.0.1.

## Why trust this list

Every claim above was read on the vendor's own pages on 17 October 2026: Cleanvoice's home page FAQ
and integrations page; Riverside's help centre articles on removing words and on local recording;
Descript's help centre article on removing filler words; Async's help centre articles on Text Mode,
filler words and silence removal; CapCut's transcript editing and filler word pages; and Audacity's
4 transition guide, cut feature page and OpenVINO download page. We did not use review sites, and
we have not tested these features hands-on, so treat "why it is underrated" as our reading of the
documentation rather than a test result.

We make Paraphrase, a competing editor, and none of the six entries is ours. We have no customer
reviews to cite, because we have not collected any.

## What to do with this

Pick the tool you already pay for and try its entry on your next episode. There is a wider
[roundup of text-based editors](/blog/best-text-based-audio-editors-2026) if you are still choosing.

If you have tried all of these and cutting words is still the slow part, that is the one job
Paraphrase does: you edit your own recording by its transcript, the AI cleanup proposes cuts you
can see and undo, and nothing is ever generated. [Make a free account on
paraphrase.bot](https://paraphrase.bot), no card needed, and try it on 15 minutes of your own audio.
