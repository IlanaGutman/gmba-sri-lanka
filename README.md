# Team Sri Lanka - Culture and Business (Reichman GMBA, 25231)

Our team site for the course. We take one Israeli company into the Sri Lankan market and plan the first face-to-face meeting with a client. **The company is not chosen yet.**

**Live site:** https://ilanagutman.github.io/gmba-sri-lanka/ · **The pitch:** https://ilanagutman.github.io/gmba-sri-lanka/pitch/

## What is here

| Page | File | Grade part |
|---|---|---|
| Team home | `index.html` | - |
| The 4-minute pitch | `pitch/index.html` | Assignment 1 (30%), presented in class |
| The company | `company/index.html` | Assignment 1 (30%) |
| The culture | `culture/index.html` | Assignment 1 (30%) |
| The client and the roadmap | `client/index.html` | Assignment 2 (40%) |
| The meeting | `meeting/index.html` | Assignment 3 (30%) |

Each page has yellow **"To add"** boxes. A box says who fills it and what to write. When the text is in, the box becomes normal page text.

The pitch also has gold dashed fields such as **[Company]** or **[client]**. Each one is a single word or phrase to fill in once we choose the company.

## The pitch

Eight slides, about 4 minutes. Open `pitch/` and use the arrow keys or the buttons at the bottom right. Click the clock to start the talk timer: it turns orange at 4 minutes and red at 5. Every slide has **Speaker notes** with the script and timing.

| Slide | What is on it | Status |
|---|---|---|
| 1 | Title | Fill **[Company]** |
| 2 | Why Sri Lanka | Written, add the local need |
| 3 | How we chose (scoring table) | To fill |
| 4 | The company | To fill |
| 5 | The first client | To fill |
| 6 | Culture is the strategy | Written |
| 7 | The road to the meeting | Written, fill the [fields] |
| 8 | Scenario and closing line | Written |

## The design

A Sri Lankan flag theme with a fine-jewellery feel: the flag's maroon as the background, flag gold as the main colour, saffron and green for details, serif headings and gem-shaped dividers. In comparisons, Israel is shown in sapphire blue and Sri Lanka in gold. The whole theme lives in `assets/team.css`, so every page shares it.

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
- Building blocks: `.fact` cards in `.twocol`, `.flip` cards, `.timeline` with `.tstep`, `.scenario`, `.vs` strips, `.check` lists, `.notice`, `.todo`. The pitch adds `.slide` sections, `.stat` cards, a `.matrix` table, `.notes` speaker notes and `.fill` placeholders.
- Theme colours are variables at the top of `assets/team.css` (`--flag-maroon`, `--flag-gold`, `--flag-saffron`, `--flag-green`). Change colours there, not in each page.
- When you fill a `.todo` box, replace it with a normal block (`.fact` is the default). Do not leave the yellow box around finished text.
- When you fill a `.fill` placeholder, replace the whole `<span class="fill">[...]</span>` with plain text.
- After any change, update this README, the status chips on `index.html` and AI-USE.md in the same pull request.
- When a page has no open boxes, change its status chip on `index.html` from `open` or `draft` to `done`.
- Check every page at 1280px and at 390px wide before you open the pull request.

## Credit

The design system and the first draft of the culture page come from the course kit, [SoundGuyAI/RuniLectures](https://github.com/SoundGuyAI/RuniLectures), which invites students to copy it.

## Turn on the live site (repo owner, one time)

*Settings* > *Pages* > *Source: Deploy from a branch* > *Branch: main, folder: / (root)* > *Save*. The site is live after about one minute.
