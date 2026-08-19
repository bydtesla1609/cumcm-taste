---
name: cumcm-taste
description: Ground mathematical models in real-world facts before selecting methods. Use for CUMCM and other modeling problems involving physical, engineering, environmental, biological, economic, operational, or other real scenarios where omitted constraints, domain effects, thresholds, saturation, regime changes, or questionable assumptions could change the answer. Also use when reviewing whether a proposed model is realistic. Do not add this workflow to pure theorem proving or routine calculations with no material real-world assumptions.
---

# CUMCM Taste

Put facts before methods. Determine what the real system permits, which effects can change the requested result, and which simplifications are defensible before recommending a model.

## Non-negotiable rules

- Do not select or defend a modeling method before completing the method-admission report.
- Separate facts, sourced domain conclusions, calculations, assumptions, and team choices.
- Do not add a factor merely because it exists. Show how it can affect the requested output.
- Do not omit a factor merely because it complicates the solution. Bound or test its impact first.
- Never invent a source, parameter, simulation, independent review, or subagent result.
- Call a result global only when the original feasible region is demonstrably preserved.
- Prefer the smallest model that remains valid within the required error and decision tolerance.

## 1. Check available capabilities

Record whether the current agent can search sources, run calculations, and launch independent subagents.

- If search is unavailable, use only supplied sources and label unanswered domain questions.
- If computation is unavailable, perform a symbolic and dimensional analysis and leave explicit numerical checks.
- For an applicable real-world problem with material domain uncertainty, if subagents are available, launch independent domain research in parallel with the lead agent's scene analysis. Wait for that research before admitting a method.
- If subagents are unavailable, perform the research sequentially and state that it was not independently executed.

Capability loss may reduce confidence; it must not be hidden.

## 2. Reconstruct the problem before researching

List, for every question:

- object and scenario;
- inputs and requested outputs;
- official hard constraints;
- spatial, temporal, unit, and evaluation conventions;
- dependencies between questions;
- facts explicitly given by the problem;
- ambiguities that would materially change the answer.

Do not silently resolve a material ambiguity.

If the problem fully specifies or explicitly excludes every material real-world assumption, issue a brief admission statement and proceed with the ordinary calculation. Do not launch literature research or subagents merely to satisfy the workflow.

## 3. Build a real-world factor inventory

Search or reason about factors not explicitly supplied by the problem. For each candidate factor, report:

- mechanism;
- affected output;
- expected direction of influence;
- plausible magnitude or governing dimensionless ratio;
- conditions under which it matters;
- evidence or calculation supporting the claim;
- proposed treatment.

Include boundaries, conservation laws, capacities, delays, losses, measurement effects, interactions, and initial or terminal conditions when relevant. Avoid generic checklists that are unrelated to the actual output.

## 4. Run independent domain research

When parallel agents are available, give researchers the raw problem and a neutral request. Do not reveal the lead agent's preferred model or desired conclusion.

Require two deliverables:

1. **Background and assumptions:** studied scenario, symbol meanings, assumptions, parameter range, applicability conditions, and source reliability.
2. **Relevant conclusions:** mechanisms that affect this problem, necessary case divisions, thresholds, saturation, reversals, hysteresis, non-monotonicity, or regime changes, plus how each conclusion changes the model.

Read `references/evidence-policy.md` before accepting research claims. Preserve citations and theorem, equation, table, figure, section, or page locators when available.

## 5. Perform a data-free solution rehearsal

Before substituting final data:

- write the minimal governing relationships;
- check units, signs, limiting cases, and conservation requirements;
- verify every classical formula's applicability conditions;
- identify conditions that block the classical route;
- test whether the structure must be piecewise or regime-dependent;
- compare the full candidate model with successively simplified versions;
- identify parameters that cannot be estimated from available evidence.

Use order-of-magnitude estimates, small simulations, sensitivity checks, or upper and lower bounds when tools permit. Do not confuse a small parameter change with a small change in the final decision.

For every numerical demonstration based on values not supplied by the problem, list the assumed parameter values, source or status of each value, and calculation method. Otherwise omit the demonstration.

## 6. Classify every factor

Place each factor in exactly one class:

- **Must model:** omission could change feasibility, ranking, classification, optimum, or the requested conclusion.
- **Test before omitting:** impact is uncertain and needs a bound, sensitivity check, source, or small simulation.
- **May omit:** evidence shows the impact stays below the stated tolerance in the relevant regime.
- **Unresolved:** evidence or capability is insufficient; carry it forward as a risk.

For every omitted factor, state the omission basis and the model's resulting validity range.

## 7. Issue the method-admission report

Use `references/report-template.md`. The report must identify:

- the recommended minimal model;
- retained and omitted factors with reasons;
- required case divisions and switching conditions;
- applicable parameter range;
- unresolved uncertainties;
- evidence strength;
- conditions that require upgrading the model.

Only after this report may the agent choose algorithms, fit parameters, optimize, or write the formal solution.

## 8. Keep the final model concise

Integrate only conclusions that change equations, constraints, cases, parameter ranges, validation, or conclusion strength. Put useful but non-operative background in a short note or omit it.
