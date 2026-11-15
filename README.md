# Embrace The Beep

A message from CJ:

Hi! Thank you for checking out my drum rhythm trainer app, Embrace The Beep.

I want to take a moment and explain what this app is for, and what it is not. This app is a utility intended to help drummers and percussionists practice specific patterns and get objective, real-time feedback on their timing and dynamics. It includes the ability to chart out grooves and patterns up to 4 bars long, as well as over 75 included in the app. My hope is that by using this app, drummers will be able to more quickly improve their timing and build speed on whatever it is they are working on, so that they can spend more time being creative and performative.

This app is **NOT** a substitute for a drum teacher. Embrace The Beep can tell you how well you're keeping timing and dynamics with extremely high levels of accuracy, but it cannot tell you what you should work on next or if your playing has feel/soul to it. If possible, you should seek out a local drum instructor to help guide you through your learning journey, with Embrace The Beep as a tool to measure a specific aspect of your progress.

While I am working hard on making this app compatible with acoustic drumkits, I anticipate it will be most effective for single-instrument percussionists and e-kit users. The reason is simply that multiple sounds blending together is a lot harder to parse than a single instrument, such as a drumline snare drummer or an e-kit that sends out MIDI notes.

Now, let's talk about how I've used, and have not used, AI for this project. I started this project after getting laid off from my job of 7 years as a software tester. My expertise and experience is not in programming or software development. While I decided everything that this app will and will not do, I used Claude to do the coding and a lot of back-end analysis needed to get rhythm and audio detection working properly. For the UI, I allowed Claude to programmatically draw simple shapes like rectangles, circles, and diamonds, using syntax available to Rust and python. These are code-only shapes that do not have asset files.

While I find the use of AI acceptable for writing code or as a productivity tool, I strongly believe that AI should have no role in creating an artistic product. This is a shout-out against generative AI used to create AI art or visual assets. Art should remain a human endeavour, a way for people to communicate messages and emotions to other humans. This app contains no AI-generated art assets, and Claude was not used for complex drawings, such as the notation staff. I used existing packages for things like that, which will be noted in the credits section. The logo was hand-drawn by my talented niece, with no AI involvement.

Embrace The Beep does not use AI within its own functionality. It uses a lot of math, does not connect to the internet, and does not have a built-in AI model. I have no interest in collecting any data from users and risk violating their privacy.

Every pattern and groove that comes with this app was manually charted by me, using the app's notation tool, with the exception of some of the flam rudiments, where the AI took it upon itself to create them while testing flam detection. I checked them against the Percussive Arts Society rudiment list to ensure they were accurate, found that they were, and decided not to manually re-notate this small group. I include this instance for the sake of transparency, as I understand that different people have different tolerances over the use of AI.

Embrace The Beep is intended to help drummers overcome their shortcomings, blind spots, and weaknesses. It is not intended to make up for them. Drumming is a discipline that requires many thousands of hours of practice to become good at, many of them spent on things like rudiments, and this app will not change that.

With all that said, thank you for reading this and I hope you will continue to follow the progress of Embrace The Beep as I push towards eventual release. My target audiences will include percussion students and drumkit users of all levels.

Drums are hard\
Music is hard\
Be kind to yourself and others\
Go practice

CJ

---

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
- **A microphone as your kit** (new, still being tested): play a
  practice pad or a snare with no electronic kit. Every hit the mic
  hears counts as a snare hit, so it suits rudiments and single-drum
  patterns.
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
sends MIDI over USB, or a microphone on a practice pad or snare. Mac,
iPhone/iPad and Android versions are next.

## Acoustic drums: where it stands (2026-11-14)

All results so far are from one player, one set of drums and one room.

- **A practice pad or a snare works in the app now** (Windows), with a
  microphone as the kit input. It's new and still being tested.
- **Practice pad:** in testing, the app caught nearly every stroke,
  including ghost notes and the grace notes of flams and drags.
- **Snare and toms:** a drum keeps ringing when the next stroke lands,
  which can hide quick strokes. Slow and medium playing is caught
  reliably. At speed, a soft stroke right after a loud one can still
  be missed.
- **Full kit:** in a first recording of a full acoustic kit, every
  single hit on every drum and cymbal was found. The hard part is
  telling *which* drum or cymbal was hit, especially when the kick lands
  at the same moment as other things. That's being worked on, and full
  kit support isn't in the app yet.
- **Still to check:** how exact the timing is, compared with an
  electronic pad.

## Coming to phones

The phone screens are laid out for every size from the small iPhone SE to
the largest Pro Max (pictures in the 2026-10-16 changelog). On a phone:

- **Practise with the phone sideways on a stand.**
- **The Groove Editor and recording go sideways too.**
- **The metronome works upright or sideways.**
- **Light and dark**, following your phone's own setting.

## Roadmap

**Next up**
- **Acoustic drums with a microphone.** One pad or drum works now (see
  "Acoustic drums: where it stands" above). Next: checking the timing,
  then telling drums and cymbals apart for a full kit.
- **Mac**, then **iPhone/iPad** and **Android**
- **A test version for a few testers** on Windows.

**Patterns**
- More common grooves by genre.
- Checking the new drag rudiments by ear and eye.

**Later**
- Polished, installable apps for all four platforms.

See [CHANGELOG.md](CHANGELOG.md) for what's changed recently.

## Feedback

Ideas and feature requests are welcome. Open an issue on this repo.
