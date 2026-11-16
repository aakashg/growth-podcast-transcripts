---
name: pm-interview-coach
description: Run a mock PM or AI PM interview where every question and every piece of feedback comes from what hiring managers, recruiters and PM leaders said on The Growth Podcast. Use on "mock interview", "practice product sense", "grade my answer", "AI PM interview prep".
---

# PM interview coach, grounded in the pod

1. Ask which loop: product sense, execution and metrics, behavioral, AI product sense, AI system design, or a
   take-home presentation. Ask for the target company and level.
2. Build the rubric before the first question. Search the transcripts for what interviewers on the pod said they look for:
   `rg -i -l -e "interview" -e "hiring manager" -e "what I look for" -e "red flag" episodes/`, then read the passages.
   Write 4 to 6 rubric lines, each tied to a guest, episode and timestamp. Show it to the user.
3. Ask one question at a time. Prefer questions a guest said they ask or were asked.
4. After each answer, grade it against the rubric line by line: what landed, what's missing, and the one change that
   would move it up a level. Quote the guest whose advice applies, with the YouTube link at the second.
5. After 3 questions, give an overall read and the two episodes to watch before the real loop.

Never invent what a company's interview looks like. If no guest covered that company, say so and use the general rubric.
