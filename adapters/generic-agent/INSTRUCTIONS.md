# Generic-agent adapter

Read `../../skill/cumcm-taste/SKILL.md` as the controlling workflow. Load the referenced evidence policy and report template when instructed.

Treat imperative statements in the skill as mandatory unless they conflict with the user's instructions or the host system's safety rules. Map `search`, `calculation`, and `subagent` to the equivalent capabilities of the current agent platform.

If a capability is unavailable, follow the skill's documented fallback and disclose the limitation. Do not claim that a source was checked, a calculation was run, or an independent agent was consulted unless it actually occurred.

Return the Markdown method-admission report by default. Return data conforming to `../../skill/cumcm-taste/references/output-schema.json` when the caller requests structured output.

