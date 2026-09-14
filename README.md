<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta
    name="description"
    content="Keyur Modi — Data Scientist, Machine Learning Engineer, and AI Researcher."
  >
  <meta name="author" content="Keyur Modi">
  <title>Keyur Modi | Data Scientist · ML Engineer · AI Researcher</title>

  <style>
    :root {
      --bg: #0b0f14;
      --surface: #111720;
      --surface-2: #151d28;
      --border: #263241;
      --text: #edf2f7;
      --muted: #9aa8b8;
      --accent: #4fc3f7;
      --accent-2: #7c9cff;
      --max-width: 1120px;
      --radius: 16px;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family:
        Inter,
        ui-sans-serif,
        system-ui,
        -apple-system,
        BlinkMacSystemFont,
        "Segoe UI",
        sans-serif;
      background:
        radial-gradient(circle at 80% 0%, rgba(79, 195, 247, 0.08), transparent 28%),
        radial-gradient(circle at 10% 20%, rgba(124, 156, 255, 0.06), transparent 25%),
        var(--bg);
      color: var(--text);
      line-height: 1.7;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    .container {
      width: min(100% - 40px, var(--max-width));
      margin: auto;
    }

    header {
      min-height: 88vh;
      display: flex;
      align-items: center;
      border-bottom: 1px solid var(--border);
    }

    .hero {
      max-width: 850px;
      padding: 80px 0;
    }

    .eyebrow {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      color: var(--accent);
      font-size: 0.85rem;
      font-weight: 700;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      margin-bottom: 22px;
    }

    .eyebrow::before {
      content: "";
      width: 28px;
      height: 1px;
      background: var(--accent);
    }

    h1 {
      font-size: clamp(3.2rem, 9vw, 6.5rem);
      line-height: 0.95;
      letter-spacing: -0.055em;
      margin-bottom: 28px;
    }

    .hero-title {
      font-size: clamp(1.25rem, 3vw, 2rem);
      color: var(--muted);
      max-width: 760px;
      margin-bottom: 28px;
    }

    .hero-title strong {
      color: var(--text);
    }

    .hero-description {
      max-width: 760px;
      color: var(--muted);
      font-size: 1.05rem;
    }

    .links {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
      margin-top: 34px;
    }

    .button {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      min-height: 44px;
      padding: 0 18px;
      border: 1px solid var(--border);
      border-radius: 10px;
      background: var(--surface);
      color: var(--text);
      font-size: 0.9rem;
      font-weight: 650;
      transition: 0.2s ease;
    }

    .button:hover {
      border-color: var(--accent);
      color: var(--accent);
      transform: translateY(-2px);
    }

    .button.primary {
      background: var(--accent);
      color: #061018;
      border-color: var(--accent);
    }

    .button.primary:hover {
      color: #061018;
      opacity: 0.9;
    }

    section {
      padding: 90px 0;
      border-bottom: 1px solid var(--border);
    }

    .section-heading {
      display: grid;
      grid-template-columns: 260px 1fr;
      gap: 50px;
      margin-bottom: 48px;
    }

    .section-number {
      color: var(--accent);
      font-family: monospace;
      font-size: 0.8rem;
      letter-spacing: 0.1em;
    }

    h2 {
      font-size: clamp(2rem, 4vw, 3rem);
      line-height: 1.1;
      letter-spacing: -0.035em;
    }

    .section-intro {
      color: var(--muted);
      max-width: 700px;
      margin-top: 14px;
    }

    .about {
      max-width: 820px;
      margin-left: 310px;
      color: var(--muted);
      font-size: 1.08rem;
    }

    .about p + p {
      margin-top: 18px;
    }

    .skills {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 16px;
    }

    .skill-card {
      padding: 24px;
      border: 1px solid var(--border);
      background: rgba(17, 23, 32, 0.7);
      border-radius: var(--radius);
    }

    .skill-card h3 {
      margin-bottom: 10px;
      font-size: 1rem;
    }

    .skill-card p {
      color: var(--muted);
      font-size: 0.93rem;
    }

    .projects {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 18px;
    }

    .project {
      display: flex;
      flex-direction: column;
      min-height: 300px;
      padding: 30px;
      border: 1px solid var(--border);
      background: linear-gradient(
        145deg,
        rgba(21, 29, 40, 0.9),
        rgba(17, 23, 32, 0.75)
      );
      border-radius: var(--radius);
      transition: 0.25s ease;
    }

    .project:hover {
      transform: translateY(-5px);
      border-color: rgba(79, 195, 247, 0.5);
    }

    .project-index {
      color: var(--accent);
      font-family: monospace;
      font-size: 0.8rem;
      margin-bottom: 26px;
    }

    .project h3 {
      font-size: 1.35rem;
      margin-bottom: 12px;
    }

    .project p {
      color: var(--muted);
      font-size: 0.94rem;
    }

    .project-meta {
      margin-top: auto;
      padding-top: 24px;
      display: flex;
      justify-content: space-between;
      gap: 16px;
      align-items: center;
    }

    .tags {
      display: flex;
      flex-wrap: wrap;
      gap: 7px;
    }

    .tag {
      border: 1px solid var(--border);
      border-radius: 999px;
      padding: 4px 9px;
      color: var(--muted);
      font-size: 0.72rem;
      font-family: monospace;
    }

    .project-link {
      color: var(--accent);
      white-space: nowrap;
      font-size: 0.85rem;
      font-weight: 700;
    }

    .timeline {
      position: relative;
      display: grid;
      gap: 34px;
    }

    .timeline-item {
      display: grid;
      grid-template-columns: 230px 1fr;
      gap: 45px;
    }

    .timeline-label {
      color: var(--accent);
      font-family: monospace;
      font-size: 0.82rem;
    }

    .timeline-content h3 {
      font-size: 1.3rem;
      margin-bottom: 4px;
    }

    .timeline-content .organization {
      color: var(--muted);
      margin-bottom: 12px;
    }

    .timeline-content p {
      color: var(--muted);
    }

    .education {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 18px;
    }

    .education-card {
      padding: 30px;
      border: 1px solid var(--border);
      border-radius: var(--radius);
      background: var(--surface);
    }

    .education-card .degree {
      color: var(--accent);
      font-size: 0.78rem;
      font-family: monospace;
      text-transform: uppercase;
      letter-spacing: 0.08em;
    }

    .education-card h3 {
      margin: 12px 0 6px;
      font-size: 1.25rem;
    }

    .education-card p {
      color: var(--muted);
    }

    .certifications {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    .certificate {
      padding: 10px 14px;
      border: 1px solid var(--border);
      border-radius: 10px;
      background: var(--surface);
      color: var(--muted);
      font-size: 0.88rem;
    }

    .publication {
      max-width: 850px;
      padding: 34px;
      border: 1px solid var(--border);
      border-radius: var(--radius);
      background: var(--surface);
    }

    .publication-label {
      color: var(--accent);
      font-family: monospace;
      font-size: 0.78rem;
      text-transform: uppercase;
      letter-spacing: 0.08em;
    }

    .publication h3 {
      margin: 12px 0;
      font-size: 1.5rem;
    }

    .publication p {
      color: var(--muted);
    }

    .publication a {
      display: inline-block;
      margin-top: 18px;
      color: var(--accent);
      font-weight: 700;
    }

    .contact {
      text-align: center;
      max-width: 760px;
      margin: auto;
    }

    .contact h2 {
      margin-bottom: 18px;
    }

    .contact p {
      color: var(--muted);
      margin-bottom: 28px;
    }

    footer {
      padding: 32px 0;
      color: var(--muted);
      font-size: 0.8rem;
    }

    footer .container {
      display: flex;
      justify-content: space-between;
      gap: 20px;
      flex-wrap: wrap;
    }

    @media (max-width: 850px) {
      .section-heading {
        grid-template-columns: 1fr;
        gap: 12px;
      }

      .about {
        margin-left: 0;
      }

      .skills,
      .projects,
      .education {
        grid-template-columns: 1fr;
      }

      .timeline-item {
        grid-template-columns: 1fr;
        gap: 8px;
      }
    }

    @media (max-width: 600px) {
      .container {
        width: min(100% - 28px, var(--max-width));
      }

      header {
        min-height: auto;
      }

      .hero {
        padding: 65px 0;
      }

      section {
        padding: 65px 0;
      }

      .project {
        min-height: auto;
      }

      .project-meta {
        flex-direction: column;
        align-items: flex-start;
      }
    }
  </style>
</head>

<body>

  <header>
    <div class="container">
      <div class="hero">
        <div class="eyebrow">Data · Intelligence · Research · Engineering</div>

        <h1>Keyur Modi</h1>

        <p class="hero-title">
          <strong>Data Scientist</strong> · Machine Learning Engineer · AI Researcher
        </p>

        <p class="hero-description">
          I build production machine learning systems and research-driven AI solutions
          across predictive modeling, deep learning, NLP, generative AI, similarity
          search, model evaluation, and MLOps. My work spans the full ML lifecycle —
          from data engineering and experimentation to deployment, monitoring, and
          optimization. I am particularly interested in building intelligent systems
          that are scalable, explainable, robust, and useful in real-world environments.
        </p>

        <div class="links">
          <a
            class="button primary"
            href="https://github.com/keyur462"
            target="_blank"
            rel="noopener noreferrer"
          >
            GitHub
          </a>

          <a
            class="button"
            href="https://www.linkedin.com/in/keyurmodi004"
            target="_blank"
            rel="noopener noreferrer"
          >
            LinkedIn
          </a>

          <a
            class="button"
            href="mailto:modikeyur938@gmail.com"
          >
            Email
          </a>

          <a
            class="button"
            href="https://www.acigjournal.com/Building-Trustworthy-Autonomous-AI-Essential-Principles-beyond-Traditional-Software,208710,0,2.html"
            target="_blank"
            rel="noopener noreferrer"
          >
            Research Paper
          </a>
        </div>
      </div>
    </div>
  </header>

  <main>

    <section id="about">
      <div class="container">
        <div class="section-heading">
          <div class="section-number">01 / ABOUT</div>

          <div>
            <h2>Engineering intelligence from data.</h2>
            <p class="section-intro">
              A technical profile built around applied machine learning,
              research, and production engineering.
            </p>
          </div>
        </div>

        <div class="about">
          <p>
            I am a Data Scientist and Machine Learning Engineer with 4+ years of
            hands-on experience developing, evaluating, and deploying machine
            learning models, deep learning systems, statistical solutions, and
            data-driven applications.
          </p>

          <p>
            My technical work covers Python and SQL, supervised and unsupervised
            learning, gradient boosting, deep learning, NLP, Transformers,
            LLMs, vector search, time-series modeling, anomaly detection,
            explainable AI, and cloud-based ML systems.
          </p>

          <p>
            Alongside industry experience, I have worked in academic research at
            the University of Texas at San Antonio on similarity search,
            multimodal retrieval, anomaly detection, scalable data processing,
            and trustworthy AI evaluation. I also contribute to teaching,
            student communities, research initiatives, and community-focused
            volunteer work.
          </p>
        </div>
      </div>
    </section>

    <section id="skills">
      <div class="container">
        <div class="section-heading">
          <div class="section-number">02 / EXPERTISE</div>

          <div>
            <h2>Technical capabilities.</h2>
            <p class="section-intro">
              A combination of modeling depth, software engineering,
              data infrastructure, and production ML.
            </p>
          </div>
        </div>

        <div class="skills">

          <article class="skill-card">
            <h3>Machine Learning & Statistical Modeling</h3>
            <p>
              Supervised and unsupervised learning, XGBoost, LightGBM,
              Random Forest, Logistic Regression, feature engineering,
              model selection, statistical modeling, and evaluation.
            </p>
          </article>

          <article class="skill-card">
            <h3>Deep Learning & AI</h3>
            <p>
              PyTorch, TensorFlow, Keras, neural networks, LSTMs, VAEs,
              representation learning, deep learning architectures,
              and intelligent decision systems.
            </p>
          </article>

          <article class="skill-card">
            <h3>NLP, LLMs & Generative AI</h3>
            <p>
              Transformers, Hugging Face, spaCy, NLTK, LLMs, fine-tuning,
              prompt engineering, embeddings, semantic retrieval, and RAG.
            </p>
          </article>

          <article class="skill-card">
            <h3>Similarity & Retrieval</h3>
            <p>
              FAISS, HNSW, NMSLIB, vector indexing, multimodal retrieval,
              similarity search, Jaro-Winkler, graph matching, and
              large-scale nearest-neighbor systems.
            </p>
          </article>

          <article class="skill-card">
            <h3>Data Engineering</h3>
            <p>
              Pandas, NumPy, SciPy, PySpark, ETL, data pipelines,
              preprocessing, feature extraction, PostgreSQL, MySQL,
              MongoDB, and Redis.
            </p>
          </article>

          <article class="skill-card">
            <h3>MLOps & Cloud</h3>
            <p>
              AWS, SageMaker, Lambda, S3, EC2, CloudWatch, GCP,
              BigQuery, Vertex AI, Azure AI, Docker, Kubernetes,
              GitHub Actions, GitLab CI, and Jenkins.
            </p>
          </article>

          <article class="skill-card">
            <h3>Model Evaluation & Trustworthy AI</h3>
            <p>
              SHAP, interpretability, model robustness, bias auditing,
              distribution-shift analysis, prediction stability,
              monitoring, and production model validation.
            </p>
          </article>

          <article class="skill-card">
            <h3>Analytics & Visualization</h3>
            <p>
              Power BI, Tableau, Matplotlib, Seaborn, SQL analytics,
              KPI development, data exploration, and decision-support
              dashboards.
            </p>
          </article>

        </div>
      </div>
    </section>

    <section id="projects">
      <div class="container">
        <div class="section-heading">
          <div class="section-number">03 / SELECTED WORK</div>

          <div>
            <h2>Projects that turn ideas into systems.</h2>
            <p class="section-intro">
              Selected work across AI, retrieval, healthcare intelligence,
              financial modeling, and applied machine learning.
            </p>
          </div>
        </div>

        <div class="projects">

          <article class="project">
            <div class="project-index">PROJECT / 01</div>

            <h3>Healthcare Decision Intelligence</h3>

            <p>
              A unified AI decision stack designed to process healthcare
              scenarios through seven intelligent layers, producing
              auditable and explainable decisions across treatment and
              reasoning workflows.
            </p>

            <div class="project-meta">
              <div class="tags">
                <span class="tag">Python</span>
                <span class="tag">AI</span>
                <span class="tag">Decision Systems</span>
              </div>

              <a
                class="project-link"
                href="https://github.com/keyur462/healthcare-decision-intelligence"
                target="_blank"
                rel="noopener noreferrer"
              >
                Repository →
              </a>
            </div>
          </article>

          <article class="project">
            <div class="project-index">PROJECT / 02</div>

            <h3>Multimodal Vector Retrieval Engine</h3>

            <p>
              A cross-modal retrieval system embedding image features and
              textual metadata into a shared vector space, using FAISS
              indexing for high-performance similarity search across
              large-scale embeddings.
            </p>

            <div class="project-meta">
              <div class="tags">
                <span class="tag">PyTorch</span>
                <span class="tag">FAISS</span>
                <span class="tag">Hugging Face</span>
                <span class="tag">Docker</span>
              </div>

              <a
                class="project-link"
                href="https://github.com/keyur462/skyline_project"
                target="_blank"
                rel="noopener noreferrer"
              >
                Repository →
              </a>
            </div>
          </article>

          <article class="project">
            <div class="project-index">PROJECT / 03</div>

            <h3>SmartDocs RAG Chatbot</h3
