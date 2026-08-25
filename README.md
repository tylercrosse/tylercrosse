# 👋 Tyler Crosse

I work on AI safety at AE Studio, mostly alignment, control, and interpretability. Before that I
spent seven years as a senior engineer and team lead. Georgia Tech MSCS.

Most of what I build is tooling. Eval harnesses on the research side, and developer tools for the
agent stack I use every day.

## 📄 Papers

**[Attack Selection in Agentic AI Control Evaluations Meaningfully Decreases Safety](https://arxiv.org/abs/2606.06529)**
(co-first author). An attacker that picks when to attack is much harder to catch than one that
attacks indiscriminately. We split the decision into a start policy and a stop policy, and both drop
measured safety by 20 points or more at a 1% audit budget, even though the monitor never changes.
The project started at MARS 4.0 and continued on contract at Redwood Research.
[Code](https://github.com/tylercrosse/mars-attacks) and
[writeup](https://www.tylercrosse.com/ideas/2026/paper-attack-selection/).

**[When Offline Selectors Cannot Beat the Best Single Model](https://arxiv.org/abs/2606.04161)**
(first author, ICML 2026 DEMO Workshop). A three-stage diagnostic for why learned per-instance model
selection keeps losing to the best single model. On edX dropout prediction the state doesn't carry
enough signal to tell which model will be right, so more tuning doesn't help.

**[Same Facts, Different Updates: Inference Setup Shapes LLM Behavior in Medical Allocation](https://openreview.net/forum?id=z06of44TcG)**
(second author, ICML 2026 AI4GOOD and Pluralistic Alignment Workshops). Identical factual updates
move a model's allocation differently depending on whether it can see its own prior response.

**[Inherited Goal Drift: Contextual Pressure Can Undermine Agentic Goals](https://arxiv.org/abs/2603.03258)**
(ICLR 2026 Lifelong Agents Workshop). Frontier models hold up under direct pressure to abandon a
goal, but they inherit drift when conditioned on prefilled trajectories from weaker agents.

**[Asymmetric Goal Drift in Coding Agents Under Value Conflict](https://arxiv.org/abs/2603.03456)**
(ICLR 2026 Lifelong Agents Workshop). Coding agents violate a system prompt constraint more readily
when it points against a trained-in value like security or privacy.

## 🛠️ Building

[chat-search](https://github.com/tylercrosse/chat-search) is local-first search across ChatGPT,
Claude, Codex, Gemini and OpenCode transcripts, written in Rust. Most of that corpus is already on
disk in open formats, and some of it expires, so a local tool reaches things a browser extension
can't. The archiver runs on a schedule. The index and clients aren't built yet.

[eatwell](https://github.com/tylercrosse/eatwell) is a calorie tracker. Photograph a meal and it
returns calories and macros for each dish, which you edit before logging. It also scans barcodes
against the USDA Branded dataset with an Open Food Facts fallback, and ranks previously logged foods
by frequency with a 14-day recency decay. FastAPI and SQLite behind a Vite and React PWA, deployed as
one Docker service on Fly.io. Still a personal beta with allowlist auth, so there's no public demo.
[Writeup](https://www.tylercrosse.com/ideas/2026/calorie-tracker/).

[cc-usage-bar](https://github.com/tylercrosse/cc-usage-bar) is a macOS menu bar app for Claude Code
and Codex usage. Other tools read the OAuth token out of the Keychain, which prompts the user and
means handing a credential to a third-party process. This one runs the CLIs in a PTY and parses what
they print, so it stores nothing and calls no API.
[Writeup](https://www.tylercrosse.com/ideas/2026/usage-bar/).

[goal-drift-gym](https://github.com/tylercrosse/goal-drift-gym) is a simulation harness for measuring
goal drift in multi-step agents. Seeds, config hashes, and git SHAs go into every artifact so runs
stay reproducible.

[rl-algs](https://github.com/tylercrosse/rl-algs) is a small reproducible suite for reward
misspecification, with mitigations that recover safe behavior.

## ✍️ Writing

I keep a digital garden at [tylercrosse.com](https://www.tylercrosse.com). A few to start with:

- [Persona vectors and the persona selection model](https://www.tylercrosse.com/ideas/2026/persona-vectors/)
- [Transformer Circuits Thread notes](https://www.tylercrosse.com/ideas/2026/transformer-circuits/)
- [Notes on effective ML research](https://www.tylercrosse.com/ideas/2025/ml-research-notes/)
- [How collaborative apps handle conflicting edits](https://www.tylercrosse.com/ideas/2026/real-time-collaboration-contention/)
- [GPU hardware and software](https://www.tylercrosse.com/ideas/2026/gpu-retro/)

## 🔗 Elsewhere

[tylercrosse.com](https://www.tylercrosse.com) &middot; [LinkedIn](https://www.linkedin.com/in/tylercrosse/) &middot; [X](https://x.com/tyler_crosse)
