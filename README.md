# Acid–Base Simulator

A small, browser-based chemistry simulator for exploring acid–base reactions and pH behavior in real time.

Built using HTML5 Canvas and vanilla JavaScript. No frameworks, no external libraries.

---

## Features

- Multiple reaction types:
  - Strong acid + strong base (HCl + NaOH)
  - Weak acid + strong base (CH3COOH + NaOH)
  - Strong acid + weak base (HCl + NH3)
  - Additional reactions included

- Real-time pH calculation based on:
  - Equilibrium constants (Ka, Kb)
  - Henderson–Hasselbalch equation
  - Salt hydrolysis
  - Excess reactant concentration

- Particle-based simulation:
  - Molecules move and collide inside a container
  - Reactions occur on collision
  - Reaction rates vary depending on strength (strong vs weak)

- Interactive controls:
  - Adjust acid and base quantities while the simulation is running
  - Start, pause, and reset the system

- Live data:
  - pH value and classification (acidic, neutral, basic)
  - Ion concentrations [H⁺] and [OH⁻]
  - Remaining reactants and products formed

- Event log for tracking reaction progress

---

## How it works

Each particle represents approximately 0.001 mol/L.

The simulation models real chemical behavior:

- Strong acids and bases fully dissociate
- Weak acids and bases partially dissociate using Ka/Kb values
- pH is calculated depending on the system:
  - Strong + strong: based on excess H⁺ or OH⁻
  - Weak + strong: buffer region handled using Henderson–Hasselbalch
  - Equivalence point: includes salt hydrolysis where applicable

Water autoionization is included using:

Kw = 1 × 10⁻¹⁴ (at 25°C)

---

## Getting started

No installation required.

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/acid-base-simulator.git
   cd acid-base-simulator
   ```

2. Open the project:
   - Open `index.html` in your browser

That’s it.

---

## Usage

1. Select a reaction from the dropdown menu
2. Set the number of acid and base particles
3. Click "Start"
4. Observe how the system evolves:
   - pH changes over time
   - Particles collide and react
   - Products form dynamically

You can change values while the simulation is running.

---

## Tech stack

- HTML5 Canvas
- Vanilla JavaScript
- CSS

---

## Author

Mohammad Imad Ahmed  
11th grade student

---

## Possible improvements

- Titration curve visualization
- Temperature effects
- More reaction types
- Performance optimizations for larger particle counts
- Mobile support
