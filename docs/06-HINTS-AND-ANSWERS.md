# Hints and answer directions

[Return to the stories](05-PRACTICE-STORIES.md)

There are intentionally no complete feature patches here. Use one hint, return to your code and produce evidence. Your design can differ from the reference when you state and verify the new contract.

## Story 01: Add a fourth room

**Hint 1 — ownership:** Begin from `.exhibition and .exhibit-code`. Add a room article and its navigation link with a stable ID.

**Hint 2 — reasoning:** Revisit the decision “Use the requested breakpoints explicitly”. Ask yourself: Explain why max-width includes the named width.

**Answer direction:** A defensible solution demonstrates this observable result: The link resolves and the article remains readable at 320px. The exact code is not prescribed. If your change achieves that result by changing an unrelated original rule, revise either the implementation or the story contract explicitly.

**Self-review:** Could the UI or helper appear correct while the underlying rule remains wrong? Could the underlying calculation be correct while stale presentation misleads the user? Choose the question that applies and write one distinguishing example.

## Story 02: Show a route estimate

**Hint 1 — ownership:** Begin from `.exhibition and .exhibit-code`. Add a short fictional walking-time estimate as ordinary text.

**Hint 2 — reasoning:** Revisit the decision “Repair the cause of overflow”. Ask yourself: Distinguish wrapping a token from clipping its tail.

**Answer direction:** A defensible solution demonstrates this observable result: The estimate does not depend on an image or hover state. The exact code is not prescribed. If your change achieves that result by changing an unrelated original rule, revise either the implementation or the story contract explicitly.

**Self-review:** Could the UI or helper appear correct while the underlying rule remains wrong? Could the underlying calculation be correct while stale presentation misleads the user? Choose the question that applies and write one distinguishing example.

## Story 03: Create a boundary checklist

**Hint 1 — ownership:** Begin from `.exhibition and .exhibit-code`. Record observations at 801, 800, 501 and 500 pixels.

**Hint 2 — reasoning:** Revisit the decision “Keep the reading order stable”. Ask yourself: Explain what a screen reader or stylesheet-free view encounters first.

**Answer direction:** A defensible solution demonstrates this observable result: Each entry identifies the property and expected arrangement. The exact code is not prescribed. If your change achieves that result by changing an unrelated original rule, revise either the implementation or the story contract explicitly.

**Self-review:** Could the UI or helper appear correct while the underlying rule remains wrong? Could the underlying calculation be correct while stale presentation misleads the user? Choose the question that applies and write one distinguishing example.

## Story 04: Improve a long identifier label

**Hint 1 — ownership:** Begin from `.exhibition and .exhibit-code`. Add descriptive context before the catalogue code without shortening the value.

**Hint 2 — reasoning:** Revisit the decision “Use the requested breakpoints explicitly”. Ask yourself: Explain why max-width includes the named width.

**Answer direction:** A defensible solution demonstrates this observable result: The full value remains available and its purpose is clear. The exact code is not prescribed. If your change achieves that result by changing an unrelated original rule, revise either the implementation or the story contract explicitly.

**Self-review:** Could the UI or helper appear correct while the underlying rule remains wrong? Could the underlying calculation be correct while stale presentation misleads the user? Choose the question that applies and write one distinguishing example.

## Story 05: Add a reduced-motion policy

**Hint 1 — ownership:** Begin from `.exhibition and .exhibit-code`. If you experiment with smooth scrolling, add a reduced-motion alternative.

**Hint 2 — reasoning:** Revisit the decision “Repair the cause of overflow”. Ask yourself: Distinguish wrapping a token from clipping its tail.

**Answer direction:** A defensible solution demonstrates this observable result: Navigation remains usable with motion reduction enabled. The exact code is not prescribed. If your change achieves that result by changing an unrelated original rule, revise either the implementation or the story contract explicitly.

**Self-review:** Could the UI or helper appear correct while the underlying rule remains wrong? Could the underlying calculation be correct while stale presentation misleads the user? Choose the question that applies and write one distinguishing example.

## Story 06: Improve narrow spacing

**Hint 1 — ownership:** Begin from `.exhibition and .exhibit-code`. Adjust the 500px rule after inspecting actual content crowding.

**Hint 2 — reasoning:** Revisit the decision “Keep the reading order stable”. Ask yourself: Explain what a screen reader or stylesheet-free view encounters first.

**Answer direction:** A defensible solution demonstrates this observable result: No essential content disappears and the reason for the change is recorded. The exact code is not prescribed. If your change achieves that result by changing an unrelated original rule, revise either the implementation or the story contract explicitly.

**Self-review:** Could the UI or helper appear correct while the underlying rule remains wrong? Could the underlying calculation be correct while stale presentation misleads the user? Choose the question that applies and write one distinguishing example.

## Answers to the trace questions

The viewport selects matching media rules → the desktop flex layout becomes block layout at 800px → room navigation links stack at 500px → min-width and overflow-wrap keep the long identifier inside its content box.

The expected examples are in the concepts table. Use them to check your reasoning, then supply a new example of your own. A copied sentence is not evidence that you can trace a changed input.

## When to ask for more help

Ask after you can show a concrete attempt, a specific uncertainty and an observation. Request a smaller hint before a full patch. If you do accept generated code, explain each changed line and run a counterexample you chose independently.
