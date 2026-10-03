# Six junior practice stories

[Debugging lab](04-DEBUGGING-LAB.md) · [Hints — use after an attempt](06-HINTS-AND-ANSWERS.md)

These are new exercises beyond the finished reference. No story is marked complete for you. Start a branch such as practice/story-01 and write acceptance examples before editing. Each plan leaves the actual code, wording and one design choice to you.

## Story 01: Add a fourth room

**User need:** As a learner or user of Pocket Exhibition Map, I want this small improvement so the behavior is easier to use, explain or verify.

**Feature boundary:** Add a room article and its navigation link with a stable ID.

**Implementation plan:**

1. Trace `.exhibition and .exhibit-code` and locate the smallest owning file from the code tour. Write how this story touches that responsibility.
2. Write a before/after example that demonstrates this acceptance requirement: The link resolves and the article remains readable at 320px.
3. Choose the input shape, wording or layout policy yourself. Record one alternative and the reason you did not choose it.
4. Implement only the bounded change. If it crosses files, explain what each file owns rather than copying the same decision into several places.
5. Reproduce the acceptance example and one existing boundary case. Add an automated regression for executable logic, or an explicit browser/keyboard/content observation for a static change.
6. Review the diff, explain the change without reading the solution, and record remaining limits.

**Acceptance evidence:** The link resolves and the article remains readable at 320px.

**Left for you:** exact fixture values, names, wording, the implementation and the tradeoff decision. Do not open the hints until you have an example and a first attempt.

**Stretch only after completion:** add one adversarial example that a plausible but incorrect solution would fail. Explain why that example is more informative than adding three ordinary examples.

## Story 02: Show a route estimate

**User need:** As a learner or user of Pocket Exhibition Map, I want this small improvement so the behavior is easier to use, explain or verify.

**Feature boundary:** Add a short fictional walking-time estimate as ordinary text.

**Implementation plan:**

1. Trace `.exhibition and .exhibit-code` and locate the smallest owning file from the code tour. Write how this story touches that responsibility.
2. Write a before/after example that demonstrates this acceptance requirement: The estimate does not depend on an image or hover state.
3. Choose the input shape, wording or layout policy yourself. Record one alternative and the reason you did not choose it.
4. Implement only the bounded change. If it crosses files, explain what each file owns rather than copying the same decision into several places.
5. Reproduce the acceptance example and one existing boundary case. Add an automated regression for executable logic, or an explicit browser/keyboard/content observation for a static change.
6. Review the diff, explain the change without reading the solution, and record remaining limits.

**Acceptance evidence:** The estimate does not depend on an image or hover state.

**Left for you:** exact fixture values, names, wording, the implementation and the tradeoff decision. Do not open the hints until you have an example and a first attempt.

**Stretch only after completion:** add one adversarial example that a plausible but incorrect solution would fail. Explain why that example is more informative than adding three ordinary examples.

## Story 03: Create a boundary checklist

**User need:** As a learner or user of Pocket Exhibition Map, I want this small improvement so the behavior is easier to use, explain or verify.

**Feature boundary:** Record observations at 801, 800, 501 and 500 pixels.

**Implementation plan:**

1. Trace `.exhibition and .exhibit-code` and locate the smallest owning file from the code tour. Write how this story touches that responsibility.
2. Write a before/after example that demonstrates this acceptance requirement: Each entry identifies the property and expected arrangement.
3. Choose the input shape, wording or layout policy yourself. Record one alternative and the reason you did not choose it.
4. Implement only the bounded change. If it crosses files, explain what each file owns rather than copying the same decision into several places.
5. Reproduce the acceptance example and one existing boundary case. Add an automated regression for executable logic, or an explicit browser/keyboard/content observation for a static change.
6. Review the diff, explain the change without reading the solution, and record remaining limits.

**Acceptance evidence:** Each entry identifies the property and expected arrangement.

**Left for you:** exact fixture values, names, wording, the implementation and the tradeoff decision. Do not open the hints until you have an example and a first attempt.

**Stretch only after completion:** add one adversarial example that a plausible but incorrect solution would fail. Explain why that example is more informative than adding three ordinary examples.

## Story 04: Improve a long identifier label

**User need:** As a learner or user of Pocket Exhibition Map, I want this small improvement so the behavior is easier to use, explain or verify.

**Feature boundary:** Add descriptive context before the catalogue code without shortening the value.

**Implementation plan:**

1. Trace `.exhibition and .exhibit-code` and locate the smallest owning file from the code tour. Write how this story touches that responsibility.
2. Write a before/after example that demonstrates this acceptance requirement: The full value remains available and its purpose is clear.
3. Choose the input shape, wording or layout policy yourself. Record one alternative and the reason you did not choose it.
4. Implement only the bounded change. If it crosses files, explain what each file owns rather than copying the same decision into several places.
5. Reproduce the acceptance example and one existing boundary case. Add an automated regression for executable logic, or an explicit browser/keyboard/content observation for a static change.
6. Review the diff, explain the change without reading the solution, and record remaining limits.

**Acceptance evidence:** The full value remains available and its purpose is clear.

**Left for you:** exact fixture values, names, wording, the implementation and the tradeoff decision. Do not open the hints until you have an example and a first attempt.

**Stretch only after completion:** add one adversarial example that a plausible but incorrect solution would fail. Explain why that example is more informative than adding three ordinary examples.

## Story 05: Add a reduced-motion policy

**User need:** As a learner or user of Pocket Exhibition Map, I want this small improvement so the behavior is easier to use, explain or verify.

**Feature boundary:** If you experiment with smooth scrolling, add a reduced-motion alternative.

**Implementation plan:**

1. Trace `.exhibition and .exhibit-code` and locate the smallest owning file from the code tour. Write how this story touches that responsibility.
2. Write a before/after example that demonstrates this acceptance requirement: Navigation remains usable with motion reduction enabled.
3. Choose the input shape, wording or layout policy yourself. Record one alternative and the reason you did not choose it.
4. Implement only the bounded change. If it crosses files, explain what each file owns rather than copying the same decision into several places.
5. Reproduce the acceptance example and one existing boundary case. Add an automated regression for executable logic, or an explicit browser/keyboard/content observation for a static change.
6. Review the diff, explain the change without reading the solution, and record remaining limits.

**Acceptance evidence:** Navigation remains usable with motion reduction enabled.

**Left for you:** exact fixture values, names, wording, the implementation and the tradeoff decision. Do not open the hints until you have an example and a first attempt.

**Stretch only after completion:** add one adversarial example that a plausible but incorrect solution would fail. Explain why that example is more informative than adding three ordinary examples.

## Story 06: Improve narrow spacing

**User need:** As a learner or user of Pocket Exhibition Map, I want this small improvement so the behavior is easier to use, explain or verify.

**Feature boundary:** Adjust the 500px rule after inspecting actual content crowding.

**Implementation plan:**

1. Trace `.exhibition and .exhibit-code` and locate the smallest owning file from the code tour. Write how this story touches that responsibility.
2. Write a before/after example that demonstrates this acceptance requirement: No essential content disappears and the reason for the change is recorded.
3. Choose the input shape, wording or layout policy yourself. Record one alternative and the reason you did not choose it.
4. Implement only the bounded change. If it crosses files, explain what each file owns rather than copying the same decision into several places.
5. Reproduce the acceptance example and one existing boundary case. Add an automated regression for executable logic, or an explicit browser/keyboard/content observation for a static change.
6. Review the diff, explain the change without reading the solution, and record remaining limits.

**Acceptance evidence:** No essential content disappears and the reason for the change is recorded.

**Left for you:** exact fixture values, names, wording, the implementation and the tradeoff decision. Do not open the hints until you have an example and a first attempt.

**Stretch only after completion:** add one adversarial example that a plausible but incorrect solution would fail. Explain why that example is more informative than adding three ordinary examples.

<!-- expanded-story-clinics -->

## Additional planning checkpoints for stories 01–06

[Nine more stories, 07–15](11-NINE-MORE-STORIES.md) · [Expanded workshop map](WORKBOOK-INDEX.md)

Keep the original plans above. The following checkpoints add implementation and review depth without completing the exercise for you.

### Story 01 planning clinic: Add a fourth room

**Before editing:** restate the boundary in your own words: Add a room article and its navigation link with a stable ID. Identify the part of `public/style.css` or `public/index.html and public/style.css` that owns it. If your proposed design changes another owner, explain the dependency instead of opening every file for a broad rewrite.

**Acceptance matrix:** write ordinary, boundary and repeat/recovery rows that establish “The link resolves and the article remains readable at 320px.” Include exact starting data or content and the expected retained information. Calculate expected values or inspect meaningful source order independently of the proposed implementation.

**First implementation slice:** make only enough of the change to demonstrate one acceptance row. Inspect the diff and predict the next row before running it. If your first slice is mostly setup or abstraction with no observable result, consider a smaller direct route.

**Review challenge:** sketch a plausible wrong solution that would pass a casual demonstration. Choose a counterexample that exposes its specific weakness. Ask an assistant to critique that example rather than immediately asking it to finish the entire feature.

**Evidence and explanation:** use npm test (local asset references), plus the relevant browser/content observation. Record the actual observation and the limit of the check. Finish by naming a design decision you made yourself and explaining why the neighboring original behavior still holds.

### Story 02 planning clinic: Show a route estimate

**Before editing:** restate the boundary in your own words: Add a short fictional walking-time estimate as ordinary text. Identify the part of `public/style.css` or `public/index.html and public/style.css` that owns it. If your proposed design changes another owner, explain the dependency instead of opening every file for a broad rewrite.

**Acceptance matrix:** write ordinary, boundary and repeat/recovery rows that establish “The estimate does not depend on an image or hover state.” Include exact starting data or content and the expected retained information. Calculate expected values or inspect meaningful source order independently of the proposed implementation.

**First implementation slice:** make only enough of the change to demonstrate one acceptance row. Inspect the diff and predict the next row before running it. If your first slice is mostly setup or abstraction with no observable result, consider a smaller direct route.

**Review challenge:** sketch a plausible wrong solution that would pass a casual demonstration. Choose a counterexample that exposes its specific weakness. Ask an assistant to critique that example rather than immediately asking it to finish the entire feature.

**Evidence and explanation:** use npm test (local asset references), plus the relevant browser/content observation. Record the actual observation and the limit of the check. Finish by naming a design decision you made yourself and explaining why the neighboring original behavior still holds.

### Story 03 planning clinic: Create a boundary checklist

**Before editing:** restate the boundary in your own words: Record observations at 801, 800, 501 and 500 pixels. Identify the part of `public/style.css` or `public/index.html and public/style.css` that owns it. If your proposed design changes another owner, explain the dependency instead of opening every file for a broad rewrite.

**Acceptance matrix:** write ordinary, boundary and repeat/recovery rows that establish “Each entry identifies the property and expected arrangement.” Include exact starting data or content and the expected retained information. Calculate expected values or inspect meaningful source order independently of the proposed implementation.

**First implementation slice:** make only enough of the change to demonstrate one acceptance row. Inspect the diff and predict the next row before running it. If your first slice is mostly setup or abstraction with no observable result, consider a smaller direct route.

**Review challenge:** sketch a plausible wrong solution that would pass a casual demonstration. Choose a counterexample that exposes its specific weakness. Ask an assistant to critique that example rather than immediately asking it to finish the entire feature.

**Evidence and explanation:** use npm test (local asset references), plus the relevant browser/content observation. Record the actual observation and the limit of the check. Finish by naming a design decision you made yourself and explaining why the neighboring original behavior still holds.

### Story 04 planning clinic: Improve a long identifier label

**Before editing:** restate the boundary in your own words: Add descriptive context before the catalogue code without shortening the value. Identify the part of `public/style.css` or `public/index.html and public/style.css` that owns it. If your proposed design changes another owner, explain the dependency instead of opening every file for a broad rewrite.

**Acceptance matrix:** write ordinary, boundary and repeat/recovery rows that establish “The full value remains available and its purpose is clear.” Include exact starting data or content and the expected retained information. Calculate expected values or inspect meaningful source order independently of the proposed implementation.

**First implementation slice:** make only enough of the change to demonstrate one acceptance row. Inspect the diff and predict the next row before running it. If your first slice is mostly setup or abstraction with no observable result, consider a smaller direct route.

**Review challenge:** sketch a plausible wrong solution that would pass a casual demonstration. Choose a counterexample that exposes its specific weakness. Ask an assistant to critique that example rather than immediately asking it to finish the entire feature.

**Evidence and explanation:** use npm test (local asset references), plus the relevant browser/content observation. Record the actual observation and the limit of the check. Finish by naming a design decision you made yourself and explaining why the neighboring original behavior still holds.

### Story 05 planning clinic: Add a reduced-motion policy

**Before editing:** restate the boundary in your own words: If you experiment with smooth scrolling, add a reduced-motion alternative. Identify the part of `public/style.css` or `public/index.html and public/style.css` that owns it. If your proposed design changes another owner, explain the dependency instead of opening every file for a broad rewrite.

**Acceptance matrix:** write ordinary, boundary and repeat/recovery rows that establish “Navigation remains usable with motion reduction enabled.” Include exact starting data or content and the expected retained information. Calculate expected values or inspect meaningful source order independently of the proposed implementation.

**First implementation slice:** make only enough of the change to demonstrate one acceptance row. Inspect the diff and predict the next row before running it. If your first slice is mostly setup or abstraction with no observable result, consider a smaller direct route.

**Review challenge:** sketch a plausible wrong solution that would pass a casual demonstration. Choose a counterexample that exposes its specific weakness. Ask an assistant to critique that example rather than immediately asking it to finish the entire feature.

**Evidence and explanation:** use npm test (local asset references), plus the relevant browser/content observation. Record the actual observation and the limit of the check. Finish by naming a design decision you made yourself and explaining why the neighboring original behavior still holds.

### Story 06 planning clinic: Improve narrow spacing

**Before editing:** restate the boundary in your own words: Adjust the 500px rule after inspecting actual content crowding. Identify the part of `public/style.css` or `public/index.html and public/style.css` that owns it. If your proposed design changes another owner, explain the dependency instead of opening every file for a broad rewrite.

**Acceptance matrix:** write ordinary, boundary and repeat/recovery rows that establish “No essential content disappears and the reason for the change is recorded.” Include exact starting data or content and the expected retained information. Calculate expected values or inspect meaningful source order independently of the proposed implementation.

**First implementation slice:** make only enough of the change to demonstrate one acceptance row. Inspect the diff and predict the next row before running it. If your first slice is mostly setup or abstraction with no observable result, consider a smaller direct route.

**Review challenge:** sketch a plausible wrong solution that would pass a casual demonstration. Choose a counterexample that exposes its specific weakness. Ask an assistant to critique that example rather than immediately asking it to finish the entire feature.

**Evidence and explanation:** use npm test (local asset references), plus the relevant browser/content observation. Record the actual observation and the limit of the check. Finish by naming a design decision you made yourself and explaining why the neighboring original behavior still holds.
