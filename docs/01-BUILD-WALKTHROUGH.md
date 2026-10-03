# Building Pocket Exhibition Map, one decision at a time

[Learning route](00-START-HERE.md) · [Code tour](03-CODE-TOUR.md)

This is a reconstruction of how to approach the finished reference. It explains visible design choices; it is not a transcript of hidden reasoning or a claim that a fictional team performed these steps.

## Start from the contract

The guide stacks its route and exhibit list at max-width:800px, simplifies navigation at max-width:500px, and wraps the deliberately long catalogue identifier at 320px without hiding it.

The smallest useful result answers this user need: A visitor needs exhibit descriptions that stay readable on a phone or a zoomed desktop. Write the examples before choosing file names. Keep the scope small enough that the decisive behavior fits in one trace.

## Step 1: Map content before drawing boxes

The visitor needs a short route and a sequence of rooms. The room links refer to real fragment IDs so they remain useful without JavaScript. The route is supporting information, not a separate interactive map service. Limiting the feature to text and local anchors keeps the responsive behavior directly inspectable.

**Pause and produce evidence:** 801px. Predict the outcome, then compare it with the reference. In your notes, distinguish what the code says should happen from what you actually observed.

## Step 2: Make the desktop relationship explicit

The exhibition container distributes an aside and a content section. The aside takes a bounded share; the section can use the remaining room. Read min-width:0 on the section before examining the long identifier. It gives the section permission to shrink below content-driven minimum sizing, while overflow-wrap decides how the identifier uses that smaller area.

**Pause and produce evidence:** 800px. Predict the outcome, then compare it with the reference. In your notes, distinguish what the code says should happen from what you actually observed.

## Step 3: Inspect equality at each breakpoint

Set the viewport to 801px and then 800px. Repeat around 501px and 500px. Describe the exact property that changes, rather than saying the page becomes mobile. This is the CSS version of a boundary-value test: equality is part of the contract, not an incidental screenshot dimension.

**Pause and produce evidence:** 500px. Predict the outcome, then compare it with the reference. In your notes, distinguish what the code says should happen from what you actually observed.

## Step 4: Debug the deliberate stress content

The catalogue identifier is intentionally longer than ordinary text. Temporarily remove its wrapping rule and inspect the page’s scroll width. Do not solve the problem by deleting the identifier or hiding horizontal overflow. A correct layout keeps the content available and expresses where a break is permitted.

**Pause and produce evidence:** 320px with long identifier. Predict the outcome, then compare it with the reference. In your notes, distinguish what the code says should happen from what you actually observed.

## Keep the implementation reviewable

A useful commit has one understandable reason to exist. Separate the initial working slice, the checks that expose its important boundaries, and the teaching material that explains it. The published commits in this repository were assembled from verified working files; they are real commits, not fabricated evidence of a long historical development process. M001 additionally contains the actual two-file baseline and a separate opening-time correction.

For your own variation, commit at a point where the behavior and evidence agree. Describe the trigger, the resulting behavior and the check in the commit message or review note. Avoid mixing a rule change with unrelated formatting because it makes the learning decision harder to see.

## Stop before adding a platform

The next useful improvement is a sharper example or clearer explanation, not a database, account system or framework migration. Add an abstraction only when it names a real repeated responsibility. You should be able to describe what becomes easier to change after the abstraction and what new complexity it introduces.

**Independent design choice from the original brief:** Decide which information should stack first at narrow widths.

The reference made one choice, documented in the code tour. You may choose differently in a branch if you first revise the contract and acceptance examples. A deliberate alternative is a stronger learning artifact than an unexplained copy.
