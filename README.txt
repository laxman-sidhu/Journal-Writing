JOURNAL WRITING


Three aesthetic, scrapbook-style journals — Dhanashri's (soft lavender), Pratiksha's (warm cream) and Siddhesh's (rose pink) — hosted from one repository on GitHub Pages, sharing one engine while keeping their stories, themes and identities separate.

No server, no database: each story is a small JSON file committed to this repo, and the private editor publishes straight to GitHub from the browser. Public pages only ever read.


LIVE

Dhanashri : https://laxman-sidhu.github.io/Journal-Writing/Dhanashri-Journal/
Pratiksha : https://laxman-sidhu.github.io/Journal-Writing/Pratiksha-Journal/
Siddhesh  : https://laxman-sidhu.github.io/Journal-Writing/Siddhesh-Journal/


STRUCTURE

assets/              shared engine (edit once, all three clients update): core.js, style.css, backgrounds/ (bg01-bg28), PROJECT.txt, Setup.txt
Dhanashri-Journal/   client A (lavender): index.html, story.html, admin.html, data/
Pratiksha-Journal/   client B (cream):    index.html, story.html, admin.html, data/
Siddhesh-Journal/    client C (rose pink):index.html, story.html, admin.html, data/

The only client-specific code is a small window.JOURNAL_CLIENT block at the top of each client's pages (its title, theme and own data folder) plus a data-client attribute that selects its colour theme. Every publish is routed through that client's own data folder, so one editor can never write into another's stories.


DOCS

Full explainer: assets/PROJECT.txt
Setup, hosting and tokens: assets/Setup.txt


FEATURES

A fixed Word-style ribbon at the top of the editor: document actions, an Insert / Edit / Arrange / Pages command row, and a contextual formatting row whose height never changes, so the canvas never jumps as you select things.

Freeform canvas with text boxes that behave like Word's — click once to select and drag from anywhere in the box, double-click to type (which holds the box still), click the empty part of the box to stop typing and move it again, resize from all eight corners and walls, and move a box past the page edge and still see it. Around forty fonts, size, bold / italic / underline / strikethrough, bulleted and numbered lists, four alignments, line spacing, text colour, box fill, and free rotation. Font, size and colour all work on a selection as well as the whole box: highlight a word or a line and only that changes. Dragging snaps to the page centre and to other items' edges, with guide lines (hold Alt to place freely). Arrow keys nudge, Ctrl+D duplicates, Delete removes, Escape backs out.

Videos by direct link — a Cloudinary upload, or any .mp4 or .webm served over https. They play in the browser's own player, so a page stays clean with no branding, channel name or share buttons; YouTube and Vimeo links are refused for exactly that reason. Only a thumbnail you choose is saved into the story, so the file stays small however long the clip is. The page shows that thumbnail with a play badge and swaps in the player on click, with full controls. Several clips can share a page, and starting one stops the others. Videos take the same Plain or Card look as photos, with a caption. The PDF export keeps the thumbnail and its play badge, so a printed page still reads as a video rather than a photo.

Photos (move, resize, rotate, crop, caption; looks: plain with transparency preserved, frame, border; an independent shadow toggle; adjustable corner rounding; and caption font/size/colour), stickers, upload-your-own image stickers, washi tape, doodles, layering, multi-page stories, 28 per-page backgrounds, cover picker, autosave, drafts, and PDF export.
