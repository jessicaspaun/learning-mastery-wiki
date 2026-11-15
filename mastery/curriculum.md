# From first lesson to independent performance

[Mastery research](index.md) · [Wiki home](../README.md) · [Practice design](../practice-design.md)

## Work backward from a real use

Start with one representative task that combines the capabilities the learner eventually needs. For programming, a learner might want to build and maintain a small command-line tool. The simplest whole version can read a few lines, transform them, and print a result. Learning the syntax of a loop serves that task. Later versions can add invalid input, tests, and a changed requirement. Whole-task instructional design proposes starting with simplified versions of the target activity, organizing practice into increasingly complex task classes, supplying the needed support, and using focused component practice where it helps. This is a design framework. The right progression depends on the task and the learner. [Van Merriënboer et al., instructional design for complex learning](https://classroom.eumetsat.int/pluginfile.php/8128/mod_resource/content/3/TakingtheLoadOffLearnersMind_JvanMerrienboer.pdf) · [Paas and Van Merriënboer, managing load in complex learning](https://doi.org/10.1177/0963721420922183)

| Field | Question |
| --- | --- |
| Target task | What would a competent person do in the setting the learner cares about? |
| Components | What must they recall, recognize, choose, execute, and check? |
| Prerequisites | Which of those capabilities would block the simplest version today? |
| Simplified whole task | What can be removed while preserving the central decision or coordination? |
| Representative variations | Which changes in audience, inputs, constraints, or timing matter in actual use? |
| Advancement evidence | What new attempt would show readiness to reduce support or increase complexity? |

A **simplified task** reduces demands while keeping the activity meaningful. A **scaffold** supplies help that can fade, such as completed steps, a worked model, or a question. Adjust difficulty and support separately. A learner can move from completing a scaffolded task to performing the same type unaided. Then add complexity. If the learner can already do it and explain the relevant choices, move ahead. [Expertise reversal effect](https://doi.org/10.1207/S15326985EP3801_4) · [How expertise develops](expertise.md)

## Choose work that reveals the decisions

| Domain | Simplified whole task | Focused drill | Increase the demands |
| --- | --- | --- | --- |
| Guitar | Play one complete verse slowly with a chart | Loop two bars at the chord change that disrupts the beat | Play the full song with a backing track, then another person |
| Writing | Draft a short request that a familiar reader can act on | Rewrite one unclear claim and ask a reader to paraphrase it | Change the audience, add an objection, or write with incomplete information |
| Math | Solve a short problem from setup through answer check | Practice the prerequisite operation when it keeps breaking the solution | Mix unmarked problem families and introduce a new representation |
| Programming | Write and run a small program that solves a defined problem | Trace or repair the branch that keeps failing | Add malformed input, a fresh specification, or someone else’s code |
| Soccer | Play a short possession exercise with an active defender and reachable outlets | Receive and direct the first touch to a target | Vary defender positioning, available outlets, or time pressure |

When showing a model, explain what you noticed and the decision it led to. An experienced programmer might reveal the edge case they think of before coding. A writer might explain why a paragraph appears early. Have the learner reconstruct a decision, try it on another case, and explain how they checked. This adapts *cognitive apprenticeship*, an instructional framework that includes modeling, coaching, scaffolding, articulation, reflection, and exploration. [Collins et al., cognitive apprenticeship](https://web.eecs.umich.edu/~mjguz/csl/home.cc.gatech.edu/allison/uploads/4/collins1989.pdf)

## Use checks and retries to decide when to advance

In instructional research, *mastery learning* refers to an approach that sets objectives, checks performance, gives corrective instruction, and allows another opportunity to meet the standard. An older synthesis of 108 controlled evaluations reported positive average effects on exam performance, with effects varying by design and subject. A more recent introductory-programming study illustrates how repeated opportunities can be built into one course. In the wiki, mastery also refers to dependable performance in the task conditions the user values. For that broader goal, add delayed and fresh checks to any criterion used to advance. [Kulik et al., mastery learning meta-analysis](https://doi.org/10.3102/00346543060002265) · [Montagner et al., introductory-programming course study](https://zilles.cs.illinois.edu/papers/mastery_INSPER_SIGCSE_2024.pdf)

1. **Set a useful criterion.** “Given an unfamiliar small data file and language documentation, implement the specified behavior and handle empty and invalid rows.”
2. **Collect a short attempt.** Use tasks that show whether the learner can choose and execute the relevant strategy.
3. **Give corrective practice.** If only empty rows fail, trace that case and revise the program.
4. **Check a new example.** Use a different file with an equivalent requirement. Repeat after a gap when retention matters.
5. **Advance locally.** Increase the demands of the component that is ready. Keep other parts of the plan at their current level.

A criterion can be a behavior, a qualitative rubric, or a score with a justification. Choose a threshold that fits the consequences of the target task. For a creative task, progress may show up as achieving a reader effect across several pieces, with several different ways of getting there.

## Allocate more practice where it changes performance

- **Use brief independent checks to find the current constraint.** If the learner cannot start, offer an example or smaller task. If the learner knows the method and picks the wrong one, compare cases. If the isolated skill works and full performance fails, reconnect the drill to a representative task.
- **Revisit earlier capabilities when they are required in later work.** A writing project can bring back argument structure while adding source evaluation. A longer guitar piece can bring back a chord progression while introducing a change of dynamics.
- **Make practice opportunities part of the environment.** Arrange a real reader, maintainer, teammate, or practice partner when the goal depends on one. Workplace transfer reviews identify opportunities to use training and supportive conditions as relevant alongside the training itself. [Blume et al., transfer of training meta-analysis](https://jasonhuangatwork.com/papers/Blume_Ford_Baldwin_Huang_2010_JOM-Training_Transfer_Meta.pdf) · [Grossman and Salas, training-transfer review](https://doi.org/10.1111/j.1468-2419.2011.00373.x)
- **Use simulation when real practice is scarce or costly.** Choose a simulation that preserves the relevant decisions and feedback. Evidence from health-professions training supports simulation paired with deliberate practice for the measured clinical skill outcomes. The interventions bundle several components, and transfer beyond measured skills depends on the simulation and assessment. [McGaghie et al., simulation and deliberate practice meta-analysis](https://pubmed.ncbi.nlm.nih.gov/21512370/)

## Adapt to the learner and their resources

Use the learner’s current attempt to select the starting point. Someone with experience in a neighboring domain may skip a prerequisite they can already demonstrate and need practice in places where the new domain differs. Offer usable formats, suitable equipment, and time to respond. For example, an athlete can practice identifying open space at a lower pace while preserving the passing choice. A programmer can use written or spoken models with the same test at the end. Distinguish the demands that define the skill from demands incidental to its presentation. Record accommodations or tool access when they affect what the assessment measures.

Research with older and younger adults illustrates the value of observing individual performance. In a bimanual force-tracking experiment, the two groups had different patterns of improvement within the session and similar overall reductions in error. The experiment measured one laboratory task over a single session. Use the learner’s own progress and access needs to decide pace and practice format. [Zvornik et al., bimanual tracking experiment](https://pmc.ncbi.nlm.nih.gov/articles/PMC11043555/) · [National Academies, learning and transfer](https://www.nationalacademies.org/read/9853/chapter/6)
