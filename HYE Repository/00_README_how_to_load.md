# HYE Repository, how to use this

A repository of the Hello You Experiment X/Twitter corpus (1215 posts, 2025-07-07 to 2026-08-07), structured for bulk assessment in NotebookLM or any AI notebook rather than post-by-post upload.

Every post in the archive has now been read cold. All 1215 of 1215 carry a no-memory interpretation.

## Files
- master_index.csv, one row per post, id, timestamp, text, emoji, media files, OCR'd GIF caption, signals, interpretation, status, URL.
- posts_YYYY-MM.md, the corpus split into monthly documents (the NotebookLM sources). Each post shows paired media with its on-screen GIF caption, emoji decode, full text, signals, and interpretation.
- 00_corpus_overview.md, context source to load alongside the monthly docs.

## Interpretation method (cold wild-type reads)
Each post was handed to a fresh model with no prior context and this exact unoptimized prompt.

> "Interpret this meaningfully and deeply. What does it mean, what is the author trying to say, and how does it translate to current culture and generations? Do not use memory for the interpretations. It ideally is an incognito mode translation but no worries if not."

The GIF is included because text, emoji, and GIF are one artifact, a codon. A frame from every GIF was run through OCR to recover its on-screen words, and those captions are embedded per post. GIF captions recovered, 314 of 632 GIF posts.

Reply handling. Replies to the author's own posts were read with the earlier post fed in as context. Replies to other people were read as the author striking sparks off an absent prompt, since the original posts are not in the archive. The handle and rough domain of who was replied to were included where known.

## Load into NotebookLM
1. New notebook, for example "Hello You Experiment".
2. Add sources, Upload, 00_corpus_overview.md and each posts_YYYY-MM.md (12 monthly docs, under the source limit). Optionally add master_index.csv.
3. Ask macro questions, for example recurring beliefs and how they converge, how work, meaning, identity, and mortality shift month over month, or where the cold reads agree.

## Corpus by month
- 2025-07: 4 posts
- 2025-10: 13 posts
- 2025-11: 288 posts
- 2025-12: 30 posts
- 2026-01: 212 posts
- 2026-02: 2 posts
- 2026-03: 138 posts
- 2026-04: 102 posts
- 2026-05: 159 posts
- 2026-06: 137 posts
- 2026-07: 88 posts
- 2026-08: 42 posts
