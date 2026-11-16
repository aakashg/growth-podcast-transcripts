# Guide for agents (Claude Code, Codex, Cursor)

This repo is every episode of The Growth Podcast with Aakash Gupta, one markdown file per episode.

## Layout

- `index.json` and `index.csv`: one row per episode. Read these first. Fields: `title`, `subtitle`, `date`, `guests`,
  `substack_url`, `youtube_url`, `duration`, `word_count`, `speaker_names`, `file`.
- `episodes/<date>-<slug>.md`: the transcript. YAML frontmatter (same fields), then speaker turns:

  ```
  **Guest Name** (00:12:31)

  What they said...
  ```

  The timestamp is when the turn starts in the aired episode. To link a quote, append `&t=<seconds>s` to `youtube_url`.

## How to work with it

- A full episode runs 8,000 to 20,000 words. Don't load the whole archive into context. Search, then read.
- Search with grep or ripgrep: `rg -i "north star metric" episodes/ -l` finds episodes, `rg -i -B2 -A8 "..."` shows the passage
  and the speaker line above it.
- Filter by guest or date with `index.csv` before reading files.
- Most episodes open with a short teaser of clips from later in the episode, then the host's intro.

## Accuracy

- Transcripts are machine-made from the aired audio. Names, companies and numbers can be misheard. Check the audio
  (the `youtube_url` at the timestamp) before you publish a quote.
- `speaker_names: "substack"` means names came from the episode's speaker map. `"inferred"` means they were set from
  the title and the host's intro, so double-check who is talking on short turns.
- Sponsor reads are marked with `<!-- sponsor -->` on the line above where they were detected (about 1,000 paragraphs).
  Detection is best effort: a few mid-roll reads that name no URL or code are unmarked, so skip host monologues about a
  product that has nothing to do with the episode.
- Attribute every claim to the person who said it, with the episode and timestamp. Never invent a quote.

## License

See `LICENSE`. Build anything, including commercial products; credit and link back; don't re-host the raw files as a
dataset; don't present guests as endorsing your product or imitate their voices.
