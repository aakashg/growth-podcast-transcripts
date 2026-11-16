---
name: ask-the-pod
description: Answer any product, growth, AI PM or career question from what Growth Podcast guests actually said, with the guest, episode and a YouTube link at the exact second. Use on "what do guests say about X", "ask the pod", "who on the pod talked about X", or any PM question asked inside this repo.
---

# Ask the Growth Podcast

Answer from the transcripts in `episodes/`, never from memory.

1. Turn the question into 3 to 6 search terms, including the plain words a guest would say out loud
   ("pricing page", "raise prices", "willingness to pay"), not only the jargon.
2. Find the episodes: `rg -i -l -e "term one" -e "term two" episodes/ | head -40`. Use `index.csv` to filter by guest or year.
3. Read the passages: `rg -i -B3 -A12 "term" episodes/<file>.md`. The `**Name** (hh:mm:ss)` line above a passage tells you
   who said it and when.
4. Keep only passages that answer the question. Prefer guests who did the thing (ran it, built it, hired for it) over
   guests talking in general.
5. Answer in this shape:
   - One line: the answer, in plain words.
   - 3 to 5 guest takes. For each: the guest and their role from the episode, the point in one or two sentences, one short
     quote copied exactly from the transcript, and the link `youtube_url&t=<seconds>s`.
   - Where guests disagree, say so and show both sides.
   - Close with the one episode to watch first and why.

Rules: copy quotes character for character from the file. Never put words in a guest's mouth. If the archive doesn't
cover the question, say which nearby topics it does cover.
