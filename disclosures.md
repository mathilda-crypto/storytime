# Disclosures

## What was developed for this Hackathon

Storytime and its core workflow were newly developed during the UGREEN Hackathon 2026. Principal functionality developed for the Hackathon:

- The journaling workflow: entries by text, voice note or handwriting photo, saved as dated Markdown files with written and happened dates.
- The three modes (Listen, Explore, Act or create), tones, plot-twist rules and inner-critic method.
- Programmes with a chosen time frame, one main focus, experiments, check-ins and a text map.
- "Talk with my diary" and "Talk with my coach" with recorded-versus-interpretation labelling.
- The Career and freelance application kit: achievement bank, requirement matching, drafts without invented facts.
- Privacy, integrity and support rules, and the quote list.

The idea draws on the author's earlier notes on journaling and coaching; no previously developed Skill or submission material is reused.

## Third-party components and open-source libraries

This package contains only Markdown files written for this Skill. It bundles no third-party code, libraries, fonts, images or data.

The Skill relies at run time on UGREEN NAS capabilities and registered experts (`file-agent`, `document-agent`, `photo-agent`, `knowledge-agent`), provided by UGREEN under its own terms. They are not included in this package. This Skill is not an official UGREEN Skill.

Quotations in [Quotes](quotes.md) are short, attributed lines; all but one come from works in the public domain. "LinkedIn" is named only to describe where the user may copy their own text; it is a trademark of its owner and this Skill is not affiliated with it.

## AI tools used to build it

| Tool | Source | Principal use |
|---|---|---|
| UGOS Skill Creation Tool (`uliya-skill-kit`) | UGREEN, Hackathon Starter Kit | Capability catalog lookup, Skill format rules and static checks |
| Claude (Anthropic) | claude.ai | Structuring the author's notes, feasibility check against the catalog, concept mockup, drafting `SKILL.md` and references, running the static checker |

## Data handling

- The Skill reads only the journal folder and application folders the user names, and only through NAS experts.
- It never asks for credentials and never contacts outside services.
- It writes only after the user chooses to save and the platform approves.
- All examples in this package are synthetic; it contains no personal data, credentials or keys.
