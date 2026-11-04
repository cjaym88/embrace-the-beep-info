# Embrace The Beep

A real-time drum practice tool. Play along to a groove on an electronic kit
or drum pad, and it shows how close each hit landed: early, late, or right
on, as you play.

> **Status: functional prototype, in active development.** The source code is
> private. This page is for following progress, the roadmap, and
> giving feedback.

![Embrace The Beep's Practice screen: a sidebar on the left (Practice,
Metronome, Groove Editor, History, Settings), the Flamacue rudiment as drum
notation with its flams' small slashed grace notes and the sticking (lR, L,
R, ...) printed under each note, a timeline row underneath, and one row of
controls along the bottom: Start, the groove, tempo, loops and
click](screenshots/2026-10-23-practice.png)

*The Practice screen, ready to play the Flamacue rudiment at 80 BPM. The
groove is shown as drum notation, with each flam's grace note just in front
of its main note and the sticking (which hand plays each note) printed
underneath. Below the music, the timeline gets a mark for every hit as you
play. Everything you need is along the bottom: Start, the groove, tempo,
loops and the click.*

## A new app (2026-10-23)

The app has been rebuilt from the ground up as one app for Windows,
Mac, iPhone/iPad and Android. Windows is finished; the others are next.

- **The same scores as before.** The same playing gets the same score as
  in the first version.
- **A steadier click.** On one setup, the click holds its timing to about
  a tenth of a millisecond (the first version's varied by 3-4 ms).
- **All new screens:** a sidebar with Practice, Metronome, Groove Editor,
  History and Settings, in light or dark.

## What it does today

- **Play along to a groove** from a standard `.mid` file or the built-in
  library: rock, funk, shuffle, half-time, swing, blues, bossa nova,
  samba, waltz, disco, punk, blast beats, double bass and more. A count-in
  and a click (beats, 8ths, triplets or 16ths) play with it.
- **Live feedback on every hit**: hit, missed or extra, graded from
  *tight* to *off* by how far from the beat it landed, shown on the
  notation and a timeline as you play.
- **Drum notation**: cymbals, ghost notes, accents, flams, drags, open
  hi-hats, triplets and other tuplets, and the sticking under the notes.
- **Any time signature**, and a different one per bar.
- **Rudiments**: the standard rudiments built in, with their sticking,
  including flams, drags, rolls, paradiddles and ratamacues.
- **Flams and drags scored**, including their grace notes.
- **Listen** to any groove with real drum sounds.
- **A review after each session**: a score out of 100 and stars, each
  note coloured by how it went, every loop's timing and volume, and a
  summary in plain words. **Play back** what you played.
- **Dynamics**: how evenly you play from loop to loop, and whether ghost
  notes stay quiet and accents stand out.
- **History**: every session kept, a chart of your scores per groove,
  and your best for each groove at each tempo.
- **Groove Editor**: make grooves by tapping a grid or by playing them
  in, see them as notation, listen to them, add sticking, and import or
  export `.mid` files.
- **Metronome**: tap tempo, any time signature, subdivisions, swing,
  accents, a full-screen flash and a tempo trainer.
- **Polyrhythms**: up to four click tracks at once.
- **Pad setup by hitting each pad**, with your own extra pieces, and
  several saved kits.
- **Latency calibration** three ways: with a microphone, by tapping
  along, or with your kit's own metronome.
- **Plays alongside other audio**: music, lesson videos or screen
  recording.
- **Runs entirely on your computer**: no account, no internet, nothing
  uploaded.

![The review screen after a session: a score of 93 with four stars and "On
the beat · fairly steady" at the top, a one-bar groove in notation with
each note coloured by how it went, a popup on one open hi-hat note listing
its four loops (tight, good, tight, tight, and how many ms early), and the
timeline underneath with a shape for each hit](screenshots/2026-10-23-review.png)

*A session's review, opened from History: 93 and four stars. Each note is
coloured by how it went over the four loops (green: tight, teal: good).
Tapping the open hi-hat on "1-and" shows every loop: all within 10 ms,
slightly early.*

![The Groove Editor with the Swiss Army Triplet rudiment: a grid with a row
per drum, the snare's notes showing their sticking (rL, L, R), and the grid
menu open for beat 1: 16ths, 32nds, triplets (selected), sextuplets,
quintuplets and septuplets, those the beat's notes wouldn't fit greyed
out](screenshots/2026-10-23-groove-editor.png)

*The Groove Editor with the Swiss Army Triplet open. Tapping a beat's
number opens its grid menu: this beat is in triplets, and the grids its
notes wouldn't fit are greyed out. Each snare note shows its sticking; a
flam's is written with its grace note's hand first ("rL").*

![The metronome: 120 BPM in large numbers with tempo and Tap buttons and
Start, time signatures 3/4 to 7/8 plus Other, a swing slider, and in
polyrhythm mode two tracks: 4 beats with 2 clicks each, and 3 beats, each
step a box as tall as it is loud](screenshots/2026-10-23-metronome.png)

*The metronome playing 4 against 3: the main track in 4/4 with 8ths, the
second track's three evenly spaced beats underneath. Each step is as wide
as it lasts and as tall as it's loud: tap one to accent, soften or mute
it.*

![The groove picker on the Rudiments tab: Single Stroke Roll, Four Stroke
Roll, Triple Stroke Roll, Quads, Double Stroke Roll, 5, 6 and 7 Stroke
Roll, each 4/4, 1 bar](screenshots/2026-10-23-rudiments.png)

*Choosing a groove: built-in grooves, rudiments and your own.*

![Practice with a four-bar groove whose last bar is in 7/8: bars 2 to 4
in notation, the 7/8 bar's hi-hats beamed 2+2+3, the timeline underneath,
and "Bars 2-4 of 4" between the ‹ › arrows](screenshots/2026-10-27-practice-7-8.png)

*A groove that ends with a bar of 7/8. The arrows by the music size
buttons step through a groove that doesn't fit on one screen.*

![The Groove Editor on bar 4, marked "4.1 7/8": its beats grouped 2+2+3,
the rows sorted Crash, Hi-hat, Snare, Kick](screenshots/2026-10-27-groove-editor-7-8.png)

*The same groove in the Groove Editor: bar 4's header shows its time
signature, and Auto-sort has put the drums in staff order.*

![The Groove Editor's menu for bar 2: the bar's time signature at the top,
then beat 2.1's grids, the ones its notes wouldn't fit greyed
out](screenshots/2026-10-27-groove-editor-bar-menu.png)

*Tapping a bar's first beat: that bar's time signature, and the beat's
grid.*

**Works with:** Windows today, plus any electronic kit or drum pad that
sends MIDI over USB. Mac, iPhone/iPad and Android versions are next.

## Coming to phones

The phone screens are laid out for every size from the small iPhone SE to
the largest Pro Max (pictures in the 2026-10-16 changelog). On a phone:

- **Practise with the phone sideways on a stand**, every button big enough
  to tap from the kit.
- **The Groove Editor and recording go sideways too.**
- **The metronome works upright or sideways.**
- **Light and dark**, following your phone's own setting.

## Roadmap

**Next up**
- **Acoustic drums with a microphone.** The first test on a practice pad
  went well (2026-11-03 in the changelog). Next: a snare and a floor tom,
  and checking the timing. If they pass, the app will be able to listen
  to a real drum, not only an electronic kit.
- **Mac**, then **iPhone/iPad** and **Android**, with the same scoring
  on every platform, and flams drawn clearly in the notation on small
  screens.
- **A test version for a few testers** on Windows.

**Patterns**
- More common grooves by genre.
- Checking the new drag rudiments by ear and eye.

**Later**
- Polished, installable apps for all four platforms.

See [CHANGELOG.md](CHANGELOG.md) for what's changed recently.

## Feedback

Ideas and feature requests are welcome. Open an issue on this repo.
