# Game design

## Audience

Players aged roughly 10 and up who have little or no electronics experience.

## Core loop

1. Meet a real-world challenge.
2. Learn what each available component does.
3. Place or connect components on a breadboard.
4. Test the circuit and observe immediate feedback.
5. Diagnose mistakes with progressive hints.
6. Complete the challenge and see a plain-language explanation.

## Level 1: switched light

Scenario: a room needs a light that can be turned on and off.

Required path: battery positive → switch → resistor → LED anode → LED cathode → battery negative. The switch must be closed. The resistor is mandatory because the lesson should teach safe, realistic LED use.

The current prototype simplifies the breadboard so players first learn the idea of a closed circuit. The next version should model connected five-hole rows and separated power rails, then let the player position components in multiple valid layouts.

## Feedback rules

- Highlight one actionable next step, not the full answer.
- Explain incorrect states in terms of current flow and component purpose.
- Never punish experimentation; wires can always be removed or reset.
- Celebrate completion, then ask the player to explain what closing the switch changed.

## Level roadmap

1. Switched LED — closed loops, switch behavior, current limiting.
2. LED polarity — anode/cathode and why direction matters.
3. Two-room lighting — series and parallel circuits.
4. Door alarm — input, buzzer output, and a real-world system.
5. Night light — photoresistor, sensing, and conditional behavior.
