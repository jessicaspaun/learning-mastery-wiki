# Codex coaching playbook

[Wiki home](README.md) · [Technique reference](techniques.md) · [Evidence notes](evidence.md) · [Coach evaluation](mastery/codex-evaluation.md)

This page is reference material for building a Codex skill that helps a learner practice. It describes the coaching behavior, the evidence behind it, and scenarios to check during development.

## Start from the learner’s task

Gather the information that changes the exercise. Ask for the goal and current level when they are unclear. If the learner has a recent attempt, use it. When a useful next step is possible, offer a short baseline or exercise with a stated assumption. Invite the learner to adjust time, equipment, accessibility preferences, available feedback, or the desired depth.

Useful intake prompts include “What do you want to be able to do?”, “What can you already do on your own?”, and “Where did your last attempt get stuck?” A goal, a sample, and the relevant constraints usually give enough context for the first task. Use the [practice design](practice-design.md) and [domain guides](README.md#pick-a-guide) to select the exercise.

## Choose the next action from the attempt

| Observation | Coach response |
| --- | --- |
| Missing fact or definition | Supply or locate a reliable explanation, then ask for a recall attempt and check it |
| Prerequisite or procedure is unfamiliar | Show a short model, then give a partial problem or similar attempt |
| Learner can explain a rule and misapplies it | Ask for a prediction, compare cases, and check one boundary case |
| Learner can execute methods when told which to use | Mix two or three known types. Ask which method they chose and what cue guided them. |
| Output is hard to assess | Ask for a draft, test output, recording observation, or independent assessor’s notes and use a specific criterion |
| Learner only succeeds with cues | Give a comparable task with less support, then add an independent attempt after a gap |
| Drill performance fails in context | Preserve the practiced component and add the relevant real-world constraint, audience, timing, or decision |
| Learner demonstrates the goal across attempts | Increase a relevant demand, test transfer, or define a broader goal with the learner |

When giving feedback, identify the evidence, explain the gap, and give the learner a change to test. Mark interpretations as hypotheses if the available evidence could support several explanations. If a sensory observation is needed, ask for the evidence the learner can provide. For example, ask them to count where the rhythm drifted on a recording or ask a coach to observe their first touch.

## When Codex is the practice partner

In coaching mode, give the learner an opportunity to think before offering a solution. Offer progressively more help when the learner stalls or asks for it:

1. **Prompt** the observation or prediction that would narrow the problem.
2. **Cue** the concept, step, or example that may help.
3. **Scaffold** a partial solution and ask the learner to finish or modify it.
4. **Model** the complete solution with the reasoning, then offer a fresh task that the learner can attempt independently.

Answer directly when the learner asks for an explanation or a worked solution. A fresh follow-up problem can check understanding after a complete demonstration. For writing, distinguish feedback, revision suggestions, and the learner’s own draft in the coaching workflow. For programming, propose a failing test or point to a trace before editing when the user asks to learn by debugging. Generate answer keys separately from practice prompts when immediate visibility would give away the solution.

AI-supported practice and learning can diverge. A field experiment in high-school math found that a general-purpose chatbot improved performance during practice while the group later scored lower on an unaided test. A teacher-designed tutoring condition mitigated the drop. A college physics experiment found improved immediate posttests with a designed AI tutor in its setting. A 2026 programming preprint by Shen and Tamkin reported weaker understanding and debugging when developers learned a new library with AI assistance in their experiment. These studies differ in settings, designs, and outcomes. For a coaching skill, include checks that match the learner’s intended level of independence. [Bastani et al., math field experiment](https://doi.org/10.1073/pnas.2422633122) · [Kestin et al., college physics trial](https://pmc.ncbi.nlm.nih.gov/articles/PMC12179260/) · [Shen and Tamkin, programming preprint](https://arxiv.org/abs/2601.20245)

## A compact coaching response

```text
Target: What the learner is practicing right now.
Task: One specific attempt, with allowed help and a success criterion.
Feedback: What the attempt shows and one change to try.
Next check: A comparable delayed task or a new case with relevant variation.
```

Use only the fields that fit the moment. If you are handing the learner an exercise for the first time, give the task and wait for their attempt before giving feedback. A longer plan can include the weekly sequence and a practice log. Cite sources when making evidence claims, and call an example schedule or threshold a starting point.

## Scenarios to test a future skill

| Learner request | Good coaching behavior | What to check |
| --- | --- | --- |
| “I know the guitar chords individually, but I lose the beat during changes.” | Establish a tempo baseline, isolate two bars, reconnect them, and plan a cold take | The drill measures pulse through the transition and returns to the song |
| “Everyone says my writing is confusing.” | Ask for a draft and its intended reader, choose one problem, and use reader feedback to guide revision | The coach can explain the reader’s difficulty using a specific passage |
| “I do fine on worksheets but freeze on mixed math quizzes.” | Compare confusable problem types, mix unlabeled problems, and ask for the reason behind each choice | Delayed tasks require selecting a method independently |
| “I can follow Python videos, but I can’t start a script.” | Demonstrate a small example and move through predicting, tracing, modifying, and building | The learner implements or debugs a fresh variation with the agreed tools |
| “My passes are good in practice but I lose the ball in games.” | Diagnose whether the issue is scanning, touch, timing, the decision, or pass execution. Add a live option and a defender. | The learner judges an opportunity in play and records the choice and outcome separately |
| “Just show me how to solve this.” | Give the explanation in full, with a follow-up exercise if useful | The request is answered and the next practice task has its own independent check |

For evaluation, compare what the learner can do on their own after using the skill with their baseline. Check whether the coach chooses the appropriate practice for the error and whether the follow-up case measures the stated goal. Use realistic user requests and both novice and experienced learner examples.
