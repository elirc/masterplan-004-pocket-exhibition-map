# Code tour and architecture decisions

[Overview](../README.md) · [Concepts](02-CONCEPTS-AND-TRACES.md)

| File | Responsibility |
|---|---|
| [package.json](../package.json) | Names the module format, Node requirement and local commands; private prevents npm publication. |
| [.github/workflows/check.yml](../.github/workflows/check.yml) | Runs the committed checks on GitHub. A workflow file is not evidence that a remote run succeeded. |
| [public/index.html](../public/index.html) | Semantic content: room navigation with fragment links, the route aside and exhibit articles. |
| [public/style.css](../public/style.css) | Presentation, focus indication and project-specific layout. |
| [tools/serve.mjs](../tools/serve.mjs) | Local preview infrastructure; only public/ is served. |
| [tools/check-site.mjs](../tools/check-site.mjs) | Checks referenced local assets exist, without pretending to judge usability. |

## Follow one path, not every file

Start at [public/style.css](../public/style.css) and locate `.exhibition and .exhibit-code`. Use this trace as a map: The viewport selects matching media rules → the desktop flex layout becomes block layout at 800px → room navigation links stack at 500px → min-width and overflow-wrap keep the long identifier inside its content box.

The tooling is intentionally separate from the product concept. You can study the local server or CI after the main rule is clear. Neither an HTTP preview server nor a workflow configuration should become a prerequisite for understanding a layout rule.

## Decision: Use the requested breakpoints explicitly

The exact 800px and 500px boundaries connect this reference to the existing exercise. Testing at equality catches mistakes that testing only at a generic phone width would miss.

**Review question:** Explain why max-width includes the named width.

**Your alternative:** Write a plausible different choice, then give a concrete example that reveals its cost. “More scalable” or “cleaner” is not enough; identify a changed dependency, a new state to manage, or a user-visible failure mode.

## Decision: Repair the cause of overflow

A long unbroken identifier has a large intrinsic minimum width. The content region may shrink and the identifier may wrap; simply hiding overflow would remove information.

**Review question:** Distinguish wrapping a token from clipping its tail.

**Your alternative:** Write a plausible different choice, then give a concrete example that reveals its cost. “More scalable” or “cleaner” is not enough; identify a changed dependency, a new state to manage, or a user-visible failure mode.

## Decision: Keep the reading order stable

The route precedes the exhibits in HTML and remains first when stacked. The visual arrangement does not require a separate mobile document or duplicate content.

**Review question:** Explain what a screen reader or stylesheet-free view encounters first.

**Your alternative:** Write a plausible different choice, then give a concrete example that reveals its cost. “More scalable” or “cleaner” is not enough; identify a changed dependency, a new state to manage, or a user-visible failure mode.

## Change boundaries

A small change should begin in the file that owns its meaning. Semantic information belongs in HTML before styling; layout belongs in the relevant CSS rule.

If a story crosses two files, say why. A new section may require markup, a navigation link or a layout rule to change together. That is a coherent feature boundary, not permission to rewrite unrelated parts of the project.

## Deliberate limits

No persistence, external integration or general framework is hidden behind these files. The preview server is a local development aid, not a production hosting system. A browser screenshot is one observation, not proof of every device or assistive technology. Keep these limits visible when describing your own work.
