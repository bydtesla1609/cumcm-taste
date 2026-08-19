# Acceptance cases

Run these cases with only the user prompt, raw problem material, and installed skill. Do not give the agent the expected findings.

## Case 1: Physical simplification

Ask the agent to model a projectile, vehicle, thermal process, or mechanical system where drag, friction, heat loss, or a boundary may or may not matter.

Pass when the agent estimates or bounds the omitted effect before selecting the model. Fail when it blindly includes every effect or dismisses one without evidence.

## Case 2: Regime change

Use a scenario with a documented threshold, saturation, hysteresis, reversal, or non-monotonic response.

Pass when the agent finds the defining variable, applicable range, case division, and modeling consequence from reliable sources. Fail when it only says that a special effect "may exist."

## Case 3: Simple problem

Use a routine calculation whose relevant facts and assumptions are fully specified.

Pass when the agent performs a short admission check and stops without launching domain research or subagents. Fail when it manufactures unnecessary literature review, capability commentary, or model complexity.

## Case 4: Missing capabilities or evidence

Disable search or subagents, or provide a niche scenario with weak evidence.

Pass when the agent reports the limitation and carries uncertainty forward. Fail when it fabricates research, citations, simulations, or independent agreement.

## Common scoring

Score each item 0 or 1:

- reconstructs the actual problem before choosing a method;
- ties every candidate factor to a requested output;
- distinguishes must-model, test, omit, and unresolved factors;
- captures source setting, assumptions, range, conclusion, and locator;
- checks for thresholds and necessary case divisions;
- performs a data-free rehearsal;
- recommends the smallest defensible model;
- states validity range and upgrade triggers;
- does not overclaim source quality, computation, independence, or optimality.

A release candidate should score at least 8/9 on every case with no fabrication.
