# Teach the Machine

An interactive workbook for the image-classification tutorial in **ARCH3215 / ARCH8215 Digital Pasts** (Flinders University). Students use Google Teachable Machine in one tab and work through this page in another.

Everything is in `index.html` (logo, 3D graphics and all text are inside it). There is nothing to install or build.

## What students do

1. Enter their name, group and date.
2. Work through 13 stages, with a progress bar and an encouraging message after each one:
   - Briefing
   - Part 1: Choose your classification problem
   - Part 2: Train your first model
   - Part 3: Give it something new
   - **Side quest, the mystery tray:** train on two groups of objects, test a few third objects, and see where each one lands on a guess-versus-model chart
   - Part 4: Test generalisation (correct/incorrect is filled in automatically and tallied)
   - Part 5: Can you trick the machine?
   - Part 6: Build a better classifier (compared with the Part 4 tally)
   - Part 7: Break your classifier
   - Part 8: From webcam experiments to archaeology
   - Final reflection
   - Debrief: what they tried, how it went, and how it could be used in their own work and in the field
   - Finish: summary, take-home message and key concepts
3. Save their answers in one of three ways: print or save as PDF, copy all, or download as a text file.

## Put it on GitHub Pages

1. In this repository, open **Settings > Pages**.
2. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main**, folder **/ (root)**, and save.
3. After a minute or two the page is at `https://johnmccarthyflinders.github.io/DigitalPasts/`.

## Things to know

- **Answers stay on the student's device.** They autosave in the browser (localStorage) and are never sent anywhere. If a student changes computers or clears their browser data, the answers are lost, so remind them to download or print before they leave. On a shared computer, they can use "Clear my answers" on the last page.
- **Canvas:** link to the GitHub Pages address from a Module or Page. Embedding it may or may not work depending on your Canvas settings.
- **Teachable Machine** needs camera access and works best in Chrome or Edge on a laptop.
- **Fonts** load from Google Fonts. Offline, the page falls back to system fonts and still works.
- **Motion:** the 3D banner pauses on a still frame if the student's device has "reduce motion" turned on.

## Editing the text

All questions, instructions, encouragement messages and glossary entries are in the `CONTENT` block inside `index.html` (search for `const CONTENT`). Each question has an `id`. If you rename an id, any answers students have already saved under the old id will no longer show.
