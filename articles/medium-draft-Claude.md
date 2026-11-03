# Eurodance: four MIDI kits, built from rules and checked by script

DRAFT. This article has not been published.

Eurodance hooks: four-on-the-floor drums, octave-jump bass, minor-key piano chords and a steady-eighth lead at 136 to 144 BPM. The pack holds four kits. Each kit has six roles with two variations each as 8-bar MIDI parts, plus one 32-bar arrangement that places those parts. That is 52 MIDI files you can open in any DAW.

## What is inside

- **Neon Crowd**: 140 BPM, A aeolian. Chords: Am (2 bars) | F (2 bars) | C (2 bars) | G (2 bars).
- **Star Ticket**: 138 BPM, D aeolian. Chords: Dm (2 bars) | Bb (2 bars) | F (2 bars) | C (2 bars).
- **Night Bus**: 144 BPM, G aeolian. Chords: Gm (2 bars) | Eb (2 bars) | Bb (2 bars) | F (2 bars).
- **Laser Bridge**: 136 BPM, C aeolian. Chords: Cm (2 bars) | Ab (2 bars) | Eb (2 bars) | Bb (2 bars).

Roles in every kit: drums, bass, keys, motif, sequence and pad. The motif and the sequence never play together in the arrangement. The last eight bars restate the motif from the first eight, so each arrangement has a beginning, a middle and a return.

## How it was made

A script writes the notes from fixed rules and a seeded random generator, so the same inputs give the same MIDI bytes. Then a separate validator reads every file back and checks the format, the tempo, the note ranges, the polyphony limits, the drum map, and that the two variations of a part differ. A second MIDI parser counts the notes again as a cross-check. The validator also rejects a deliberately broken file and accepts a clean one, so you know it can fail. Result for this build: 52 files checked, 0 errors.

## How to use it

Start from the drums and octave bass, then drop the motif on top as the hook.

Use either the combined arrangement or the separate parts. Do not stack the part files on top of the combined file. No program changes are encoded. A conventional GM player will normally use its default piano program for pitched channels unless configured otherwise; compatible GM channel 10 percussion is treated separately. Player behavior may vary.

## What the preview is

Preview is Neon Crowd bars 17-32 at 140 BPM, 27.455 seconds, not the 32-bar MIDI. It is a simple synthesized render of the MIDI, made so you can hear the structure. It is preview, not a master. No human listening audition was performed for this build.

## Limits

The files are notes only. They contain no samples, no sound design and no mix. The artwork is an illustration drawn by code. No license is set in the repository yet.

Repository: https://github.com/mizcausevic-dev/eurodance
