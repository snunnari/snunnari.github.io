# Blinded real-world vignette similarity rating instructions

You are an independent rater in a blinded exercise about similarity between decision situations and real-world situations.

The packet defines reusable text blocks, targets, real-world vignettes, vignette sets, and tasks. A target consists of the text blocks listed for that target, concatenated in the listed order. Each task pairs one target with one vignette set.

For each task, read the target's complete ordered text and every real-world vignette in the assigned set before allocating points. Allocate exactly **1,000 nonnegative integer points** across all vignettes in that set.

For each vignette, ask: **How similar is the target situation to this real-world situation?** Give more points to vignettes that the target resembles more closely as a whole. Interpret the points as a relative similarity allocation within the set presented for that task.

Focus on the overall decision situation faced by the focal decision-maker: the roles of the parties, their relationship and interaction context, the structure and nature of the choice, and the considerations that the situation makes relevant. Compare the target to the real-world situation described in each vignette rather than trying to assign the target to an abstract category.

Do not base the rating on the action you predict the focal decision-maker will take, whether a particular action is morally or strategically correct, or a justification you invent after the fact. Do not reward mere shared wording or superficial lexical overlap. Judge semantic similarity between the target situation and each real-world vignette as presented.

Use only the target and vignette texts provided in the packet. Do not infer anything from neutral identifiers, their order, the number of vignettes in a set, overlaps between sets, or possible hidden source labels or categories. Do not use outside knowledge, other packets, other agents' responses, or any classification data. There is no required minimum number of vignettes that must receive positive points.

Complete every task in the packet. Each task is independent and must sum to exactly 1,000 points.

Return compact JSON only. Each top-level key is a task ID and its value maps the relevant vignette IDs to points:

```json
{"Q01":{"V01":300,"V02":500,"V03":200}}
```

Requirements:

- Include every task identifier shown in the packet exactly once.
- Within each task, include every vignette identifier in the task's vignette set exactly once.
- Use nonnegative integers only.
- Make the points in every task sum to exactly 1,000.
- Do not include explanations or markdown outside the JSON object.

Before answering, verify the task count, vignette identifiers, integer points, and 1,000-point total for every task.
