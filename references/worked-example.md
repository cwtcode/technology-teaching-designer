# Worked alignment example: input validation

Treat this as an illustrative design, not observed classroom evidence or official curriculum alignment.

## Context and specification

Assume S2 or comparable beginners who can use input, variables, and one conditional in Python; 50 minutes; pairs with one computer. Confirm these assumptions in actual use. Use synthetic scores rather than personal data.

O1: Explain how a validity rule distinguishes accepted/rejected inputs.
O2: Implement and test a score range rule, including boundary cases.
O3: Use feedback to improve the solution and explain one revision.

Core scope: scores supplied as integers; 0 to 100 inclusive. Invalid text conversion is an extension, not an unannounced prerequisite. Core inquiry: "What evidence would convince another person that our rule works?"

## Sequence

| Stage | Minutes | Activity and evidence |
|---|---:|---|
| Instruction | 6 | Diagnose whether students distinguish 0, 100, -1, 101; share criteria |
| Demo | 8 | Predict a flawed rule using OR; trace two cases; contrast AND |
| Guided practice/application | 20 | Complete a partially worked range check; choose cases; independently adapt to a different range |
| Evaluation/improvement | 10 | Exchange test plans, run them, identify missed boundaries, revise and explain |
| Conclusion | 6 | Individually explain why both limits matter and propose the next test |

Reserve the last two practice minutes for saving and transition. If the diagnostic shows missing condition knowledge, replace the independent coding variation with supported tracing and schedule coding next lesson.

## Resource alignment

- Worksheet A1: predict accepted/rejected cases (O1); slide prompt uses identical values.
- Worksheet A2: complete and explain the condition (O1/O2); demo and notes use the same rule.
- Worksheet A3: test table with input, expected outcome, actual outcome, explanation (O2).
- Worksheet A4: peer feedback and recorded revision (O3); slide criteria match the answer guide.
- Exit E1: explain why a boundary case matters (O1/O2).

Example core logic, assuming an integer variable named score:

```python
if 0 <= score <= 100:
    print("Accepted")
else:
    print("Rejected")
```

Expected: -1 rejected; 0 accepted; 50 accepted; 100 accepted; 101 rejected. If full input conversion is included, explicitly teach and test non-numeric input handling.

## Inquiry, agency, rationale and anticipation

Use guided inquiry: teacher fixes the validity requirement and time; students choose test cases, justify coverage, and prioritise a revision. Provide hints only as needed. Use a worked example to manage procedural complexity and fade the completed condition for transfer. Examine individual explanation rather than inferring understanding from pair completion.

Anticipate OR/AND confusion, omission of equality at boundaries, dominant partners, and changes made without testing. Use value tracing, contrasting cases, rotating tester/explainer roles, and one-change-at-a-time retesting. If computers fail, trace printed snippets with test cards. Do not claim that these supports succeeded before collecting evidence.
