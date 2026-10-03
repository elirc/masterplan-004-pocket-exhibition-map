# Rebuild Pocket Exhibition Map through small verified slices

[Expanded workshop map](WORKBOOK-INDEX.md) · [Repository overview](../README.md)

This is a hypothetical reconstruction exercise using the existing reference as a comparison point. Work on a practice branch or a separate scratch copy. Do not erase the working reference. Your goal is to recover the important decisions from requirements, not reproduce every character or configuration file from memory.

## Session zero: write a contract you can challenge

The guide stacks its route and exhibit list at max-width:800px, simplifies navigation at max-width:500px, and wraps the deliberately long catalogue identifier at 320px without hiding it.

Your target skill is responsive layout and overflow diagnosis. Write three examples before implementation: one ordinary success, one boundary distinction and one recovery or repeat sequence. Reuse the fixed reference fixtures only after making a prediction. If your new example is outside the documented scope, decide whether to reject it or explicitly expand the contract; do not let an incidental implementation choice decide silently.

Write a short non-goal list tied to this exercise. Non-goals keep an assistant from adding a database, a UI framework or a broad refactor before you understand the central rule. For static layout work, a meaningful non-goal may be scripting interactions that native HTML already handles. For stateful work, it may be remote persistence or a global state container.

## Slice 1: Map content before drawing boxes

**Reference context:** The visitor needs a short route and a sequence of rooms. The room links refer to real fragment IDs so they remain useful without JavaScript. The route is supporting information, not a separate interactive map service. Limiting the feature to text and local anchors keeps the responsive behavior directly inspectable.

### Your implementation route

1. Inspect `public/style.css` and the related adapter `public/index.html and public/style.css`. Write which responsibility belongs to each for this slice. A path is a place to inspect, not automatic permission to edit every file.
2. State the example independently: **801px → Desktop two-region arrangement**. Explain which requirement supplies the expected answer.
3. Build the smallest version that can express the example. Start with explicit data and direct control flow. Introduce a helper only when you can name its input, output and reason to change.
4. Observe the result through the real boundary: a command, a browser control, or a layout condition. A function returning the right value does not prove a button passes it the right input.
5. Add a neighboring example that would fail if you special-cased the first one. Review your diff before comparing with the reference.

### Pause at the first uncertainty

Write the smallest question you cannot answer. It might concern ownership, a comparison operator, the effect of deleting a property, or when a callback actually runs. Include the exact expression and an example. Ask a mentor for one clue, then return to the source; avoid requesting a complete replacement implementation.

### Inspect an alternative

Choose one plausible different design for this slice. Describe the extra state, dependency or maintenance rule it introduces. If it satisfies the same contract, it is not automatically wrong. Compare the cost of making the next small change. If it violates the contract, provide the smallest concrete example that demonstrates that violation.

### Capture a reviewable stopping point

Record your actual check: npm test (local asset references), plus the relevant browser/content observation. State what it established and what remains untested. Use a commit message about the resulting behavior rather than a list of file names. If the slice does not work yet, keep the uncertainty visible in the journal instead of writing a success narrative.

**Left for you:** the code, fixture values beyond the supplied example, exact naming and the acceptance evidence. The reference is available for comparison after an attempt; it is not evidence that your branch has passed.

## Slice 2: Make the desktop relationship explicit

**Reference context:** The exhibition container distributes an aside and a content section. The aside takes a bounded share; the section can use the remaining room. Read min-width:0 on the section before examining the long identifier. It gives the section permission to shrink below content-driven minimum sizing, while overflow-wrap decides how the identifier uses that smaller area.

### Your implementation route

1. Inspect `public/style.css` and the related adapter `public/index.html and public/style.css`. Write which responsibility belongs to each for this slice. A path is a place to inspect, not automatic permission to edit every file.
2. State the example independently: **800px → Route stacks above exhibits**. Explain which requirement supplies the expected answer.
3. Build the smallest version that can express the example. Start with explicit data and direct control flow. Introduce a helper only when you can name its input, output and reason to change.
4. Observe the result through the real boundary: a command, a browser control, or a layout condition. A function returning the right value does not prove a button passes it the right input.
5. Add a neighboring example that would fail if you special-cased the first one. Review your diff before comparing with the reference.

### Pause at the first uncertainty

Write the smallest question you cannot answer. It might concern ownership, a comparison operator, the effect of deleting a property, or when a callback actually runs. Include the exact expression and an example. Ask a mentor for one clue, then return to the source; avoid requesting a complete replacement implementation.

### Inspect an alternative

Choose one plausible different design for this slice. Describe the extra state, dependency or maintenance rule it introduces. If it satisfies the same contract, it is not automatically wrong. Compare the cost of making the next small change. If it violates the contract, provide the smallest concrete example that demonstrates that violation.

### Capture a reviewable stopping point

Record your actual check: npm test (local asset references), plus the relevant browser/content observation. State what it established and what remains untested. Use a commit message about the resulting behavior rather than a list of file names. If the slice does not work yet, keep the uncertainty visible in the journal instead of writing a success narrative.

**Left for you:** the code, fixture values beyond the supplied example, exact naming and the acceptance evidence. The reference is available for comparison after an attempt; it is not evidence that your branch has passed.

## Slice 3: Inspect equality at each breakpoint

**Reference context:** Set the viewport to 801px and then 800px. Repeat around 501px and 500px. Describe the exact property that changes, rather than saying the page becomes mobile. This is the CSS version of a boundary-value test: equality is part of the contract, not an incidental screenshot dimension.

### Your implementation route

1. Inspect `public/style.css` and the related adapter `public/index.html and public/style.css`. Write which responsibility belongs to each for this slice. A path is a place to inspect, not automatic permission to edit every file.
2. State the example independently: **500px → Room links stack vertically**. Explain which requirement supplies the expected answer.
3. Build the smallest version that can express the example. Start with explicit data and direct control flow. Introduce a helper only when you can name its input, output and reason to change.
4. Observe the result through the real boundary: a command, a browser control, or a layout condition. A function returning the right value does not prove a button passes it the right input.
5. Add a neighboring example that would fail if you special-cased the first one. Review your diff before comparing with the reference.

### Pause at the first uncertainty

Write the smallest question you cannot answer. It might concern ownership, a comparison operator, the effect of deleting a property, or when a callback actually runs. Include the exact expression and an example. Ask a mentor for one clue, then return to the source; avoid requesting a complete replacement implementation.

### Inspect an alternative

Choose one plausible different design for this slice. Describe the extra state, dependency or maintenance rule it introduces. If it satisfies the same contract, it is not automatically wrong. Compare the cost of making the next small change. If it violates the contract, provide the smallest concrete example that demonstrates that violation.

### Capture a reviewable stopping point

Record your actual check: npm test (local asset references), plus the relevant browser/content observation. State what it established and what remains untested. Use a commit message about the resulting behavior rather than a list of file names. If the slice does not work yet, keep the uncertainty visible in the journal instead of writing a success narrative.

**Left for you:** the code, fixture values beyond the supplied example, exact naming and the acceptance evidence. The reference is available for comparison after an attempt; it is not evidence that your branch has passed.

## Slice 4: Debug the deliberate stress content

**Reference context:** The catalogue identifier is intentionally longer than ordinary text. Temporarily remove its wrapping rule and inspect the page’s scroll width. Do not solve the problem by deleting the identifier or hiding horizontal overflow. A correct layout keeps the content available and expresses where a break is permitted.

### Your implementation route

1. Inspect `public/style.css` and the related adapter `public/index.html and public/style.css`. Write which responsibility belongs to each for this slice. A path is a place to inspect, not automatic permission to edit every file.
2. State the example independently: **320px with long identifier → Identifier remains visible and wraps**. Explain which requirement supplies the expected answer.
3. Build the smallest version that can express the example. Start with explicit data and direct control flow. Introduce a helper only when you can name its input, output and reason to change.
4. Observe the result through the real boundary: a command, a browser control, or a layout condition. A function returning the right value does not prove a button passes it the right input.
5. Add a neighboring example that would fail if you special-cased the first one. Review your diff before comparing with the reference.

### Pause at the first uncertainty

Write the smallest question you cannot answer. It might concern ownership, a comparison operator, the effect of deleting a property, or when a callback actually runs. Include the exact expression and an example. Ask a mentor for one clue, then return to the source; avoid requesting a complete replacement implementation.

### Inspect an alternative

Choose one plausible different design for this slice. Describe the extra state, dependency or maintenance rule it introduces. If it satisfies the same contract, it is not automatically wrong. Compare the cost of making the next small change. If it violates the contract, provide the smallest concrete example that demonstrates that violation.

### Capture a reviewable stopping point

Record your actual check: npm test (local asset references), plus the relevant browser/content observation. State what it established and what remains untested. Use a commit message about the resulting behavior rather than a list of file names. If the slice does not work yet, keep the uncertainty visible in the journal instead of writing a success narrative.

**Left for you:** the code, fixture values beyond the supplied example, exact naming and the acceptance evidence. The reference is available for comparison after an attempt; it is not evidence that your branch has passed.

## Reconstruct the whole path without the guide

The viewport selects matching media rules → the desktop flex layout becomes block layout at 800px → room navigation links stack at 500px → min-width and overflow-wrap keep the long identifier inside its content box.

Close this page and redraw that route from memory using your own labels. Open the code only to resolve a specific uncertainty. Then trace a different valid input and one boundary. If your picture requires a hidden value that you cannot locate in the source, investigate it; diagrams can invent state just as easily as prose can.

## Compare your implementation fairly

First compare behavior and evidence. Only then compare style and abstractions. A shorter implementation may be harder for you to explain; a longer implementation may duplicate a rule that later drifts. State the concrete tradeoff. Do not treat matching the reference line for line as the only successful outcome.

## Finish with a teach-back

Explain why `.exhibition and .exhibit-code` is enough for its present responsibility, which work remains in `public/index.html and public/style.css`, and which future requirement would justify changing that boundary. Answer the original transfer question: Why is hiding overflow a poor substitute for understanding its cause? Keep the answer short enough that another junior can challenge it with an example.
