# The Growth Podcast: every transcript

Every episode of The Growth Podcast with Aakash Gupta, as markdown, free to build on.

**164 episodes. 215 hours. 2.27 million words. 150 guests.** August 2024 to November 2026.

Each line carries the speaker and the second it was said, so anything you build can link straight back to the guest
saying it.

## Start in two minutes

```bash
git clone https://github.com/aakashg/growth-podcast-transcripts
cd growth-podcast-transcripts
claude
```

Then ask:

```
/ask-the-pod how should I price a new AI feature?
```

You get the answer, the guests who've done it, an exact quote from each, and a YouTube link that starts at the moment
they said it.

**No download:** add the free MCP server and search the show from any Claude Code session.

```bash
claude mcp add --transport http growth-podcast https://growth-podcast-mcp.aakashg.workers.dev/mcp
```

## What's inside

| Path | What it is |
|---|---|
| `episodes/<date>-<slug>.md` | One episode: YAML frontmatter, then the conversation turn by turn |
| `index.csv`, `index.json` | One row per episode: title, date, guests, links, length, word count |
| `AGENTS.md` | How the files are laid out, for Claude Code, Codex and Cursor |
| `.claude/skills/ask-the-pod` | Answers any PM question from the guests, with quotes and timestamps |
| `.claude/skills/pm-interview-coach` | Mock interviews graded against what interviewers on the show said they look for |

A turn looks like this:

```markdown
**Stephanie Leue** (00:00:58)

If someone's telling you we tried it, it didn't work, don't stop there. Like think about 10 different ways.
```

Sponsor reads are marked with `<!-- sponsor -->` on the line above wherever they were detected, so you can strip them.

## Things to build

An X bot that answers with a guest quote. A "which episode should I watch" recommender. A library of every framework
taught on the show. A tool tracker showing what AI tools guests used in 2024 against 2026. Interview flashcards. A
debate generator. A game.

## The challenge

Build something on this repo and post it in [Discussions → Show and tell](../../discussions/categories/show-and-tell).
Five winners each get a year of paid [Product Growth](https://www.news.aakashg.com) and a 15-minute call with Aakash.
Details and the deadline: [the launch post](https://www.news.aakashg.com/p/pod-transcripts-github).

## How the transcripts were made

From the aired audio of each episode, the same transcript that sits on its Substack page, so nothing here is off-air.
131 episodes carry speaker names from the episode's speaker map, 29 had names set from the title and the host's intro
and were checked by hand, and 4 come from the YouTube caption track with speakers not separated (`speaker_names` in the
frontmatter says which). Transcripts are machine-made: check a quote against the audio before you publish it.

## License

Build anything, including products you charge for. Credit The Growth Podcast and link back. Don't re-host the raw files
as a dataset, present a guest as endorsing your product, or imitate anyone's voice. Full terms in [`LICENSE`](LICENSE).

Inspired by Lenny Rachitsky's transcript release and everything his readers built on it.
