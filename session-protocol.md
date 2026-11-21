# Starting and ending an agent-led learning session

[Wiki home](README.md) · [Coaching playbook](codex-coach.md) · [Evaluate the coach](mastery/codex-evaluation.md)

Every coaching session has an opening, a practice period, and a closing. The opening establishes what the learner is working on and what will count as a useful attempt. The closing records the evidence and leaves a concrete starting point for the next session. This protocol is a proposed agent workflow that applies the wiki’s [practice design](practice-design.md) and [assessment guidance](assessment.md).

## Open the session

1. **Recover context.** Read the available previous session record. Identify its next task and pending review. For a first session, use the learner’s stated goal and any example they provide.
2. **Set the scope.** Choose one target, the available time or number of exercises, and the tools or help allowed. Reuse known preferences and ask only for missing information that changes the plan. If time is unspecified, propose one short practice round.
3. **State the finish condition.** Name the final check and when practice will end. For example, “We’ll finish with one fresh loop to debug using Python documentation, then record what you could do.”
4. **Give a starting check.** Offer a brief attempt that shows the current capability. If a review is due, check it before a refresher. Use the result to choose the practice.

Make the start visible with a short message such as the following. Give the opening task and wait for the learner’s attempt.

> **Session started.** We’ll spend about 20 minutes practicing loop boundaries. Success today means finding the error in a fresh function and explaining the correction using Python documentation. First, predict what this short loop does at the boundary. We’ll finish with a similar check and save the next step.

The opening goal can change if the attempt reveals a missing prerequisite. Explain the adjustment and update the finish condition. For physical skills, include the usual warm-up and setup before measuring the target.

## Practice within the agreed scope

Use a short cycle of attempt, observation, feedback, and retry. Record the task, outcome, and help used. Choose the next exercise from that evidence. A successful attempt after a hint gives a useful starting point for fading that hint on a fresh case.

Work toward the agreed final check within the time or exercise budget. When elapsed time is available, use it. Otherwise, track completed exercises or ask for remaining time at a natural break. The agent should describe a time allocation as approximate unless it can actually measure it.

## Close the session

Start closing when the learner asks to finish, the agreed scope is reached, or they need to stop for another reason.

1. **Offer the final check when practical.** Use a short fresh or comparable task with the agreed tools and support. Give the learner time to answer before evaluating it.
2. **Compare the evidence.** Describe the starting and ending attempts, including any difference in difficulty or help. Record an unfinished check as pending.
3. **Name the next target.** Identify one remaining gap and choose the next opening task. When retention matters, suggest a review gap that fits the learner’s goal and availability.
4. **Write the handoff.** Produce the compact record below. Save it to an established local learning record when available, then report the saved location. Otherwise, include a copyable record in the response.
5. **Mark the close explicitly.** Say “Session ended” or “Session paused,” state the outcome, and stop presenting exercises until the learner resumes.

For example, after observing both attempts, the closing could read as follows.

> **Session ended.** You found the boundary error in the final function and explained the correction using the allowed documentation, with zero hints. The opening attempt needed one cue. Next time, start with a fresh boundary case before reviewing the rule. Suggested review is in two days. Your session record is below.

Describe the result as performance observed today. A later check adds evidence about retention. Use comparable conditions and fresh cases to assess the ability more broadly. [Assessment guidance](assessment.md) · [Retention and transfer research](foundations.md#separate-what-you-can-do-now-from-what-you-can-do-later)

## Handle stops, interruptions, and resuming

| Situation | Agent behavior |
| --- | --- |
| Learner says “stop,” “done,” or “end session” | Close using available evidence. Mark any skipped final check as pending and give a short handoff. |
| Learner says “pause” or “I have to go” | Mark the session paused and record the exact unfinished task, completed steps, and next action. |
| The chat ends unexpectedly | On return, use the most recent visible work and saved record. Describe the last known state and check whether the learner wants to resume it. |
| The learner resumes a paused session | Read the record, give the next action, and offer a brief check if a meaningful gap has passed. |
| A new session follows a completed session | Begin with the recorded opening task or due review. Confirm any changed constraints. |
| The learner reaches the goal early | Run the final check and close. Expand the scope when the learner wants more practice. |
| The learner asks to continue after closing | Start another round with a fresh scope and finish condition, or resume the recorded unfinished task. |

At an explicit stop, make the record from the evidence already available. If the agent lacks access to a prior record, ask for the relevant handoff or use a short baseline to rebuild context.

## Keep a compact session record

```text
Date and skill:
Status: ended / paused
Target and success criterion:
Scope used: approximate time or completed exercises
Allowed tools and help:
Opening attempt and result:
Practice completed and help used:
Final check and result: observed / pending
Evidence: artifact location, test output, observation, or learner report
Remaining gap:
Next opening task:
Suggested review gap or agreed date:
If paused: unfinished step and exact next action
```

Keep learner records in the learner’s agreed storage location. This public research repository contains reusable protocol examples. Publishing a learner’s personal session record requires their authorization. Claim a record was saved only after the write succeeds. If saving fails, include the record in the closing message so the learner can carry it into the next session.

## Fit the final check to the skill

| Skill | Opening check | Closing check |
| --- | --- | --- |
| Guitar | Record one take of a troublesome transition at a stated tempo | Play the transition inside the chorus at a comparable tempo, then record pulse and continuity |
| Writing | Draft a short passage for a named reader and purpose | Draft or revise a fresh passage using the same criterion and collect reader feedback when available |
| Math | Solve one unfamiliar problem using agreed references | Choose and explain a method on a parallel problem with the same help allowed |
| Programming | Predict or debug a small function | Debug a fresh function and run a test that verifies the correction |
| Soccer | Observe a receiving opportunity with stated pressure and options | Observe a comparable live decision and record the choice and execution |

If a task needs a reader, partner, recording, or another day, end the chat session with that check marked pending and describe how to return its result.
