---
title: Pan Guancheng — AI Agent Researcher
description: Portfolio of Pan Guancheng, a Zhejiang University student and open-source AI agent builder.
hide:
  - navigation
  - toc
  - footer
---

<style>
  .md-content__inner { max-width: 1120px; }
  .pg-resume {
    --pg-ink: #172033;
    --pg-muted: #596579;
    --pg-line: rgba(23, 32, 51, .12);
    --pg-blue: #3859df;
    --pg-violet: #7c3aed;
    color: var(--pg-ink);
    font-family: Inter, "Noto Sans SC", system-ui, sans-serif;
  }
  [data-md-color-scheme="slate"] .pg-resume {
    --pg-ink: #f2f5ff;
    --pg-muted: #b1bad0;
    --pg-line: rgba(255, 255, 255, .14);
  }
  .pg-resume * { box-sizing: border-box; }
  .pg-hero {
    position: relative;
    overflow: hidden;
    padding: clamp(2rem, 6vw, 4.8rem);
    border: 1px solid var(--pg-line);
    border-radius: 28px;
    background:
      radial-gradient(circle at 84% 18%, rgba(124, 58, 237, .22), transparent 32%),
      radial-gradient(circle at 68% 90%, rgba(56, 89, 223, .18), transparent 36%),
      linear-gradient(145deg, rgba(56, 89, 223, .08), rgba(255, 255, 255, .02));
  }
  .pg-hero::after {
    content: "PG";
    position: absolute;
    right: clamp(1rem, 5vw, 4rem);
    bottom: -1.6rem;
    color: rgba(56, 89, 223, .08);
    font-size: clamp(7rem, 20vw, 15rem);
    font-weight: 900;
    letter-spacing: -.08em;
    line-height: 1;
    pointer-events: none;
  }
  .pg-kicker {
    color: var(--pg-blue);
    font-size: .78rem;
    font-weight: 800;
    letter-spacing: .15em;
    text-transform: uppercase;
  }
  .pg-title {
    position: relative;
    z-index: 1;
    margin: .9rem 0 .35rem;
    font-size: clamp(2.7rem, 7vw, 5.6rem);
    font-weight: 850;
    letter-spacing: -.06em;
    line-height: .98;
  }
  .pg-title span {
    display: block;
    margin-top: .75rem;
    color: var(--pg-muted);
    font-size: .27em;
    font-weight: 700;
    letter-spacing: .08em;
    text-transform: uppercase;
  }
  .pg-role {
    position: relative;
    z-index: 1;
    max-width: 760px;
    margin: 1.4rem 0;
    font-size: clamp(1.08rem, 2vw, 1.45rem);
    font-weight: 650;
    line-height: 1.5;
  }
  .pg-summary {
    position: relative;
    z-index: 1;
    max-width: 780px;
    color: var(--pg-muted);
    font-size: 1rem;
    line-height: 1.8;
  }
  .pg-actions { position: relative; z-index: 1; display: flex; flex-wrap: wrap; gap: .7rem; margin-top: 1.7rem; }
  .pg-button {
    display: inline-flex;
    align-items: center;
    min-height: 42px;
    padding: .65rem 1rem;
    border: 1px solid var(--pg-line);
    border-radius: 999px;
    color: var(--pg-ink) !important;
    font-size: .9rem;
    font-weight: 750;
    text-decoration: none;
  }
  .pg-button--primary { border-color: transparent; background: var(--pg-ink); color: white !important; }
  [data-md-color-scheme="slate"] .pg-button--primary { background: #f2f5ff; color: #172033 !important; }
  .pg-section { margin: clamp(3rem, 7vw, 5.5rem) 0; }
  .pg-section-head { display: grid; grid-template-columns: minmax(150px, .38fr) 1fr; gap: 2rem; margin-bottom: 1.4rem; }
  .pg-section-index { color: var(--pg-blue); font-size: .76rem; font-weight: 850; letter-spacing: .12em; text-transform: uppercase; }
  .pg-section h2 { margin: 0; font-size: clamp(1.65rem, 3.2vw, 2.6rem); letter-spacing: -.04em; }
  .pg-section-lead { max-width: 750px; margin: .65rem 0 0; color: var(--pg-muted); line-height: 1.75; }
  .pg-grid { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 1rem; }
  .pg-card {
    display: flex;
    flex-direction: column;
    min-height: 260px;
    padding: 1.45rem;
    border: 1px solid var(--pg-line);
    border-radius: 20px;
    background: rgba(255, 255, 255, .025);
  }
  .pg-card--wide { grid-column: 1 / -1; min-height: auto; }
  .pg-card-label { color: var(--pg-violet); font-size: .74rem; font-weight: 850; letter-spacing: .1em; text-transform: uppercase; }
  .pg-card h3 { margin: .65rem 0 .55rem; font-size: 1.28rem; letter-spacing: -.025em; }
  .pg-card p { margin: 0; color: var(--pg-muted); font-size: .93rem; line-height: 1.7; }
  .pg-card-links { display: flex; flex-wrap: wrap; gap: .8rem; margin-top: auto; padding-top: 1.2rem; }
  .pg-card-links a { color: var(--pg-blue) !important; font-size: .86rem; font-weight: 800; }
  .pg-metrics { display: grid; grid-template-columns: repeat(4, 1fr); gap: 1px; overflow: hidden; margin-top: 1.4rem; border: 1px solid var(--pg-line); border-radius: 18px; background: var(--pg-line); }
  .pg-metric { padding: 1.3rem; background: var(--md-default-bg-color); }
  .pg-metric strong { display: block; font-size: 1.55rem; letter-spacing: -.04em; }
  .pg-metric span { display: block; margin-top: .3rem; color: var(--pg-muted); font-size: .77rem; line-height: 1.45; }
  .pg-proposal {
    padding: clamp(1.7rem, 5vw, 3rem);
    border: 1px solid rgba(56, 89, 223, .3);
    border-radius: 24px;
    background: linear-gradient(135deg, rgba(56, 89, 223, .12), rgba(124, 58, 237, .08));
  }
  .pg-proposal h3 { margin: .35rem 0 .7rem; font-size: clamp(1.5rem, 3vw, 2.2rem); letter-spacing: -.04em; }
  .pg-proposal p { max-width: 820px; color: var(--pg-muted); line-height: 1.8; }
  .pg-deliverables { display: flex; flex-wrap: wrap; gap: .55rem; margin-top: 1.2rem; }
  .pg-chip { padding: .48rem .72rem; border: 1px solid var(--pg-line); border-radius: 999px; font-size: .78rem; font-weight: 750; }
  .pg-footer { display: flex; justify-content: space-between; gap: 2rem; padding: 1.5rem 0 2.5rem; border-top: 1px solid var(--pg-line); color: var(--pg-muted); font-size: .84rem; }
  @media (max-width: 760px) {
    .pg-section-head { grid-template-columns: 1fr; gap: .65rem; }
    .pg-grid { grid-template-columns: 1fr; }
    .pg-card--wide { grid-column: auto; }
    .pg-metrics { grid-template-columns: repeat(2, 1fr); }
    .pg-footer { flex-direction: column; }
  }
</style>

<main class="pg-resume">
  <section class="pg-hero">
    <div class="pg-kicker">Zhejiang University · Hangzhou</div>
    <h1 class="pg-title">潘冠成<span>Pan Guancheng</span></h1>
    <p class="pg-role">Student · Independent AI Agent Researcher · Open-Source Builder</p>
    <p class="pg-summary">
      I build evidence-gated AI agent systems for mathematics, scientific research, and education—making model outputs auditable, reproducible, and safer to deploy. I also turn the engineering process into open-source tools and Chinese technical tutorials.
    </p>
    <div class="pg-actions">
      <a class="pg-button pg-button--primary" href="mailto:3250101086@zju.edu.cn">3250101086@zju.edu.cn</a>
      <a class="pg-button" href="https://github.com/Ephemeral6">GitHub · Ephemeral6</a>
      <a class="pg-button" href="https://ephemeral6.github.io/">Knowledge Garden</a>
    </div>
  </section>

  <section class="pg-section">
    <div class="pg-section-head">
      <div class="pg-section-index">01 · Profile</div>
      <div>
        <h2>From plausible answers to verifiable systems.</h2>
        <p class="pg-section-lead">
          My work focuses on the infrastructure around foundation models: typed problem and evidence graphs, trusted verification boundaries, replayable execution, tool safety, and rigorous evaluation. The goal is not simply to make an agent answer—but to make its reasoning process inspectable and its failures useful.
        </p>
      </div>
    </div>
    <div class="pg-metrics">
      <div class="pg-metric"><strong>127</strong><span>offline tests in the graph-native Math Agent</span></div>
      <div class="pg-metric"><strong>135</strong><span>deterministic fault and replay scenarios</span></div>
      <div class="pg-metric"><strong>12/12</strong><span>AgentFirewall guard tests passed</span></div>
      <div class="pg-metric"><strong>7/7</strong><span>demonstration attacks blocked</span></div>
    </div>
  </section>

  <section class="pg-section">
    <div class="pg-section-head">
      <div class="pg-section-index">02 · Selected Work</div>
      <div>
        <h2>Open-source systems with inspectable evidence.</h2>
        <p class="pg-section-lead">A focused selection across agent infrastructure, safety, knowledge systems, and scientific AI.</p>
      </div>
    </div>
    <div class="pg-grid">
      <article class="pg-card">
        <div class="pg-card-label">Agent Infrastructure</div>
        <h3>Evidence-Gated Agent Stack</h3>
        <p>A graph-native mathematical agent and a general modeling harness built around typed state, evidence freshness, invariant-checked patches, trusted verifiers, and replayable audit trails.</p>
        <div class="pg-card-links">
          <a href="https://github.com/Ephemeral6/math-agent">Math Agent ↗</a>
          <a href="https://github.com/Ephemeral6/modeling-harness">Modeling Harness ↗</a>
        </div>
      </article>
      <article class="pg-card">
        <div class="pg-card-label">Agent Safety</div>
        <h3>AgentFirewall / AgentVault</h3>
        <p>A secure payment layer for AI agents on Monad, combining an MCP server, prompt-injection defenses, policy enforcement, session keys, and on-chain vault controls.</p>
        <div class="pg-card-links"><a href="https://github.com/Ephemeral6/agentfirewall">Repository ↗</a></div>
      </article>
      <article class="pg-card">
        <div class="pg-card-label">Education · Knowledge Systems</div>
        <h3>Knowledge Integrator</h3>
        <p>An LLM and knowledge-graph platform that integrates multiple textbooks, supports large heterogeneous documents, provides hybrid retrieval with citations, and incorporates teacher feedback.</p>
        <div class="pg-card-links"><a href="https://github.com/Ephemeral6/knowledge-integrator-full">Repository ↗</a></div>
      </article>
      <article class="pg-card">
        <div class="pg-card-label">Scientific AI</div>
        <h3>Micro-RAG & Computational Chemistry</h3>
        <p>Domain systems for microbiology retrieval and Text-to-SQL, plus an automation toolkit for molecular enumeration, 3D structure generation, and Gaussian workflows.</p>
        <div class="pg-card-links">
          <a href="https://github.com/Ephemeral6/micro-rag">Micro-RAG ↗</a>
          <a href="https://github.com/Ephemeral6/compchem-toolkit">CompChem Toolkit ↗</a>
        </div>
      </article>
      <article class="pg-card pg-card--wide">
        <div class="pg-card-label">Technical Communication</div>
        <h3>Engineering ideas into reusable methods</h3>
        <p>I write in Chinese about multi-agent systems, RAG, formal reasoning, evaluation, and agent safety. Bake Protocol is one example: a documented workflow for converting visually complex AI-generated HTML into editable presentation decks through selective rasterization.</p>
        <div class="pg-card-links"><a href="https://github.com/Ephemeral6/bake-protocol">Bake Protocol ↗</a></div>
      </article>
    </div>
  </section>

  <section class="pg-section">
    <div class="pg-proposal">
      <div class="pg-section-index">Proposed Kimi Collaboration</div>
      <h3>Kimi Evidence Lab</h3>
      <p>
        A public, reproducible evaluation and teaching platform that connects the Kimi API to my existing Math Agent and Modeling Harness. It would compare bare-model and evidence-gated workflows across mathematics, scientific question answering, and knowledge retrieval—binding conclusions to traces, verifier outputs, latency, cost, and failure analysis.
      </p>
      <div class="pg-deliverables">
        <span class="pg-chip">Open-source Kimi adapter</span>
        <span class="pg-chip">Reproducible task suite</span>
        <span class="pg-chip">Public evaluation reports</span>
        <span class="pg-chip">Chinese tutorials</span>
        <span class="pg-chip">Technical demos</span>
        <span class="pg-chip">Structured product feedback</span>
      </div>
    </div>
  </section>

  <footer class="pg-footer">
    <span>潘冠成 · Pan Guancheng · Hangzhou, China</span>
    <span>Last updated August 2026</span>
  </footer>
</main>
