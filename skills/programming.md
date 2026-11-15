# Learning programming

[Wiki home](../README.md) · [Practice design](../practice-design.md) · [Codex coaching playbook](../codex-coach.md)

## Name the capability

Programming combines knowing language features, reading code, predicting behavior, designing a solution, writing and testing it, and diagnosing failures. Try one small baseline that resembles the work you want to do. When you can follow a tutorial and struggle to start your own script, practice turning a short brief into inputs, outputs, examples, and working code.

## Predict, run, investigate, modify, make

The activities below adapt PRIMM, a school-based programming pedagogy. Read each activity at the moment you need it.

```python
def count_short_words(words, limit):
    count = 0
    for word in words:
        if len(word) < limit:
            count += 1
    return count
```

1. **Predict.** On paper, predict the result of `count_short_words(["a", "bee", "ox"], 3)` and the result with an empty list.
2. **Run.** Compare the observed and predicted results.
3. **Investigate.** Trace `word`, `len(word)`, and `count` after each iteration. Explain what happens when a word has length exactly 3.
4. **Modify.** Change the boundary to count words of length at most the limit. Write a test that fails with the original version and passes after the change.
5. **Make.** Start from a blank file. Given a list of expense amounts and a budget threshold, write a function that counts expenses strictly below the threshold. Test an empty list, one equal to the threshold, and lists where all or none qualify. After that, add a second requirement such as accepting only positive amounts.

<details>
<summary>Check the two predictions</summary>

The outputs are `2` and `0`. The comparison is strict, so the three-letter word is skipped. With an empty list, the loop executes zero times and the count stays at zero.

</details>

If reading is a struggle, label each section by its purpose. If writing from a blank page is too hard, reorder scrambled solution lines, then fill gaps in a similar function and eventually write a new one.

## Practice debugging explicitly

1. Reproduce the problem with a small input. State the expected and actual behavior.
2. Make a prediction about where execution diverges from your expectation.
3. Use a trace, debugger, or focused log to inspect a relevant variable or branch.
4. Change one thing and rerun. Add a test for the failure and run related tests.
5. Explain why the change works and what new input could still break it.

For a larger project, choose a thin feature with a clear behavior you can test. Make it work end to end, then introduce an edge case or a new requirement. Practice reading unfamiliar code as well as starting from a blank file.

## Check retention and transfer

After a gap, implement a fresh function from a new brief and debug a small unfamiliar program. Keep agreed resources available. Verify behavior with tests, ask the learner to explain a design choice or trace an edge case, then change one requirement. When AI is part of practice, include a check at the level of AI assistance the learner needs to work with independently.

## What the research covers

The PRIMM school study reported higher posttest performance in intervention classes. A systematic review describes Parsons problems, in which learners reorder code, as a scaffold with open questions about transfer. A semester-long introductory programming study found that subgoal-labeled examples helped early quiz performance and course completion outcomes. Average exam scores were similar. Debugging research describes a range of intervention designs with differing evidence. The script and project progressions are adaptations for self-study. [Sentance et al., PRIMM](https://eprints.gla.ac.uk/229013/) · [Ericson et al., Parsons problems review](https://doi.org/10.1145/3571785.3574127) · [Margulieux et al., labeled subgoals](https://doi.org/10.1186/s40594-020-00222-7) · [Systematic review of debugging instruction](https://doi.org/10.1145/3690652)
