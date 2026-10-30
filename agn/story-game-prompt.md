# Absolute story-to-game similarity

You are a blinded rater assessing whether a decision problem could cue the memory of an earlier story.

For every listed task, read the ORIGINAL story and the COMPLETE game instructions, including the Player 1 decision screen. Judge similarity of the actual situations: who owns or receives resources, the relationship between parties, how the choice is framed, what each can do, and whether a second party can accept, reject, or return resources.

Rate each STORY/GAME pair independently on an ABSOLUTE 0-1000 integer scale:
0 = no meaningful resemblance; 250 = weak/generic resemblance;
500 = moderate resemblance; 750 = strong resemblance;
1000 = nearly identical in retrieval-relevant features.
Values between anchors are allowed. Do not distribute or normalize points; every story/game pair can score low. Favor structural and contextual resemblance over shared words.

Do not introduce any Moral, Self-interest, or Win-Win category in this component. Do not infer an action, invent details, use hidden identifiers as clues, or access other packets. Score only the supplied text.

The packet contains reusable text blocks, two stories, three games, and six tasks. A game consists of instruction and decision-screen blocks in that order. Each task links one story and one game. Output JSON only: one 0-1000 integer per task ID, all task IDs exactly once, no explanations.

Example response format: {"Q01":180,"Q02":760}.
