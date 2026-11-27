# Team Sri Lanka - Culture and Business (Reichman GMBA, 25231)

Our team site for the course. We take one Israeli company into the Sri Lankan market and plan the first face-to-face meeting with a client.

**Live site:** https://ilanagutman.github.io/gmba-sri-lanka/ (works after GitHub Pages is turned on, see the bottom of this file)

## What is here

| Page | File | Grade part |
|---|---|---|
| Team home | `index.html` | - |
| The company | `company/index.html` | Assignment 1 (30%) |
| The culture | `culture/index.html` | Assignment 1 (30%) |
| The client and the roadmap | `client/index.html` | Assignment 2 (40%) |
| The meeting | `meeting/index.html` | Assignment 3 (30%) |

Each page has yellow **"To add"** boxes. A box says who fills it and what to write. When the text is in, the box becomes normal page text.

## How to add your part (no code needed)

**A. Send text.** Go to *Issues* > *New issue* > *Add content*. Paste your text and say which page and which box. A teammate or an AI agent puts it on the page.

**B. Edit on GitHub.** Open the page file, click the pencil, change the text, then choose *Create a new branch for this commit and start a pull request*.

**C. Use your AI agent** (Claude Code, Codex, Cursor or another). Give it this brief:

> Work in https://github.com/IlanaGutman/gmba-sri-lanka. Read README.md first. Fill the "To add" box "[BOX]" on the page [PAGE] with the text below. Keep the design system in `assets/`. Every claim gets a numbered source marker and a line with a URL in the Sources section of that page. Write tendencies, not verdicts about a whole nation. Work on a new branch, open a pull request, and stop there. Add one line to AI-USE.md that says what you did.
>
> [YOUR TEXT OR YOUR REQUEST]

## Rules (from the course kit)

1. **A source for every claim.** A number on the page, a link in the Sources list.
2. **Tendencies, not verdicts.** "Meetings often start with tea" plus a source. Never "Sri Lankans are...".
3. **Invented dialogue gets the label "illustrative scenario".**
4. **AI use is written down** in [AI-USE.md](AI-USE.md). The syllabus requires it in every hand-in.
5. **A person reads every pull request** before it is merged.
6. **This repo is public.** No private notes, no phone numbers, no names of real contacts without their consent.

## For the agent that edits this site

- Plain HTML, CSS and JS. No build step, no framework. A page must open from disk.
- `assets/style.css` and `assets/engine.js` come from the course kit. Do not change them. Put team additions in `assets/team.css`.
- Building blocks: `.fact` cards in `.twocol`, `.flip` cards, `.timeline` with `.tstep`, `.scenario`, `.vs` strips, `.check` lists, `.notice`, `.todo`.
- When you fill a `.todo` box, replace it with a normal block (`.fact` is the default). Do not leave the yellow box around finished text.
- When a page has no open boxes, change its status chip on `index.html` from `open` or `draft` to `done`.
- Check every page at 1280px and at 390px wide before you open the pull request.

## Credit

The design system and the first draft of the culture page come from the course kit, [SoundGuyAI/RuniLectures](https://github.com/SoundGuyAI/RuniLectures), which invites students to copy it.

## Turn on the live site (repo owner, one time)

*Settings* > *Pages* > *Source: Deploy from a branch* > *Branch: main, folder: / (root)* > *Save*. The site is live after about one minute.
