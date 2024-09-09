# Judging grid criteria

The goal of the judging grid is to reward all the different type of teams and process

* Reward actual findings
* Reward all valid tests scenario
* Reward team's understanding and team's process to find scenario
* Publishing this grid helps team to not stop on failed scenario but to focus on the overall security testing as a learning

## Judging grid proposal

Here is a proposal on criteria to evaluate the teams

| Criteria | Comment | Min | Max |
|----------|----------|----------|----------|
| CVSS Score | Computed using a CVSS calculator  | 0 | 10 |
| False positive multiplier | A failed attempt give less points  | x0.2 | x1 |
| Explanation clarity | They know what that are doing and follow a good methodology  | x0.5 | x1.5 |||
| Assessment is correct | They understand and explain the security issue. |  -2 | +2 |
| Correct mitigation | They propose a correct mitigation |  -2 | +2 |
| Technical/Functional complexity | The scenario is complex technically |  0 | +5 |
| Originality / innovative touch | The original of the scenario  |  0 | +5 |
| Total including small team multiplier*| |  |  |

To compute a test score, you multiple the CVSS by the multipliers and add the _bonus_ to it. To be fair, put 0 in case of negative score for the test.

\* Optional: To compute the total score, you sum up all the test scores and multiply by a **small team** multiplier that could help the smaller team (where it was more complex). The multiplier is x1 for a team of 5 people, x1.2 for a team of 4, x1.5 for a team of 3 and x2 for a team of 2.

## Common examples

* Participant tampers a user name entered in the UI and it is reflected: Not an issue, it could have been done directly with the UI -> False positive, x0.5
* Participant finds a business/functional case that makes the issue much worse than expected: innovative touch +4-5

### Case example

Imagine a team of 5 people with 3 tests, 2 false positive and a true positive.

* Test 1 is a real vulnerability, estimated CVSS 8, quite well explain and very technical
* Test 2 is a false positive, very creative scenario that could have been a real vulnerability but is, in fact, well mitigated
* Test 3 is a false positive of a medium issue, not well understand and assessed

| Criteria                       |  Min | Max | Test 1 | Test 2 | Test 3
|----------|----------|----------|--------|------|----|
| CVSS Score                 |0 | 10 | 8 | 7 | 5
| False positive multiplier  | x0.2 | x1 | 1 | 0.2 | 0.2
| Explanation clarity  | x0.5 | x1.5 | 1.2 | 1.5 | 0.8
| Assessment is correct  |  -2 | +2 |+2|+2|-1
| Correct mitigation  |  -2 | +2 |+1|0|-1
| Technical/Functional complexity  |  0 | +5 |+5|+3|0
| Originality / innovative touch   |  0 | +5 |0|+3|0
| Total | | | 17.6 | 10.1 | 0

**Grand total** : (17.6+10.1+0) x 1 = **27.7**

## Rewards

The rewards do not have to be limited to the best score. You could also create specific categories like:

* Most serious vulnerability
* Most innovative finding
* Best test plan
* "Worst" vulnerability found

## Sheets

The judging material is provided in the _material_ folder as:

* [Open document template](material/hacking-event-judging.ods)
* [Microsoft Excel template](material/hacking-event-judging.xltx)