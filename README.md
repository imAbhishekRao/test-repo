# Français on Tips — media

Audio, images and passage text for the mock tests. Served to the site through
jsDelivr, which reads this repository directly — there is nothing to deploy.

**This repository is public.** That is a requirement of jsDelivr. Nothing secret
belongs here: correct answers and login codes live in the database and the
content sheet, never in these files.

## Adding a file

On github.com: open the folder → **Add file → Upload files** → drag it in →
**Commit changes**. It is live within a minute or two.

Then put the short path into the content sheet — `audio/l02-s1.mp3`, not the
full URL — and publish from the Content page.

## Layout

    audio/       .mp3 recordings, one per listening document
    images/      option pictures
    passages/    reading texts, Markdown

## Naming

Audio and passages: `l03-s1.mp3`, `r04-s1.md` — test id, then stimulus id.

**Option images must be opaque:** `l03-q07-1.jpg` through `-4.jpg`. A
descriptive name like `gare.jpg` appears in the page source before the candidate
answers and gives the question away — the importer rejects those. Do not let the
trailing number track the option letter either; if `-1` is always the right
answer, that becomes learnable.

## Replacing a file

jsDelivr caches an existing path for up to about 12 hours. To change a
recording, upload it under a new name (`l03-s1-v2.mp3`) and update the sheet.
That is also safer: a file cannot change underneath someone who is mid-test.

## Passages

Plain Markdown — one `#` heading, then paragraphs separated by blank lines.
That is all the renderer handles, on purpose. Save as UTF-8 so accents survive;
the GitHub editor does this by default.
