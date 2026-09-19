# Four-person team plan

## Shared product goal

Ship a polished Level 1 in two one-week sprints. A first-time player should be able to build a battery → switch → resistor → LED circuit, close the switch, see the LED light, and explain why it works.

## Ownership

### Person 1 — Game systems and integration

- Own the circuit graph, connection rules, level state, reset, and win condition.
- Define stable data shapes for components, terminals, wires, and level definitions.
- Integrate work from the other three owners and maintain the release branch.
- Add unit tests for valid, open, reversed-LED, and short-circuit states.

Deliverables: `circuitEngine.js`, Level 1 configuration, automated logic tests, releases.

### Person 2 — Breadboard interaction and visual design

- Build reusable battery, switch, resistor, LED, terminal, and wire visuals.
- Own click/drag wiring, selected states, wire removal, responsive layout, and animation.
- Research real breadboard row/rail behavior and translate it into a beginner-friendly model.
- Pair with Person 4 on accessible colors, focus styles, and keyboard interaction.

Deliverables: breadboard UI, component library, interaction polish, responsive views.

### Person 3 — Learning design and content

- Write the Level 1 introduction, progressive hints, component explanations, and success recap.
- Define the learning objective and a short pre/post check for playtesting.
- Design Levels 2–4: polarity, series versus parallel, and a real-world alarm circuit.
- Run at least five beginner playtests and summarize where players get stuck.

Deliverables: lesson scripts, hint system content, future-level briefs, playtest report.

### Person 4 — Quality, accessibility, and project operations

- Set up linting, tests, CI, issue templates, and the pull-request checklist.
- Test Chrome, Firefox, Safari, desktop, mobile, keyboard-only use, and screen readers.
- Track bugs and acceptance criteria; verify fixes before merge.
- Own deployment and a short demo script for presenting the project.

Deliverables: CI workflow, QA matrix, accessibility report, deployed demo, demo script.

## Two-sprint schedule

| Time | Person 1 | Person 2 | Person 3 | Person 4 |
|---|---|---|---|---|
| Day 1 | Data model + interfaces | Wireframe + visual system | Learning objectives + copy outline | Repo rules + test plan |
| Days 2–3 | Circuit engine | Core components + wiring | Tutorial and hints | CI + accessibility baseline |
| Days 4–5 | Integrate Level 1 | Responsive polish | Internal playtest | Browser/keyboard testing |
| Days 6–7 | Fix engine issues | Error/success animation | Five user tests | Triage and regression tests |
| Days 8–9 | Future-level support | Final visual polish | Revise content + roadmap | Deploy + demo rehearsal |
| Day 10 | Team bug bash, final acceptance test, release, and retrospective |

## Integration contracts

- Person 1 publishes the component/terminal data model by the end of Day 1.
- Person 2 renders only from that model; visual state does not decide electrical validity.
- Person 3 stores lessons and hints as data, not hard-coded UI fragments.
- Person 4 writes acceptance tests against the shared Level 1 criteria below.
- Everyone opens small pull requests; one review is required, and Person 1 resolves interface conflicts.

## Level 1 acceptance criteria

- The player can connect and remove wires without reloading the page.
- The LED lights only when the circuit is valid and the switch is closed.
- Reversed or incomplete circuits produce a useful, non-punitive hint.
- Every interactive control is usable by keyboard and has a readable label.
- The layout works at 375 px mobile width and common laptop sizes.
- A beginner can complete the level in under five minutes without outside help.

## Suggested issue labels

`area:engine`, `area:ui`, `area:content`, `area:qa`, `type:bug`, `type:feature`, `good-first-issue`, `blocked`, `needs-review`

## Working agreement

- Ten-minute daily check-in: yesterday, today, blocker.
- Decisions affecting interfaces go into a short issue or architecture note.
- Merge only when automated checks pass and acceptance criteria remain true.
- Demo the integrated game twice per week so problems surface early.
