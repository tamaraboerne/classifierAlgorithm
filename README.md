# Project: Autonomous Vehicle – *Theoretical* Classifier for Return-to-Base Decision

This repository provides the code and documentation for a simulation of an imagined autonomous vehicle operating within a virtual environment. The project deals exclusively with the decision-making logic that determines when the vehicle ought to return to base to prevent potential, simulated hazards.

---

## Conceptual Scenario (Fully Simulated)

- A fictional autonomous vehicle explores a virtual area.
- In certain simulated situations, exploration should be **terminated** and the vehicle should theoretically **return to base** to avoid imagined damage.
- The return decision is made entirely in software through a **classification algorithm**.

---

## Cost Model (Hypothetical)

In the theoretical scenario, each decision is assigned an artificial cost:

- Continuing exploration when return would have been correct → **Cost = 8**
- Returning at the correct moment → **Cost = 2**
- Returning unnecessarily → **Cost = 4**

**Goal:** Minimize **total simulated cost** through correct classification decisions.

---

## Simulated Sensor Data

- The “vehicle” produces **synthetic sequences of integer measurements**, representing fictional sensor readings.
- These sequences are generated purely in software.
- Example: `49 21 54 35 23 ...`

There is **no real hardware or physical measurement system**.

---

## Classification Task (Theoretical Model)

- The software must decide whether a sequence represents a **dangerous situation** (→ return required) or a **harmless situation** (→ continue).
- Historical simulation data shows differing sequence patterns between dangerous and harmless events.
- A **first-order Markov chain** is used as the classification model.
- Prior probabilities used in the simulation:
  - **90% harmless**
  - **10% dangerous**

---

## Project Objective

- Develop a **software-only classifier** that makes the correct decision about when a hypothetical vehicle should “return to base.”
- Minimize simulated operational costs by avoiding incorrect decisions.

---

## Notes

- This is a **decision-making simulation under uncertainty**.
- The project investigates classification, probability modeling, and Markov chains—not real robotics.
- No hardware, sensors, or real-world data are used; everything is artificially generated and conceptual.
- This project was developed as part of a **university coursework assignment** in the context of a software engineering curriculum.

