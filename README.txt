JOURNAL WRITING


Three aesthetic, scrapbook-style journals — Dhanashri's (soft lavender), Pratiksha's (warm cream) and Siddhesh's (soft rose) — hosted from one repository on GitHub Pages, sharing one engine while keeping their stories, themes and identities separate.

No server, no database: each story is a small JSON file committed to this repo, and the private editor publishes straight to GitHub from the browser. Public pages only ever read.


LIVE

Dhanashri : https://laxman-sidhu.github.io/Journal-Writing/Dhanashri-Journal/
Pratiksha : https://laxman-sidhu.github.io/Journal-Writing/Pratiksha-Journal/
Siddhesh  : https://laxman-sidhu.github.io/Journal-Writing/Siddhesh-Journal/


STRUCTURE

assets/              shared engine (edit once, all three clients update): core.js, style.css, backgrounds/, PROJECT.txt, Setup.txt
Dhanashri-Journal/   client A (lavender): index.html, story.html, admin.html, data/
Pratiksha-Journal/   client B (cream):    index.html, story.html, admin.html, data/
Siddhesh-Journal/    client C (rose):     index.html, story.html, admin.html, data/

The only client-specific code is a small window.JOURNAL_CLIENT block at the top of each client's pages (its title, theme and own data folder) plus a data-client attribute that selects its colour theme. Every publish is routed through that client's own data folder, so one editor can never write into another's stories.


DOCS

Full explainer: assets/PROJECT.txt
Setup, hosting and tokens: assets/Setup.txt


FEATURES

Freeform canvas with text (20 fonts, alignment, fill, rotation, and inline bold/italic/underline on a selection), photos (move, resize, rotate, crop, caption; looks: card, plain with transparency preserved, frame, border; an independent shadow toggle; and caption font/size/colour), stickers, upload-your-own image stickers, washi tape, doodles, layering, multi-page stories, per-page backgrounds, cover picker, autosave, drafts, and PDF export.
