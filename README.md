# Alan Rocque — About page

Two versions below. Pick one.

---

## Version 1 — Markdown (for Next.js `.mdx`, Astro, or any static-site generator)

```markdown
# Alan Rocque

Hi, I'm Alan. I'm a senior at the University of Wisconsin–Madison studying
Computer Science and Data Science, graduating in May 2026.

I've spent the last three summers as a software engineering intern — at
Amazon in 2025 working on a distributed configuration system on AWS
AppConfig, and at Intel in 2024 and 2023 on anomaly detection for hardware
log files and an internal workflow API. Alongside coursework and research
with UW's Informatics Skunkworks, I build things on the side.

Most of what I build these days sits in the same place: **tooling and
evaluation for the next layer of AI systems.** Memory services for agents,
benchmarks for world models, scaffolding for MCP servers, reproductions of
new research papers. I like the parts of the stack where systems engineering
meets ML — places where a cleanly-designed interface matters as much as the
model behind it.

I'm looking for new-grad software engineering roles starting summer 2026,
especially in ML infrastructure, agent systems, or developer tools. If
you're building in that space, I'd like to hear from you.

## Connect

- Email: <alanrocque@outlook.com>
- GitHub: [alanrocques](https://github.com/alanrocques)
- LinkedIn: [alan-rocque](https://www.linkedin.com/in/alan-rocque)

## Selected projects

- **[Engram](https://github.com/alanrocques/Engram)** — experiential memory
  service for AI agents. Ingests OpenTelemetry traces, distills reusable
  lessons with an LLM, and serves them back at decision time via hybrid
  retrieval. FastAPI + Postgres/pgvector + Celery backend, React dashboard,
  Python SDK, end-to-end tests against Langflow and TestZeus Hercules.

- **[KimiHarness](https://github.com/alanrocques/KimiHarness)** — open-weight
  reproduction of [Meta-Harness](https://arxiv.org/abs/2603.28052), three
  weeks after the paper dropped. Swapped the paper's Claude Opus 4.6 proposer
  for Kimi K2.6 via Moonshot. 0.69 → 1.00 accuracy on Symptom2Disease over
  12 iterations for 73¢.

- **[DreamBench](https://github.com/alanrocques/DreamBench)** — a diagnostic
  benchmark for learned world models (DreamerV3, IRIS, DIAMOND, Δ-IRIS).
  Runs targeted probes for object permanence, physics consistency, reward
  fidelity, and more across Atari, MiniGrid, and Crafter — showing *where*
  a world model's imagination breaks, not just an aggregate score.

- **[create-mcp](https://github.com/alanrocques/create-mcp)** — `npx
  create-mcp@latest` scaffolds a production-ready Model Context Protocol
  server in TypeScript or Python with auth, deployment configs, and passing
  tests.

## Experience

- **Amazon** — SWE Intern, Summer 2025. Distributed configuration system on
  AWS AppConfig; multi-region A/B testing across NA, EU, FE.
- **Intel** — SWE Intern, Summers 2023 & 2024. Anomaly detection on log
  files; internal workflow API migration from NodeJS to NestJS.
- **UW Informatics Skunkworks** — Undergraduate Researcher, 2024–present.
  NBA game-outcome prediction with SVMs and multi-layer perceptrons.
```

---

## Version 2 — Standalone HTML (one file, no dependencies, Walton-minimal)

Save as `index.html` and deploy. Dark, readable, uses system fonts.

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Alan Rocque</title>
  <meta name="description" content="Alan Rocque — CS + Data Science at UW–Madison. Building tooling and evaluation for AI systems.">
  <meta property="og:title" content="Alan Rocque">
  <meta property="og:description" content="CS + Data Science at UW–Madison. Building tooling and evaluation for AI systems.">
  <style>
    :root {
      --bg: #0d0d0f;
      --surface: #17171a;
      --text: #e8e8ea;
      --muted: #9a9aa0;
      --accent: #7cc4ff;
      --border: #26262b;
    }
    @media (prefers-color-scheme: light) {
      :root { --bg: #fafafa; --surface: #fff; --text: #111; --muted: #666; --accent: #0057d9; --border: #e5e5e5; }
    }
    * { box-sizing: border-box; }
    html { -webkit-font-smoothing: antialiased; }
    body {
      background: var(--bg); color: var(--text);
      font: 16px/1.6 -apple-system, BlinkMacSystemFont, "Inter", "Segoe UI", sans-serif;
      margin: 0; padding: 0;
    }
    main { max-width: 640px; margin: 0 auto; padding: 72px 24px 96px; }
    h1 { font-size: 28px; letter-spacing: -0.01em; margin: 0 0 8px; font-weight: 600; }
    .subtitle { color: var(--muted); margin: 0 0 40px; font-size: 15px; }
    h2 { font-size: 13px; text-transform: uppercase; letter-spacing: 0.08em;
         color: var(--muted); margin: 48px 0 16px; font-weight: 600; }
    p { margin: 0 0 16px; }
    a { color: var(--accent); text-decoration: none; }
    a:hover { text-decoration: underline; }
    ul { padding: 0; margin: 0; list-style: none; }
    ul.links li { margin-bottom: 8px; font-size: 15px; }
    ul.projects li { padding: 16px 0; border-bottom: 1px solid var(--border); }
    ul.projects li:last-child { border-bottom: none; }
    ul.projects .name { font-weight: 600; font-size: 15px; }
    ul.projects .desc { color: var(--muted); margin-top: 4px; font-size: 14px; }
    ul.experience li { display: flex; justify-content: space-between; padding: 8px 0;
                       font-size: 14px; gap: 16px; }
    ul.experience li .role { color: var(--muted); }
    code { font-family: ui-monospace, "SF Mono", Menlo, monospace; font-size: 0.92em; }
  </style>
</head>
<body>
<main>
  <h1>Alan Rocque</h1>
  <p class="subtitle">CS + Data Science at UW–Madison, graduating May 2026.</p>

  <p>Hi, I'm Alan. I've spent the last three summers interning at Amazon and Intel, and I build things on the side that usually end up in the same place: <strong>tooling and evaluation for the next layer of AI systems</strong> — memory services for agents, benchmarks for world models, scaffolding for MCP servers, reproductions of new research papers.</p>

  <p>I like the parts of the stack where systems engineering meets ML — where a cleanly-designed interface matters as much as the model behind it.</p>

  <p>Looking for new-grad software engineering roles starting summer 2026, especially in ML infrastructure, agent systems, or developer tools. If you're building in that space, I'd like to hear from you.</p>

  <h2>Connect</h2>
  <ul class="links">
    <li><a href="mailto:alanrocque@outlook.com">alanrocque@outlook.com</a></li>
    <li><a href="https://github.com/alanrocques">github.com/alanrocques</a></li>
    <li><a href="https://www.linkedin.com/in/alan-rocque">linkedin.com/in/alan-rocque</a></li>
  </ul>

  <h2>Selected projects</h2>
  <ul class="projects">
    <li>
      <div class="name"><a href="https://github.com/alanrocques/Engram">Engram</a></div>
      <div class="desc">Experiential memory service for AI agents. Ingests OpenTelemetry traces, distills lessons with an LLM, serves them via hybrid retrieval. FastAPI + Postgres/pgvector backend, React dashboard, Python SDK, end-to-end tests against Langflow and TestZeus Hercules.</div>
    </li>
    <li>
      <div class="name"><a href="https://github.com/alanrocques/KimiHarness">KimiHarness</a></div>
      <div class="desc">Open-weight reproduction of <a href="https://arxiv.org/abs/2603.28052">Meta-Harness</a>, three weeks after the paper dropped. Drove Symptom2Disease classification from 69% to 100% accuracy for 73¢ by swapping the paper's Claude Opus 4.6 proposer for Kimi K2.6.</div>
    </li>
    <li>
      <div class="name"><a href="https://github.com/alanrocques/DreamBench">DreamBench</a></div>
      <div class="desc">Diagnostic benchmark for learned world models (DreamerV3, IRIS, DIAMOND, Δ-IRIS). Runs targeted probes for object permanence, physics, reward fidelity across Atari, MiniGrid, and Crafter — showing <em>where</em> a world model's imagination breaks, not just an aggregate score.</div>
    </li>
    <li>
      <div class="name"><a href="https://github.com/alanrocques/create-mcp">create-mcp</a></div>
      <div class="desc"><code>npx create-mcp@latest</code> scaffolds a production-ready Model Context Protocol server in TypeScript or Python with auth, deployment configs, and passing tests.</div>
    </li>
  </ul>

  <h2>Experience</h2>
  <ul class="experience">
    <li><span>Amazon — SWE Intern</span><span class="role">Summer 2025</span></li>
    <li><span>Intel — SWE Intern</span><span class="role">Summers 2023, 2024</span></li>
    <li><span>UW Informatics Skunkworks — Researcher</span><span class="role">2024–present</span></li>
  </ul>
</main>
</body>
</html>
```

---

## Notes

- **Your GitHub handle on the résumé is `alanrocque` but the actual repos are at `alanrocques`**. The page uses `alanrocques` (plural) everywhere because that's where the code lives. Double-check and update your résumé to match, or fix whichever one is wrong — they have to agree.
- **Opening line doesn't lead with Amazon.** Recruiters will see Amazon within two sentences regardless, and opening with "senior at UW–Madison" sets the right context for everything else. The Walton move — telling the reader what you *do* before what you've *done* — reads better than a brag-stack.
- **"Tooling and evaluation for the next layer of AI systems" is the thesis sentence.** It's what makes four otherwise-different repos read as one coherent point of view instead of a grab-bag.
- **Kept it to four projects.** Your older academic work (Balloc/Bfree, Grocery Inventory Manager) is good for the résumé but would dilute this page. They don't fit the theme.
- **One thing intentionally missing:** a photo. Walton's page doesn't have one either, and for a technical audience it's a neutral-to-positive choice. Add one to the HTML with a 64×64 `<img>` above the `<h1>` if you want it.
