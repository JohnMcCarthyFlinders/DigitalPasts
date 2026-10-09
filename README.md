# Digital Pasts: Machine Learning

A one-hour, single-player interactive workbook for the image-classification exercise in **ARCH3215 / ARCH8215 Digital Pasts** (Flinders University). It is written for anyone working with evidence of the past: archaeologists, palaeontologists, curators and heritage practitioners. Students work through it at home with Google Teachable Machine open in a second tab.

Live page: https://johnmccarthyflinders.github.io/DigitalPasts/

Everything is in `index.html` (logo, 3D graphics, illustrations and all text are inside it). There is nothing to install or build.

## What students do

Students enter their name and date, then work through 11 stages with a progress bar and a short encouraging message after each one:

1. Briefing
2. Part 1: Choose your classification problem
3. Part 2: Train your first model
4. Part 3: Give it something new
5. **Side quest, the mystery tray:** train on two groups of objects, test a few third objects, and see where each lands on a guess-versus-model chart
6. Part 4: Test generalisation ("Correct?" fills itself in and is tallied)
7. Part 5: Can you trick the machine?
8. Part 6: Build a better classifier (compared with the Part 4 tally)
9. Part 7: Break your classifier
10. Part 8: From webcam to the deep past (three challenges: a museum ceramics collection, field fragments, and fossil localities)
11. Finish: summary, quiz score, take-home message and key concepts

The question mix:

- **12 multiple-choice questions.** These reveal the answer and an explanation as soon as a student picks. The first answer is locked in, so the quiz score reflects first attempts.
- **3 quick polls** for predictions, such as "how well do you think it will do?".
- **8 short written answers,** each with a word limit between 40 and 100 words and a live counter. Typing stops at the limit.
- **Result tables** for recording what the model predicted.

At the end students can print or save a PDF, copy all their answers, or download them as a text file. The export includes their quiz score.

## Things to know

- **Answers stay on the student's device.** They autosave in the browser and are never sent anywhere. Clearing browser data or switching computers loses them, so students should download or print before they finish. "Clear my answers" on the last page wipes them from a shared computer.
- **The answers are in the page source.** That suits a formative exercise but not a graded quiz.
- **Teachable Machine** needs a webcam and works best in Chrome or Edge on a laptop.
- **Fonts** load from Google Fonts. Offline, the page falls back to system fonts and still works.
- **Motion:** the 3D banner shows a still frame if the device has "reduce motion" turned on.

## Editing the text

Questions, options, explanations, word limits and glossary entries are all in the `CONTENT` block inside `index.html` (search for `const CONTENT`).

- **Multiple-choice questions:** `a` is the index of the correct option. A short block after `CONTENT` moves each correct answer to a set position (the `target` list), so the correct letters are spread across A to D.
- **Word limits:** these are the `cap` values on each `q` block.
- **Question ids:** renaming an `id` hides any answers students have already saved under the old one.
