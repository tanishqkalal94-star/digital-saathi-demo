# digital-saathi-demo
Official Digital Saathi demo app for a secure document wallet concept prototype
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="theme-color" content="#f7f9fc">
  <meta name="description" content="Digital Saathi is a concept demo for a consent-first document wallet that helps people organize and selectively share important records.">
  <title>Digital Saathi — Your documents, in your control</title>
  <link rel="icon" href="assets/favicon.svg" type="image/svg+xml">
  <link rel="stylesheet" href="styles.css">
  <script src="script.js" defer></script>
</head>
<body>
  <a class="skip-link" href="#main">Skip to content</a>
  <header class="site-header">
    <div class="container nav-wrap">
      <a class="brand" href="#home" aria-label="Digital Saathi home">
        <span class="brand-mark" aria-hidden="true"><svg viewBox="0 0 32 32"><path d="M16 3 27 9v14l-11 6L5 23V9l11-6Z"/><path d="m11 16 3.2 3.2L21.5 12"/></svg></span>
        <span>Digital <b>Saathi</b></span>
      </a>
      <button class="menu-toggle" aria-expanded="false" aria-controls="primary-nav" aria-label="Open navigation"><span></span><span></span><span></span></button>
      <nav id="primary-nav" class="primary-nav" aria-label="Main navigation">
        <a href="#features">Platform</a><a href="#how-it-works">How it works</a><a href="#centres">For service centres</a><a href="#trust">Trust & safety</a>
        <button class="button button-small button-primary nav-demo" data-open-demo>Explore demo <span aria-hidden="true">↗</span></button>
      </nav>
    </div>
  </header>

  <main id="main">
    <section class="hero section" id="home">
      <div class="container hero-grid">
        <div class="hero-copy">
          <div class="eyebrow"><span class="eyebrow-dot"></span> A concept for simpler document journeys</div>
          <h1>Your documents.<br><span>In your control.</span></h1>
          <p class="hero-lead">A clearer way to organize important records and decide what to share, with whom, and why.</p>
          <div class="hero-actions"><button class="button button-primary" data-open-demo>Explore the demo <span aria-hidden="true">→</span></button><a class="button button-secondary" href="#how-it-works">See how it works</a></div>
          <div class="hero-note"><span class="lock-icon" aria-hidden="true">⌑</span><span>Privacy-minded by design. This website is a demo—not a live document service.</span></div>
        </div>
        <div class="product-scene" aria-label="Illustration of the Digital Saathi demo dashboard">
          <div class="scene-orbit orbit-one"></div><div class="scene-orbit orbit-two"></div>
          <div class="dashboard-card">
            <div class="dashboard-top"><div><span class="dash-greeting">YOUR SPACE</span><h2>Good morning, Asha <span aria-hidden="true">✦</span></h2></div><div class="avatar">A</div></div>
            <div class="dashboard-summary"><div><span class="summary-label">SAVED IN YOUR DEMO</span><strong>4 <small>sample records</small></strong></div><div class="summary-icon" aria-hidden="true">▤</div></div>
            <div class="records-heading"><strong>Recent records</strong><a href="#features">View all <span aria-hidden="true">→</span></a></div>
            <div class="record-row"><span class="record-icon icon-blue" aria-hidden="true">▧</span><span class="record-info"><b>School marks card</b><small>Education · Sample record</small></span><span class="record-arrow" aria-hidden="true">›</span></div>
            <div class="record-row"><span class="record-icon icon-orange" aria-hidden="true">◈</span><span class="record-info"><b>Vaccination record</b><small>Health · Sample record</small></span><span class="record-arrow" aria-hidden="true">›</span></div>
            <div class="record-row"><span class="record-icon icon-green" aria-hidden="true">▱</span><span class="record-info"><b>Residence certificate</b><small>Personal · Sample record</small></span><span class="record-arrow" aria-hidden="true">›</span></div>
            <div class="share-preview"><span class="share-symbol" aria-hidden="true">↗</span><span><b>Sharing stays your choice</b><small>Choose a record, purpose, and expiry.</small></span><span class="share-chevron" aria-hidden="true">→</span></div>
          </div>
          <div class="floating-tag tag-shield"><span aria-hidden="true">✓</span> You choose what to share</div>
          <div class="floating-tag tag-private"><span aria-hidden="true">◉</span> Demo data only</div>
        </div>
      </div>
      <div class="container trust-strip"><span>DESIGNED TO COMPLEMENT</span><i></i><b>DigiLocker</b><b>UIDAI</b><b>APAAR</b><b>ABDM</b><small>Not affiliated with or endorsed by these services</small></div>
    </section>

    <section class="section features-section" id="features">
      <div class="container">
        <div class="section-heading"><div><span class="section-kicker">A more considered wallet</span><h2>Everything starts with<br>clear choices.</h2></div><p>Important documents often sit across different services and life moments. Digital Saathi explores how organizing and sharing them could feel more straightforward.</p></div>
        <div class="feature-grid">
          <article class="feature-card"><div class="feature-icon icon-lavender" aria-hidden="true">▤</div><span class="feature-number">01</span><h3>One organized view</h3><p>Keep a clear catalogue of records by category, with their source and status easy to understand.</p><a href="#how-it-works" aria-label="Learn about organizing documents">Learn more <span>↗</span></a></article>
          <article class="feature-card feature-card-highlight"><div class="feature-icon icon-mint" aria-hidden="true">↗</div><span class="feature-number">02</span><h3>Share with intention</h3><p>Choose a specific record, recipient, and purpose before sharing. A permission should be clear, not a surprise.</p><a href="#how-it-works" aria-label="Learn about selective sharing">Learn more <span>↗</span></a></article>
          <article class="feature-card"><div class="feature-icon icon-peach" aria-hidden="true">◎</div><span class="feature-number">03</span><h3>Know where it came from</h3><p>Distinguish a personal upload from an issuer-provided record or a verified credential.</p><a href="#trust" aria-label="Learn about document provenance">Learn more <span>↗</span></a></article>
        </div>
      </div>
    </section>

    <section class="section process-section" id="how-it-works">
      <div class="container process-grid">
        <div class="process-intro"><span class="section-kicker">Simple by design</span><h2>A thoughtful journey,<br>step by step.</h2><p>The demo shows a possible experience. Real identity checks, official integrations, and secure storage are not implemented here.</p><button class="text-button" data-open-demo>Try the interactive demo <span aria-hidden="true">→</span></button></div>
        <div class="steps">
          <article class="step"><span class="step-count">01</span><div><h3>Organize</h3><p>See sample records grouped by the parts of life they support.</p></div><span class="step-mark" aria-hidden="true">▤</span></article>
          <article class="step"><span class="step-count">02</span><div><h3>Review</h3><p>Check the document source and decide whether it fits your need.</p></div><span class="step-mark" aria-hidden="true">⌕</span></article>
          <article class="step"><span class="step-count">03</span><div><h3>Choose</h3><p>Select what to share, who will receive it, and the intended purpose.</p></div><span class="step-mark" aria-hidden="true">☷</span></article>
          <article class="step"><span class="step-count">04</span><div><h3>Stay informed</h3><p>See a demo activity record of actions taken in this session.</p></div><span class="step-mark" aria-hidden="true">◷</span></article>
        </div>
      </div>
    </section>

    <section class="section centres-section" id="centres">
      <div class="container centres-card">
        <div class="centres-copy"><span class="section-kicker section-kicker-light">Designed for access</span><h2>Digital help,<br>closer to home.</h2><p>The concept includes an assisted journey for people who prefer guidance at a community or online service centre—while keeping decisions and consent with the individual.</p><a class="button button-light" href="#contact">Discuss a pilot <span aria-hidden="true">→</span></a></div>
        <div class="centres-visual" aria-hidden="true"><div class="centre-circle circle-back"></div><div class="centre-circle circle-front"><span class="centre-building">⌂</span><b>ONLINE<br>SERVICE CENTRE</b><small>Assisted digital access</small></div><div class="centre-person person-one">●</div><div class="centre-person person-two">●</div><div class="centre-path"></div></div>
      </div>
    </section>

    <section class="section trust-section" id="trust">
      <div class="container trust-grid">
        <div><span class="section-kicker">Trust is a product feature</span><h2>Built around care,<br>not just convenience.</h2><p class="trust-lead">Sensitive information deserves careful product decisions. Digital Saathi is a concept prototype and does not currently store or process real documents.</p><a class="text-button" href="#limitations">Read demo limitations <span aria-hidden="true">→</span></a></div>
        <div class="trust-points"><article><span class="point-icon">01</span><div><h3>Consent that makes sense</h3><p>Explain what is requested, why it is needed, and who will receive it.</p></div></article><article><span class="point-icon">02</span><div><h3>Clear document provenance</h3><p>Show whether a record is a sample, a user upload, or an issuer-provided item.</p></div></article><article><span class="point-icon">03</span><div><h3>Careful integration choices</h3><p>Any real connection to government platforms requires authorization and separate review.</p></div></article></div>
      </div>
    </section>

    <section class="section demo-cta" id="contact"><div class="container"><div class="cta-panel"><div><span class="section-kicker section-kicker-light">See the concept</span><h2>Explore Digital Saathi.</h2><p>Open the interactive sample flow. It uses fictional examples only and does not upload or save documents.</p></div><button class="button button-light" data-open-demo>Open the demo <span aria-hidden="true">↗</span></button><span class="cta-decoration" aria-hidden="true">D</span></div></div></section>

    <section class="limitations" id="limitations"><div class="container limitations-inner"><span class="warning-icon" aria-hidden="true">i</span><div><b>Prototype notice</b><p>This is an independent concept demo, not an official government website or production service. Do not enter or upload Aadhaar, financial, health, education, or other sensitive personal information. No government APIs are connected, and no document is verified.</p></div></div></section>
  </main>

  <footer class="site-footer"><div class="container footer-top"><a class="brand" href="#home"><span class="brand-mark" aria-hidden="true"><svg viewBox="0 0 32 32"><path d="M16 3 27 9v14l-11 6L5 23V9l11-6Z"/><path d="m11 16 3.2 3.2L21.5 12"/></svg></span><span>Digital <b>Saathi</b></span></a><p>A concept for safer, simpler document journeys.</p><div class="footer-links"><a href="#features">Platform</a><a href="#trust">Trust</a><a href="https://github.com/tanishqkalal94-star/digital-saathi-demo" target="_blank" rel="noopener noreferrer">Project repository ↗</a></div></div><div class="container footer-bottom"><span>© <span id="year"></span> Digital Saathi concept demo</span><span>Independent prototype · Not affiliated with government services</span></div></footer>

  <dialog class="demo-dialog" id="demo-dialog" aria-labelledby="dialog-title">
    <div class="dialog-header"><div><span class="section-kicker">Interactive preview</span><h2 id="dialog-title">A sample sharing flow</h2></div><button class="dialog-close" aria-label="Close demo">×</button></div>
    <p class="dialog-intro">This is a non-functional walkthrough using fictional sample data. Nothing is uploaded or sent.</p>
    <div class="demo-flow"><label for="sample-document">Choose a sample document</label><select id="sample-document"><option>School marks card (fictional)</option><option>Vaccination record (fictional)</option><option>Residence certificate (fictional)</option></select><label for="sample-purpose">Choose a purpose</label><select id="sample-purpose"><option>Education application</option><option>Healthcare appointment</option><option>Identity check</option></select><button class="button button-primary" id="preview-share">Preview sample permission <span aria-hidden="true">→</span></button><div class="demo-result" id="demo-result" role="status" aria-live="polite" hidden></div></div>
    <p class="dialog-footnote">Demo only · No actual sharing, verification, or storage takes place.</p>
  </dialog>
  <div class="toast" id="toast" role="status" aria-live="polite"></div>
</body>
</html>
