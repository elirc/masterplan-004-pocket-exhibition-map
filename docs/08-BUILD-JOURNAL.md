# Build journal: Pocket Exhibition Map

[Code tour](03-CODE-TOUR.md) · [Actual verification](VERIFICATION.md)

This is a retrospective teaching narrative about the implementation in this repository. It is not a verbatim conversation, fabricated team debate or hidden chain-of-thought transcript. The design explanations below are reviewable rationales tied to the source. Dates and check results belong to the verification record.

## The starting problem

A visitor needs exhibit descriptions that stay readable on a phone or a zoomed desktop.

The main temptation was to make the project larger than its learning target. The useful boundary is **responsive layout and overflow diagnosis**. A finished small example lets you inspect the whole path and ask what each part contributes. Extra infrastructure would add more things to configure before the central idea became clear.

## The first contract

The guide stacks its route and exhibit list at max-width:800px, simplifies navigation at max-width:500px, and wraps the deliberately long catalogue identifier at 320px without hiding it.

The contract turned broad intent into examples that can disagree with an implementation. That matters because a plausible-looking result can hide a wrong boundary rule. The examples in the concepts guide were chosen to expose those distinctions, not to make the demo look flawless.

## Decision note 1: Use the requested breakpoints explicitly

The exact 800px and 500px boundaries connect this reference to the existing exercise. Testing at equality catches mistakes that testing only at a generic phone width would miss.

**What a learner should challenge:** Explain why max-width includes the named width.

**Evidence to consult:** inspect the owning source file, the contract examples and the verification scope. If your alternative satisfies the same behavior with a different structure, compare the maintenance cost instead of assuming one syntax is automatically correct.

## Decision note 2: Repair the cause of overflow

A long unbroken identifier has a large intrinsic minimum width. The content region may shrink and the identifier may wrap; simply hiding overflow would remove information.

**What a learner should challenge:** Distinguish wrapping a token from clipping its tail.

**Evidence to consult:** inspect the owning source file, the contract examples and the verification scope. If your alternative satisfies the same behavior with a different structure, compare the maintenance cost instead of assuming one syntax is automatically correct.

## Decision note 3: Keep the reading order stable

The route precedes the exhibits in HTML and remains first when stacked. The visual arrangement does not require a separate mobile document or duplicate content.

**What a learner should challenge:** Explain what a screen reader or stylesheet-free view encounters first.

**Evidence to consult:** inspect the owning source file, the contract examples and the verification scope. If your alternative satisfies the same behavior with a different structure, compare the maintenance cost instead of assuming one syntax is automatically correct.

## What the checks contributed

The static asset check caught missing local resources, while the browser checks exercised layout, keyboard entry and project-specific content changes. Neither check alone would justify a blanket accessibility claim.

The record in VERIFICATION.md reports actual local observations. A GitHub Actions workflow is provided, but its remote result must be inspected separately after a push. A screenshot documents one rendered state; it is not a substitute for the interaction and boundary checks.

## What you should do differently on your own build

Start from the same user need but write your own examples first. Choose a small variation from the story list. Predict behavior, implement a slice and compare the result with your prediction. The reference helps you judge a finished result; your journal should record your own uncertainties and discoveries rather than adopting this narrative as if you experienced it.

## The handoff

The next learner can start from README, locate `.exhibition and .exhibit-code`, reproduce the example table and attempt one bounded story. That is the intended handoff quality: a working result plus enough evidence and explanation to continue safely. The six practice stories remain unfinished for the learner.
