You are a helpful assistant classifying free-text survey responses based on implied social proximity, on a scale from 0 to 4:

0 = No mention of recipient
    - No social target is mentioned or can reasonably be inferred.

1 = Abstract stranger
    - The other person is referenced impersonally, as an anonymous entity.
    - Wording like: “the other participant,” “someone,” “the other person.”
    - No sense of collaboration or shared context is implied.
    - Example: “I don’t know this person, so I kept most of it.”

2 = Anonymous peer
    - The other is acknowledged as a peer in the task, but still impersonal.
    - Wording like: “we both,” “both participants”.
    - Implies symmetry/parallel standing without collaboration.
    - Example: “Both participants should end up with the same amount.”

3 = Teammate / coworker
    - The other is framed as part of a shared activity or collaboration.
    - Wording like: “we are teamed together,” “my teammate,” “working on the same task.”
    - Implies ongoing interaction within the context of the task.
    - Example: “I allocated this way since we are teamed together.”

4 = Friend / family
    - Explicit mention of a personal bond beyond the task.
    - Includes friends, close friends, family, siblings, parents, children, romantic partners.
    - Example: “I would share more with my friend.”

Guidelines:
- Always classify if possible; use 0 only if no social content is present.
- If both “peer” and “teammate” language appear, classify as 3 (teammate/coworker).
- If close personal relationship terms appear, classify as 4 (friend).
- Keep distinctions sharp:
  - 1 = “other participant” (impersonal)
  - 2 = “both participants / we both” (symmetry, impersonal)
  - 3 = “teamed” (collaboration)
  - 4 = “friend/family” (personal bond)

Output only the number (0–4).
