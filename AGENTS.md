# COMP 585 UI Game Workflow

**As of:** November 9, 2026

## Document maintenance

- Whenever `AGENTS.md` is modified, update the `As of` date at the top to the date of the change.
- Whenever a website page or file with an `As of` date is modified, update that file's date as part of the same change.
- Preserve historical changelog dates. Do not change them to the current editing date.

## Start every work cycle

- Review the current development website and game repository before proposing implementation or documentation changes. Do not rely solely on previous chats.
- Website source: https://github.com/tklassy/Comp585UIGameWebpage
- Game source: https://github.com/maxisawesome32/COMP585Game
- Live site: https://tklassy.github.io/Comp585UIGameWebpage/
- Read applicable repository instructions, `README.md`, `index.html`, `project.html`, `roadmap.html`, `changelog.html`, relevant styles, and recent commits.
- Review applicable instructions, relevant scripts, project settings, and recent commits in the game repository before proposing game corrections. Use maxisawesome32/COMP585Game as the current game source; older references to tklassy/Comp585Game are outdated.
- If the game repository is inaccessible, state the access gap and use user-provided files or confirmed local work. Do not claim its contents were reviewed.
- Keep website and game repository changes separate. Authorization to edit or push the website does not automatically authorize changes to the game repository.
- Do not require an Assets repository or introduce a source-sync commit marker unless the user requests one.
- Use the user's stated work-cycle date. Interpret timestamps in America/Los_Angeles.
- Distinguish website-documented features, user-reported local work, source-reviewed implementation, planned work, and tested behavior.
- Website documentation alone does not verify the current Unity implementation. If game files or testing evidence are unavailable, state that limitation clearly.

## Project context

- COMP 585 focuses on demonstrating UI/UX concepts through a playable RPG / adventure game.
- The website currently describes an FPS / survival-style Unity prototype using C#, Unity UI, and TextMeshPro.
- Godot and C++ describe the original proposal. Preserve that history without presenting them as the current implementation.
- Documented systems include a grid inventory, eight-slot hotbar, item tooltips, player health and stamina, enemy health bars, ammunition and reload feedback, a no-ammo alert, a radial menu, menu hints, and floating interaction text.
- Recheck the roadmap before describing any feature as complete. Features such as crafting, dialogue, maps, character sheets, expanded settings, and Firebase/web exploration remain planned unless newer evidence establishes otherwise.
- Prioritize readable feedback, intuitive interaction, consistent controls, and appropriate screen-space or world-space presentation.

## Code corrections

- Read the current full script from the game repository or supplied by the user before preparing a correction. Request missing files when they are necessary to preserve behavior.
- Provide complete code-file replacements for Unity C# corrections, including small fixes and large files.
- Identify the exact destination path when known. Do not invent a Unity project path.
- Provide complete compilable contents without omitted sections or placeholder comments.
- Preserve unrelated behavior, class names, serialized fields, Inspector references, and public interfaces unless the requested correction requires changing them.
- Preserve Unity `.meta` files and GUIDs.
- Explain required Inspector assignments, scene setup, prefab changes, UI hierarchy changes, and input configuration separately.
- Match the Unity version and input/UI systems actually used by the project. Verify version-dependent APIs before recommending them.
- Explain the change and how to test it. Distinguish code review from compilation and Unity play testing.

## Changelog format

- Recheck the current site's structure and wording style each cycle.
- Use one section per work-cycle date in newest-first order: `Month D, YYYY`, followed by a short theme description.
- Give each change a concise past-tense action title, such as Added, Updated, Fixed, Implemented, Expanded, or Made.
- Use title-style capitalization and no final period in change titles.
- Group related details beneath the relevant change. Explain behavior and implementation in short complete-sentence paragraphs.
- Preserve the existing expandable HTML structure:
  - `<details class="date-entry">` contains the date `<summary>` and `<span class="date-description">`.
  - `<div class="date-content">` contains individual `<details class="change-entry">` elements.
  - Each change has a `<summary>` title and `<div class="change-documentation">` containing `<p>` paragraphs.
- For chat-only summaries, use the same date, theme, and action titles. For website-ready output, retain the established HTML classes and nesting.
- Do not invent script names, implementation details, test results, or completed features.
- Keep review notes and unresolved questions outside publication-ready entry text.

## Roadmap history

- Preserve the established To Do and Completed sections and their expandable structure.
- Keep older completed milestones even when later work supersedes or improves them.
- Move or add a milestone to Completed only when supported by the user's confirmation or reviewed evidence.
- Keep partially completed work clearly described as unfinished.
- Update related overview and homepage descriptions when an authorized change makes them outdated.
- Preserve the original proposal as historical context.

## Website changes and publishing

- Keep website files read-only during a work cycle. Maintain proposed entries and other drafts separately.
- Update website files at the end of a work cycle only with explicit user permission covering those edits.
- Prepare concrete proposed content and identify affected files before requesting permission so the user can review the result in chat.
- Base end-of-cycle updates on the current website, reviewed game repository changes, user-provided scripts, screenshots, test results, and confirmed work. Re-read newly pushed game commits before documenting them; distinguish pushed changes from local work and do not require a push unless the user makes it part of the cycle.
- Editing permission does not automatically authorize a push. Push, merge, deploy, or publish only when explicitly authorized. A single instruction may authorize both editing and pushing.
- Do not interpret a request to inspect, draft, reformat, or summarize as permission to modify or publish.
- Preserve the static HTML/CSS structure, shared navigation, existing visual style, and homepage development notices unless a requested change requires otherwise.
- Do not introduce a framework, backend, build system, or new dependency without a demonstrated need.
- After authorized edits, review the diff, check relative links and stylesheet paths, test expandable sections, and inspect affected pages at desktop and narrow widths.
- Check that changelog, roadmap, overview, and homepage claims remain consistent.
- Never claim publication succeeded without checking the live result. Report what was edited, pushed, verified, and still pending.

## Project reference material

- Treat synced ChatGPT project files under `sources/` as read-only reference material. Do not edit, rename, move, or delete them.
- Keep generated drafts separate from synced references.
- Preserve unrelated user changes.
