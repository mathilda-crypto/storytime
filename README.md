# Storytime – Connect your dreams

A private journal and personal coach that runs as an AI Skill on the **UGREEN AI NAS**. Write, speak or photograph an entry, choose how you want help – **Listen**, **Explore**, or **Act or create** – follow a self-paced programme with your own goal, and turn real experience into practical results such as a job application kit. Everything stays on your own NAS.

Entry for the UGREEN Hackathon 2026 · Track: *Understand Your Life*.

<img src="docs/prototype-welcome.png" width="300" alt="Prototype – welcome"> <img src="docs/prototype-checkin.png" width="300" alt="Prototype – check-in">

## What's in this repository

| Folder | What it is |
|---|---|
| [`skill/storytime/`](skill/storytime/) | The Skill package for UGREEN AI NAS: `SKILL.md` plus 12 reference files. Follows the Uliya Skill Development Standard and passes the UGOS Skill Creation Tool's static checker. |
| [`prototype/`](prototype/) | A clickable browser prototype of the experience. One HTML file, no install, no server. |
| [`docs/`](docs/) | Round 1 proposal (PDF), Devpost story, concept mockup screens and prototype screenshots. |

## Try the prototype

Open `prototype/index.html` in any modern browser – or enable GitHub Pages for this repository and open `/prototype/`.

- Click **Load sample data to explore** to see a programme in progress, or start fresh.
- Everything is stored in your browser's local storage only. **Settings → Delete everything** removes it.

What the prototype shows:

- **Write** – a **Bigger** button opens a full-screen writing space with a word count (**Smaller**, **Done** or Esc brings it back); entries save automatically (tick "Don't save this" for off-the-record, or "Extra private" for the vault), modes, depth controls ("Just save this", "Don't analyse this", "Stop here"), inner-critic reframing, plot-twist invitations (never on heavy topics), and a support message if someone may be at risk.
- **Check-in** – day X of Y, a thought for the day, the current experiment, background journeys, pause / skip / go lighter.
- **Diary and coach** – answers with their source entries, labelled *Recorded* or *My reading*, with missing dates and gaps named.
- **My notes** – browse every entry by month, filter by journey or word, open a note, step to earlier or later notes, write a follow-up.
- **Map** – the programme as a week grid with reviews and milestones; tap any day to open its notes and check-in, or write about that day.
- **All time** – every programme you have run (30 days, 45 days, open-ended…) on a year calendar coloured by programme, with days you wrote marked; open any past programme's map or its notes. Finish a programme or start a new one at any time – nothing is lost.
- **Goals** – one objective per journey (main focus first), milestones with target dates, tap-to-add milestone ideas, progress bars; the next milestone shows in the check-in and milestone dates on the map.
- **Career application kit** (only when the Career and freelance journey is chosen) – achievement bank, job-ad matching with honest gaps, CV draft with bracketed gaps, downloadable as Markdown.
- **Share with care** – selection, privacy preview (vault never shared), Markdown export.
- **Menu**, **Where was I?** and **Back** – jump anywhere, resume, and go back (the browser back button works too).

> In the prototype, replies are **rule-based placeholders** so it works offline without any AI. On the NAS, the Skill delegates to UGREEN's registered experts (document, knowledge, photo and file agents) and the NAS models write the replies.

## The Skill on UGREEN AI NAS

`skill/storytime/SKILL.md` orchestrates the NAS experts:

| Step | Expert |
|---|---|
| Read settings and programme, save entries, copy drafts | `file-agent` (`ug-filesystem`, `ug-filemgr`) |
| Transcribe voice notes | `knowledge-agent` (`ug-knowledge`) |
| Read handwriting photos, find photos, make albums | `photo-agent` (`ug-photo`) |
| Talk with my diary / coach with citations, read job ads, write drafts | `document-agent` (`ug-document`) |

Every write needs platform approval. No outside services are contacted. See [`references/nas-capabilities.md`](skill/storytime/references/nas-capabilities.md) and [`references/limitations-and-roadmap.md`](skill/storytime/references/limitations-and-roadmap.md).

To package the Skill for upload, zip the `skill/storytime` folder so that `storytime/SKILL.md` is at the top level of the ZIP.

## Principles

- **Private by default** – plain Markdown files in your own folder; nothing is shared without a preview.
- **Honest** – facts come only from your entries, with sources; interpretations are labelled; achievements and family facts are never invented.
- **You control the depth** – reflection is never compulsory.
- **Coach, not therapy** – clear support boundaries.

## Roadmap

Prompts by email, notification or calendar invite · encrypted vault · iPad handwriting import · family book and calendar export · dedicated outputs for every journey · a companion app based on the concept mockup in [`docs/mockup/`](docs/mockup/).

## Credits

Created by Mathilda Klingberg. Built with the UGREEN Skill Developer Package (UGOS Skill Creation Tool) and Claude by Anthropic as an AI assistant for structuring, drafting and checks. Quotes in the prototype are short, attributed lines, mostly from public-domain works.

## Licence

No licence has been chosen yet; until one is added, all rights are reserved by the author.
