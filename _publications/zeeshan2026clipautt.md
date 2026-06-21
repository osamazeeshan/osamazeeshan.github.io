---
layout: publication
title: CLIP-AUTT: Test-Time Personalization with Action Unit Prompting for Fine-Grained Video Emotion Recognition
bibtex_key: zeeshan2026clipautt
---

<style>
  .clip-autt-page {
    --clip-navy: #111827;
    --clip-blue: #2563eb;
    --clip-cyan: #06b6d4;
    --clip-purple: #7c3aed;
    --clip-ink: #1f2937;
    --clip-muted: #667085;
    --clip-card: rgba(255, 255, 255, 0.88);
    --clip-border: rgba(37, 99, 235, 0.16);
    color: var(--clip-ink);
  }

  .clip-autt-page a {
    color: var(--clip-blue);
  }

  .clip-hero {
    position: relative;
    overflow: hidden;
    margin: 1.5rem 0 2.5rem;
    padding: clamp(2rem, 6vw, 4.5rem) clamp(1rem, 4vw, 3rem);
    border: 1px solid var(--clip-border);
    border-radius: 2rem;
    background:
      radial-gradient(circle at 15% 20%, rgba(6, 182, 212, 0.24), transparent 34%),
      radial-gradient(circle at 85% 12%, rgba(124, 58, 237, 0.20), transparent 30%),
      linear-gradient(135deg, #f8fbff 0%, #eef6ff 48%, #f8f5ff 100%);
    box-shadow: 0 24px 70px rgba(15, 23, 42, 0.12);
    text-align: center;
  }

  .clip-hero::after {
    content: "";
    position: absolute;
    inset: auto -12% -35% -12%;
    height: 55%;
    background: linear-gradient(90deg, rgba(37, 99, 235, 0.10), rgba(6, 182, 212, 0.16), rgba(124, 58, 237, 0.10));
    filter: blur(28px);
  }

  .clip-hero > * {
    position: relative;
    z-index: 1;
  }

  .clip-kicker {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    margin-bottom: 1rem;
    padding: 0.45rem 0.9rem;
    border: 1px solid rgba(37, 99, 235, 0.20);
    border-radius: 999px;
    background: rgba(255, 255, 255, 0.78);
    color: var(--clip-blue);
    font-size: 0.82rem;
    font-weight: 800;
    letter-spacing: 0.08em;
    text-transform: uppercase;
  }

  .clip-title {
    margin: 0;
    color: var(--clip-navy);
    font-size: clamp(3rem, 10vw, 6.25rem);
    font-weight: 900;
    letter-spacing: -0.08em;
    line-height: 0.9;
  }

  .clip-subtitle {
    max-width: 980px;
    margin: 1rem auto 0;
    color: #263348;
    font-size: clamp(1.25rem, 2.5vw, 2rem);
    font-weight: 650;
    line-height: 1.2;
  }

  .clip-authors,
  .clip-affiliation {
    max-width: 920px;
    margin: 1rem auto 0;
    color: var(--clip-muted);
    font-size: 1.02rem;
    line-height: 1.65;
  }

  .clip-authors strong {
    color: var(--clip-ink);
  }

  .clip-badge-row,
  .clip-button-row {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.75rem;
    margin-top: 1.3rem;
  }

  .clip-badge {
    display: inline-flex;
    align-items: center;
    gap: 0.45rem;
    padding: 0.55rem 0.9rem;
    border: 1px solid rgba(17, 24, 39, 0.08);
    border-radius: 999px;
    background: rgba(255, 255, 255, 0.76);
    color: var(--clip-navy);
    font-weight: 750;
  }

  .clip-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-width: 8.5rem;
    padding: 0.78rem 1.15rem;
    border-radius: 999px;
    background: var(--clip-navy);
    color: #fff !important;
    font-weight: 800;
    text-decoration: none !important;
    box-shadow: 0 12px 26px rgba(17, 24, 39, 0.20);
    transition: transform 0.18s ease, box-shadow 0.18s ease;
  }

  .clip-button.secondary {
    background: #fff;
    color: var(--clip-navy) !important;
    border: 1px solid rgba(17, 24, 39, 0.12);
    box-shadow: 0 10px 22px rgba(15, 23, 42, 0.08);
  }

  .clip-button:hover {
    transform: translateY(-2px);
    box-shadow: 0 18px 34px rgba(17, 24, 39, 0.24);
  }

  .clip-nav {
    position: sticky;
    top: 0.75rem;
    z-index: 2;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.45rem;
    margin: 0 auto 2rem;
    padding: 0.45rem;
    border: 1px solid rgba(17, 24, 39, 0.08);
    border-radius: 999px;
    background: rgba(255, 255, 255, 0.86);
    backdrop-filter: blur(16px);
    box-shadow: 0 14px 35px rgba(15, 23, 42, 0.08);
  }

  .clip-nav a {
    padding: 0.5rem 0.8rem;
    border-radius: 999px;
    color: var(--clip-muted);
    font-size: 0.92rem;
    font-weight: 750;
    text-decoration: none !important;
  }

  .clip-nav a:hover {
    background: #eef6ff;
    color: var(--clip-blue);
  }

  .clip-section {
    margin: 2.5rem 0;
  }

  .clip-section h2 {
    margin-bottom: 1rem;
    color: var(--clip-navy);
    font-size: clamp(1.65rem, 3vw, 2.35rem);
    font-weight: 850;
    letter-spacing: -0.035em;
  }

  .clip-section p,
  .clip-section li {
    color: #374151;
    font-size: 1.02rem;
    line-height: 1.75;
  }

  .clip-card-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
    margin-top: 1.25rem;
  }

  .clip-card,
  .clip-figure-card,
  .clip-citation-card {
    border: 1px solid rgba(17, 24, 39, 0.08);
    border-radius: 1.25rem;
    background: var(--clip-card);
    box-shadow: 0 16px 36px rgba(15, 23, 42, 0.07);
  }

  .clip-card {
    padding: 1.25rem;
  }

  .clip-card h3 {
    margin: 0 0 0.5rem;
    color: var(--clip-navy);
    font-size: 1.08rem;
    font-weight: 850;
  }

  .clip-card p {
    margin: 0;
    color: var(--clip-muted);
  }

  .clip-figure-card {
    overflow: hidden;
    padding: clamp(0.75rem, 2vw, 1.25rem);
    background: linear-gradient(180deg, #ffffff 0%, #f8fbff 100%);
  }

  .clip-figure-card img {
    width: 100%;
    border-radius: 1rem;
  }

  .clip-caption {
    margin: 0.85rem 0 0;
    color: var(--clip-muted) !important;
    font-size: 0.95rem !important;
    text-align: center;
  }

  .clip-pill-list {
    display: flex;
    flex-wrap: wrap;
    gap: 0.65rem;
    padding: 0;
    list-style: none;
  }

  .clip-pill-list li {
    padding: 0.55rem 0.85rem;
    border: 1px solid rgba(37, 99, 235, 0.15);
    border-radius: 999px;
    background: #f8fbff;
    color: #263348;
    font-weight: 700;
    line-height: 1.2;
  }

  .clip-citation-card {
    overflow: auto;
    padding: 1rem;
    background: #0f172a;
  }

  .clip-citation-card pre {
    margin: 0;
    color: #dbeafe;
    white-space: pre-wrap;
  }

  @media (max-width: 768px) {
    .clip-card-grid {
      grid-template-columns: 1fr;
    }

    .clip-nav {
      position: static;
      border-radius: 1.25rem;
    }
  }
</style>

<div class="clip-autt-page">
  <section class="clip-hero">
    <div class="clip-kicker">ECCV 2026 · Fine-Grained Video Emotion Recognition</div>
    <h1 class="clip-title">CLIP-AUTT</h1>
    <p class="clip-subtitle">Test-Time Personalization with Action Unit Prompting for Fine-Grained Video Emotion Recognition</p>
    <p class="clip-authors">
      <strong>Muhammad Osama Zeeshan</strong> · Masoumeh Sharafi · Benoît Savary · Alessandro Lameiras Koerich · Marco Pedersoli · Eric Granger
    </p>
    <p class="clip-affiliation">The 19th European Conference on Computer Vision, Malmö, Sweden</p>
    <div class="clip-badge-row">
      <span class="clip-badge">🎭 Action Unit Prompting</span>
      <span class="clip-badge">⏱ Test-Time Personalization</span>
      <span class="clip-badge">🎬 Video Emotion Recognition</span>
    </div>
    <div class="clip-button-row">
      <a class="clip-button" href="https://arxiv.org/pdf/2603.27999">Paper PDF</a>
      <a class="clip-button secondary" href="#citation">Citation</a>
    </div>
  </section>

  <nav class="clip-nav" aria-label="CLIP-AUTT page sections">
    <a href="#abstract">Abstract</a>
    <a href="#method">Method</a>
    <a href="#results">Results</a>
    <a href="#takeaways">Takeaways</a>
    <a href="#citation">Citation</a>
  </nav>

  <section class="clip-section" id="overview">
    <div class="clip-figure-card">
      <img src="{{ '/assets/img/publications/CLIP-AUTT.png' | relative_url }}" alt="CLIP-AUTT method overview">
      <p class="clip-caption">CLIP-AUTT personalizes vision-language emotion recognition at test time with Action Unit prompts and temporal video cues.</p>
    </div>
  </section>

  <section class="clip-section" id="abstract">
    <h2>Abstract</h2>
    <p>
      Fine-grained video emotion recognition requires sensitivity to subtle facial dynamics that differ strongly across people. CLIP-AUTT addresses this challenge by combining CLIP-style vision-language representations with structured facial Action Unit semantics and test-time adaptation for unseen subjects.
    </p>
    <p>
      Instead of depending on noisy generated text prompts or expensive language-model supervision, CLIP-AUTT uses Action Units as interpretable prompts for localized facial muscle activations. The framework first learns subject-agnostic temporal emotion cues with CLIP-AU, then adapts AU prompts during inference to personalize predictions for each target video while maintaining temporal consistency.
    </p>
  </section>

  <section class="clip-section" id="method">
    <h2>Method</h2>
    <div class="clip-card-grid">
      <article class="clip-card">
        <h3>1. AU-guided prompting</h3>
        <p>Facial Action Units provide structured, interpretable language prompts that ground emotion recognition in localized facial movements.</p>
      </article>
      <article class="clip-card">
        <h3>2. Temporal video modeling</h3>
        <p>Video clips are modeled across time so the system can capture gradual expression changes rather than isolated frame-level signals.</p>
      </article>
      <article class="clip-card">
        <h3>3. Test-time personalization</h3>
        <p>Entropy-guided temporal window selection and prompt tuning adapt predictions to subject-specific expression patterns without labeled target data.</p>
      </article>
    </div>
  </section>

  <section class="clip-section" id="results">
    <h2>Evaluation</h2>
    <p>
      CLIP-AU and CLIP-AUTT are evaluated on challenging video-based subtle emotion recognition benchmarks where target subjects can show highly individualized expressive patterns.
    </p>
    <ul class="clip-pill-list">
      <li>BioVid · Pain expression analysis</li>
      <li>StressID · Stress recognition</li>
      <li>BAH · Ambivalence and hesitancy recognition</li>
    </ul>
    <p>
      Across these settings, AU-based prompting and test-time personalization improve robustness compared with state-of-the-art CLIP-based facial expression recognition and test-time adaptation methods.
    </p>
  </section>

  <section class="clip-section" id="takeaways">
    <h2>Key takeaways</h2>
    <div class="clip-card-grid">
      <article class="clip-card">
        <h3>Interpretable</h3>
        <p>Action Unit prompts connect model predictions to recognizable facial muscle movements.</p>
      </article>
      <article class="clip-card">
        <h3>Subject-aware</h3>
        <p>Prompt tuning at inference time personalizes the representation for unseen individuals.</p>
      </article>
      <article class="clip-card">
        <h3>Practical</h3>
        <p>The method targets real-world behavioral analysis where labels are scarce and expressions are subtle.</p>
      </article>
    </div>
  </section>

  <section class="clip-section" id="citation">
    <h2>Citation</h2>
    <div class="clip-citation-card">
<pre><code>@inproceedings{zeeshan2026clipautt,
  title={CLIP-AUTT: Test-Time Personalization with Action Unit Prompting for Fine-Grained Video Emotion Recognition},
  author={Zeeshan, Muhammad Osama and Sharafi, Masoumeh and Savary, Beno{\^i}t and Koerich, Alessandro Lameiras and Pedersoli, Marco and Granger, Eric},
  booktitle={In ECCV 2026: The 19th European Conference on Computer Vision, Malmö, Sweden},
  year={2026}
}</code></pre>
    </div>
  </section>

  <section class="clip-section" id="contact">
    <h2>Contact</h2>
    <p>For questions, discussion, or collaboration, please reach out to the authors.</p>
  </section>
</div>
