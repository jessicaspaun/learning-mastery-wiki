# Testing a Codex learning coach

[Mastery research](index.md) · [Wiki home](../README.md) · [Codex coaching playbook](../codex-coach.md)

A learning coach has two outcomes to check. **Coaching quality** is whether the response identifies a reasonable task, uses the available evidence, and gives help that fits the learner’s request. **Learning** is what the learner can do later under the intended conditions. Automated conversation tests can evaluate parts of coaching quality. A practice trial with delayed and fresh tasks is needed to evaluate learning.

## Read AI studies by the outcome they measured

| Study | What the study measured | What it suggests for the coach |
| --- | --- | --- |
| Bastani et al. randomized high-school math field experiment | Performance during assisted work and a later unaided assessment. General-purpose access improved practice performance and the group later scored lower independently. The teacher-designed tutor mitigated the drop. [Study](https://doi.org/10.1073/pnas.2422633122) | Check later independent math, even when the practice attempt succeeds. |
| Kestin et al. randomized crossover college physics trial | Posttests following lessons. A specially designed AI tutor group scored higher on those tests than the in-class active learning group. [Study](https://pmc.ncbi.nlm.nih.gov/articles/PMC12179260/) | Compare well-designed teaching formats in the target context and include later tests before making a retention claim. |
| Tutor CoPilot field experiment | Topic mastery in a K–12 tutoring program. AI suggestions were offered to human tutors, and mastery in the program rose by four percentage points overall in the preprint. [Working paper](https://arxiv.org/abs/2410.03017) | A human tutor deciding how to use a suggestion is a distinct coaching model. Record who makes feedback decisions. |
| Heickal and Lan introductory Python study | Completion and convergence on lab submissions. Natural-language hints helped on these outcomes. Generated test cases varied in usefulness with validity. [Conference workshop paper](https://proceedings.mlr.press/v339/heickal26a.html) | Run generated test cases when possible and track whether the result measures the intended behavior. |
| Randomized introductory programming trial on prompting instruction | Learning-oriented prompting improved in all four instructional conditions and was still evident at six weeks. The conditions did not differ on final exam performance. [Preprint](https://arxiv.org/abs/2602.16033) | Measure prompting behavior and the target programming capability separately. |
| Shen and Tamkin programming experiment | Learning a new asynchronous library. Access to AI in the experiment was associated with worse performance on a subsequent individual skills check, including code reading and debugging. [Preprint](https://arxiv.org/abs/2601.20245) | Check reasoning and diagnosis, as well as whether the code works. |

A November 2026 Stanford SCALE evidence review found that tool design and delivery can shape outcomes in K–12 settings and identified gaps concerning lasting effects and which features matter. Results in those settings are indirect evidence for an adult Codex coaching skill. [Walker et al., November 2026 review](https://scale.stanford.edu/ai/evidence-base-review/evidence-base-ai-k12-november-review)

## Evaluate the coach on realistic conversations

| Test case | What the coach should do | What the evaluator can inspect |
| --- | --- | --- |
| A novice cannot start a small program | Offer a short example or partial exercise, then ask for a prediction or completion | The response uses the user’s level and gives them a concrete action |
| A user explicitly asks for a complete explanation | Give the explanation and offer a fresh task if useful | The response honors the request and keeps any exercise distinct |
| A learner succeeds only after a hint | Record the level of help and offer a similar task with less support | The response characterizes the assisted result accurately |
| A learner describes a new plateau without an example | Ask for one informative attempt or suggest a small diagnostic | The coach presents an explanation as a hypothesis until it has evidence |
| A guitarist asks about buzz but provides no audio | Offer a reliable self-check or request a short recording or description | The response states what it observed and avoids claiming to hear the instrument |
| A soccer player practices alone | Select a solo exercise and describe what a later live check would measure | The coach can distinguish ball control from selecting a pass against defenders |
| A learner’s real work allows reference material | Agree on tools for the check and ask for independent decisions and verification | The evaluator can tell which supports were permitted |
| The learner’s attempt exposes an error in the coach’s answer key | Correct the key and re-evaluate the attempt | The coach prioritizes observable evidence and preserves the learner’s progress |

Use prompts at different experience levels, with different amounts of time and access to equipment. Give the evaluator an example of a good next action and acceptable alternatives. For math, score solution and rationale accuracy. For programming, check generated examples and edge cases by running them. For writing, apply the intended genre and audience rubric. For physical and musical goals, check that observations come from available recordings, coach notes, scores, or the learner’s report.

## Check session boundaries and handoffs

Use the [session protocol](../session-protocol.md) to evaluate complete conversations, including short and interrupted sessions.

| Test case | Expected behavior |
| --- | --- |
| Learner starts a first session with a clear goal and ten minutes | State a target, scope, allowed help, and finish condition. Offer one starting check. |
| Starting check reveals a missing prerequisite | Explain the adjusted target and update the final check to match it. |
| Learner succeeds after two hints | Record the hints and use a fresh final task with the agreed support. Wait for the attempt before evaluating it. |
| Learner says “stop” before the final check | Mark the check pending, summarize available evidence, and end the session. |
| Learner pauses in the middle of a task | Record the unfinished step and exact next action. Mark the session paused. |
| Learner resumes with a record and a review due | Read the record and give the review or next task before a refresher when appropriate. |
| A session ends after successful practice | Report the observed result and plan a delayed check where retention matters. |
| The agent cannot save the session record | Provide a copyable handoff and accurately report the save failure. |
| The final check needs a partner or another day | End with the check pending and tell the learner how to return the result. |
| Prior session context is unavailable | Use the learner’s handoff or a brief baseline to establish the starting point. |

Verify that the closing contains a visible status, evidence, remaining gap, and next opening task. Check that personal session records use the learner’s agreed storage destination.

## Test whether people learn

1. **Choose a bounded capability.** For example, diagnose an off-by-one error in an unfamiliar loop or recognize which of two algebra methods fits a problem.
2. **Build parallel tasks.** Give baseline, practice, delayed, and transfer items with comparable prerequisite demands. Keep assessment items distinct from the worked solutions used during practice.
3. **Choose a comparison that matches the question.** To test graduated hints, compare them with a worked-example explanation followed by its own practice task. Match study time and content as closely as practicable. Use multiple people and assign conditions when feasible.
4. **Score independent and assisted work separately.** Save the artifact, amount of help, task variant, and time elapsed. For open-ended work, use the same rubric and mix the order of artifacts before review if practical.
5. **Check both outcomes and failure cases.** Look for task completion, later retention, transfer, invalid feedback, and where the learner stopped or needed more support. Interpret a small trial as local evidence for refining the coach.

A skill evaluation can use these checks without requiring every learner to follow the same sequence. Start with the evidence and conditions the learner provides. Use autonomy as an outcome when the user wants to perform unaided. When the goal includes AI or documentation, assess how well the learner directs, verifies, and recovers using those tools. [Measurement and maintenance](assessment-and-maintenance.md) · [Transfer and performance under pressure](transfer-and-pressure.md)
