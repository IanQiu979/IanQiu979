# Ian Qiu

**AI security engineer, and an AI product engineer second.**

I work on keeping AI systems inside their boundaries — and I build the products that live inside them.

---

### Security

**[AI Barrier](https://github.com/IanQiu979/ai-barrier-explained)** — agent containment for developer machines *(design write-up; implementation private)*

Keeps local AI coding agents out of folders they have no business reading. Not a policy file they can ignore: a Seatbelt profile on macOS and Landlock on Linux make the boundary a kernel decision, so an agent started through the barrier gets `EPERM` rather than a warning. A root-owned daemon means an agent running as you cannot disable it, edit it, or unlock what it locked. A separate system account makes the protected folder unreadable by construction — no watcher, no sandbox, nothing to bypass.

Verified against real agents, not mocks: Claude Code, Cursor and ChatGPT desktop, every helper process denied.

---

### Products

**[Running Plan Creation](https://github.com/IanQiu979/WorkoutGenerationv2.2)** — AI running-plan generation · React Native · Cloudflare Workers · Supabase

A deterministic engine computes every number in a training plan — distance, pace, heart-rate zone, RPE — from a coaching rule set. The language model is asked only for prose, through a forced tool call whose schema has no numeric field. No model output can change a training number, by construction rather than by review. 900+ tests.

**[Running Form Analysis](https://github.com/IanQiu979/v2.3_RunningFormAna)** — video gait analysis · React Native · Supabase Edge Functions

Scores four running-form pillars from user video, under an honesty contract: a pillar that cannot be assessed says so rather than guessing, and the quota slot is refunded rather than charged. Includes an LLM eval harness, structured-output validation, and reservation semantics with explicit refund paths. 2,500+ tests.

---

### Working together

**Need an app built?** I take on paid builds — mobile and AI-backed products, end to end.

**Collaborations** on interesting projects are welcome.

**Security reviews** scoped to AI agents and AI tooling: agent sandboxing, tool permissions, prompt-to-tool-call boundaries, and what your agent can actually reach.

Email me at [ianqiulillelund@gmail.com](mailto:ianqiulillelund@gmail.com) or [i78979848@gmail.com](mailto:i78979848@gmail.com).

---

### How I work

- A test that cannot fail is not coverage.
- The model writes prose; deterministic code owns every number a user depends on.
- Destructive paths refuse rather than proceed.
