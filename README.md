# Circuit Quest

Circuit Quest is a beginner-friendly web game that teaches basic electronics by asking players to build useful circuits on a virtual breadboard.

Level 1 introduces a battery, switch, resistor, and LED. Players connect the components into a closed loop and then close the switch to turn on the light. The prototype uses plain HTML, CSS, and JavaScript so a new team can understand and extend it quickly.

## Run locally

No installation is required. Start a local server from the repository root:

```bash
npm start
```

Then open `http://localhost:8080`.

## Level 1 learning goals

- Recognize the positive and negative battery terminals.
- Understand that current needs a complete loop.
- See how a switch opens and closes a circuit.
- Learn that a resistor protects an LED by limiting current.
- Practice mapping component pins to a breadboard-style layout.

## Project files

- `index.html` — accessible game structure and component controls
- `styles.css` — responsive breadboard and component visuals
- `app.js` — wiring interactions, circuit validation, hints, and completion state
- `docs/TEAM_PLAN.md` — four-person work plan and milestone schedule
- `docs/GAME_DESIGN.md` — learning model, Level 1 rules, and roadmap

## Next technical step

Replace the simple connection-list validator with a small graph-based circuit model. Each terminal becomes a graph node, wires become edges, and a level succeeds when a valid powered path exists through the required components. That model will support multiple correct layouts and future levels.

## Contributing

Create short-lived branches named `feature/<description>`, open a pull request, and request one teammate review. Keep game logic, visual components, and lesson content modular so they can be tested independently.

## License

MIT
