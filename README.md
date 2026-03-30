<!-- ████████████████████████████████████████████████████ -->
<!--         SOHAM SHARMA — GITHUB PROFILE README         -->
<!-- ████████████████████████████████████████████████████ -->

<div align="center">

<!-- ===== ANIMATED HERO BANNER ===== -->
<svg width="900" height="300" viewBox="0 0 900 300" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#020817"/>
      <stop offset="50%" style="stop-color:#0a1628"/>
      <stop offset="100%" style="stop-color:#041424"/>
    </linearGradient>
    <radialGradient id="glow1" cx="20%" cy="40%" r="45%">
      <stop offset="0%" style="stop-color:#06b6d4;stop-opacity:0.2"/>
      <stop offset="100%" style="stop-color:#06b6d4;stop-opacity:0"/>
    </radialGradient>
    <radialGradient id="glow2" cx="80%" cy="60%" r="45%">
      <stop offset="0%" style="stop-color:#8b5cf6;stop-opacity:0.15"/>
      <stop offset="100%" style="stop-color:#8b5cf6;stop-opacity:0"/>
    </radialGradient>
    <radialGradient id="glow3" cx="50%" cy="20%" r="30%">
      <stop offset="0%" style="stop-color:#fbbf24;stop-opacity:0.08"/>
      <stop offset="100%" style="stop-color:#fbbf24;stop-opacity:0"/>
    </radialGradient>
    <linearGradient id="titleGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#67e8f9"/>
      <stop offset="45%" style="stop-color:#ffffff"/>
      <stop offset="100%" style="stop-color:#a78bfa"/>
    </linearGradient>
    <linearGradient id="subGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#06b6d4"/>
      <stop offset="100%" style="stop-color:#8b5cf6"/>
    </linearGradient>
    <linearGradient id="lineGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#06b6d4;stop-opacity:0"/>
      <stop offset="50%" style="stop-color:#06b6d4;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#8b5cf6;stop-opacity:0"/>
    </linearGradient>
    <linearGradient id="lineGrad2" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#8b5cf6;stop-opacity:0"/>
      <stop offset="50%" style="stop-color:#fbbf24;stop-opacity:0.6"/>
      <stop offset="100%" style="stop-color:#06b6d4;stop-opacity:0"/>
    </linearGradient>
    <filter id="softglow">
      <feGaussianBlur stdDeviation="2.5" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="blur1"><feGaussianBlur stdDeviation="1.8"/></filter>
  </defs>

  <!-- Background -->
  <rect width="900" height="300" fill="url(#bg)" rx="16"/>
  <rect width="900" height="300" fill="url(#glow1)" rx="16"/>
  <rect width="900" height="300" fill="url(#glow2)" rx="16"/>
  <rect width="900" height="300" fill="url(#glow3)" rx="16"/>

  <!-- Animated grid -->
  <g stroke="#06b6d4" stroke-width="0.4" opacity="0.08">
    <line x1="0" y1="60" x2="900" y2="60"/><line x1="0" y1="120" x2="900" y2="120"/>
    <line x1="0" y1="180" x2="900" y2="180"/><line x1="0" y1="240" x2="900" y2="240"/>
    <line x1="180" y1="0" x2="180" y2="300"/><line x1="360" y1="0" x2="360" y2="300"/>
    <line x1="540" y1="0" x2="540" y2="300"/><line x1="720" y1="0" x2="720" y2="300"/>
  </g>

  <!-- Floating particles -->
  <g filter="url(#blur1)">
    <circle cx="70" cy="55" r="2.5" fill="#06b6d4" opacity="0.9">
      <animate attributeName="cy" values="55;35;55" dur="4s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.9;0.3;0.9" dur="4s" repeatCount="indefinite"/>
    </circle>
    <circle cx="830" cy="70" r="2" fill="#a78bfa" opacity="0.8">
      <animate attributeName="cy" values="70;50;70" dur="5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.8;0.2;0.8" dur="5s" repeatCount="indefinite"/>
    </circle>
    <circle cx="150" cy="220" r="2.5" fill="#06b6d4" opacity="0.6">
      <animate attributeName="cy" values="220;240;220" dur="6s" repeatCount="indefinite"/>
    </circle>
    <circle cx="750" cy="240" r="2" fill="#a78bfa" opacity="0.7">
      <animate attributeName="cy" values="240;220;240" dur="4.5s" repeatCount="indefinite"/>
    </circle>
    <circle cx="450" cy="25" r="3" fill="#67e8f9" opacity="0.5">
      <animate attributeName="cy" values="25;45;25" dur="7s" repeatCount="indefinite"/>
    </circle>
    <circle cx="300" cy="270" r="1.5" fill="#fbbf24" opacity="0.6">
      <animate attributeName="cx" values="300;320;300" dur="5s" repeatCount="indefinite"/>
    </circle>
    <circle cx="600" cy="40" r="1.5" fill="#34d399" opacity="0.5">
      <animate attributeName="cy" values="40;55;40" dur="3.5s" repeatCount="indefinite"/>
    </circle>
    <circle cx="860" cy="160" r="2" fill="#06b6d4" opacity="0.6">
      <animate attributeName="cx" values="860;840;860" dur="4s" repeatCount="indefinite"/>
    </circle>
    <circle cx="40" cy="140" r="1.5" fill="#c4b5fd" opacity="0.7">
      <animate attributeName="cx" values="40;58;40" dur="5s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- Animated corner brackets -->
  <g stroke="#06b6d4" stroke-width="2" fill="none">
    <polyline points="16,44 16,16 44,16" opacity="0.5">
      <animate attributeName="opacity" values="0.5;1;0.5" dur="2.5s" repeatCount="indefinite"/>
    </polyline>
    <polyline points="856,16 884,16 884,44" opacity="0.5">
      <animate attributeName="opacity" values="0.5;1;0.5" dur="2.5s" begin="0.6s" repeatCount="indefinite"/>
    </polyline>
    <polyline points="16,256 16,284 44,284" opacity="0.5">
      <animate attributeName="opacity" values="0.5;1;0.5" dur="2.5s" begin="1.2s" repeatCount="indefinite"/>
    </polyline>
    <polyline points="856,284 884,284 884,256" opacity="0.5">
      <animate attributeName="opacity" values="0.5;1;0.5" dur="2.5s" begin="1.8s" repeatCount="indefinite"/>
    </polyline>
  </g>

  <!-- Animated horizontal lines -->
  <line x1="60" y1="210" x2="840" y2="210" stroke="url(#lineGrad)" stroke-width="1" opacity="0.4">
    <animate attributeName="opacity" values="0.3;0.8;0.3" dur="3s" repeatCount="indefinite"/>
  </line>
  <line x1="120" y1="76" x2="780" y2="76" stroke="url(#lineGrad2)" stroke-width="0.5" opacity="0.2">
    <animate attributeName="opacity" values="0.1;0.4;0.1" dur="4s" repeatCount="indefinite"/>
  </line>

  <!-- Status indicator -->
  <circle cx="450" cy="40" r="4" fill="#22c55e" opacity="0.9">
    <animate attributeName="r" values="3;5;3" dur="2s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.9;0.5;0.9" dur="2s" repeatCount="indefinite"/>
  </circle>
  <text x="450" y="56" text-anchor="middle" font-family="'Courier New',monospace" font-size="9" fill="#22c55e" letter-spacing="2" opacity="0.8">OPEN FOR COLLABORATION</text>

  <!-- Main title -->
  <text x="450" y="118" text-anchor="middle" font-family="'Courier New',monospace" font-size="60" font-weight="900" fill="url(#titleGrad)" filter="url(#softglow)" letter-spacing="6">SOHAM SHARMA</text>

  <!-- Subtitle -->
  <text x="450" y="152" text-anchor="middle" font-family="'Courier New',monospace" font-size="14" fill="url(#subGrad)" letter-spacing="3" font-weight="600">GenAI Architect · AI/ML Engineer · AWS Solutions Architect</text>

  <!-- Tagline -->
  <text x="450" y="182" text-anchor="middle" font-family="'Courier New',monospace" font-size="12" fill="#64748b" letter-spacing="1.5">Aircraft Engineer → GenAI Architect  |  11+ Years  |  Indore, India</text>

  <!-- Stats boxes -->
  <g transform="translate(90,224)">
    <!-- Box 1 -->
    <rect x="0" y="0" width="132" height="52" rx="8" fill="#06b6d408" stroke="#06b6d4" stroke-width="0.8"/>
    <text x="66" y="18" text-anchor="middle" font-family="monospace" font-size="8" fill="#94a3b8" letter-spacing="1.5">CORPORATE CLIENTS</text>
    <text x="66" y="39" text-anchor="middle" font-family="monospace" font-size="20" font-weight="bold" fill="#06b6d4">20+</text>

    <!-- Box 2 -->
    <rect x="148" y="0" width="132" height="52" rx="8" fill="#8b5cf608" stroke="#8b5cf6" stroke-width="0.8"/>
    <text x="214" y="18" text-anchor="middle" font-family="monospace" font-size="8" fill="#94a3b8" letter-spacing="1.5">SATISFACTION RATE</text>
    <text x="214" y="39" text-anchor="middle" font-family="monospace" font-size="20" font-weight="bold" fill="#a78bfa">95%</text>

    <!-- Box 3 -->
    <rect x="296" y="0" width="132" height="52" rx="8" fill="#10b98108" stroke="#10b981" stroke-width="0.8"/>
    <text x="362" y="18" text-anchor="middle" font-family="monospace" font-size="8" fill="#94a3b8" letter-spacing="1.5">MONTHLY READERS</text>
    <text x="362" y="39" text-anchor="middle" font-family="monospace" font-size="20" font-weight="bold" fill="#34d399">10K+</text>

    <!-- Box 4 -->
    <rect x="444" y="0" width="132" height="52" rx="8" fill="#f59e0b08" stroke="#f59e0b" stroke-width="0.8"/>
    <text x="510" y="18" text-anchor="middle" font-family="monospace" font-size="8" fill="#94a3b8" letter-spacing="1.5">INSTITUTIONS</text>
    <text x="510" y="39" text-anchor="middle" font-family="monospace" font-size="20" font-weight="bold" fill="#fbbf24">15+</text>

    <!-- Box 5 -->
    <rect x="592" y="0" width="132" height="52" rx="8" fill="#ec489908" stroke="#ec4899" stroke-width="0.8"/>
    <text x="658" y="18" text-anchor="middle" font-family="monospace" font-size="8" fill="#94a3b8" letter-spacing="1.5">YEARS EXPERIENCE</text>
    <text x="658" y="39" text-anchor="middle" font-family="monospace" font-size="20" font-weight="bold" fill="#f472b6">11+</text>
  </g>
</svg>

<br/>

<!-- Social Badges -->
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/soham-sharma/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sohamnsharma@gmail.com)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](http://www.medium.com/@sohamnsharma)
[![Twitter](https://img.shields.io/badge/Twitter-%231DA1F2.svg?style=for-the-badge&logo=Twitter&logoColor=white)](https://www.twitter.com/sohamnsharma)
[![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)](https://www.youtube.com/c/UC9i2PROUgpxGIaDu-Argdjw)
[![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/sohamnsharma)
[![Profile Views](https://komarev.com/ghpvc/?username=soham2710&label=Profile+Views&color=0891b2&style=for-the-badge)](https://github.com/soham2710)

</div>

---

## `> whoami`

```python
class SohamSharma:
    name         = "Soham Sharma"
    based_in     = "Indore, India 🇮🇳"
    experience   = "11+ years across IT, AI/ML & Enterprise"
    current      = "AI Product Manager & Architect @ IntelliPaaS Inc."
    past         = ["Botmartz", "Ziplyne Inc.", "Powerweave", "Genesys Intl."]
    education    = ["PG Diploma Applied Statistics — IGNOU",
                    "B.E. Aircraft Maintenance — Singhania University"]
    languages    = ["English", "Hindi", "Gujarati", "French"]
    superpower   = "From inspecting aircraft engines ✈️ → building AI engines 🤖"

    focus = [
        "🧠 LLM Ecosystems & Foundation Models",
        "🕸️  Agentic AI & Multi-Agent Orchestration",
        "🔍 RAG Architectures & Retrieval Systems",
        "☁️  Cloud-Native AI (AWS · Azure · GCP)",
        "⚙️  MLOps / LLMOps & AI Lifecycle",
    ]

    def quote(self):
        return "Don't just use AI. Architect it. Ship it. Scale it."
```

---

## `> skills --all`

<div align="center">

<!-- ===== SKILLS PANEL ===== -->
<svg width="880" height="440" viewBox="0 0 880 440" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="sbg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#020817"/>
      <stop offset="100%" style="stop-color:#0a1628"/>
    </linearGradient>
    <linearGradient id="cyanBar" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#06b6d4"/><stop offset="100%" style="stop-color:#0e7490"/>
    </linearGradient>
    <linearGradient id="purpleBar" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#8b5cf6"/><stop offset="100%" style="stop-color:#6d28d9"/>
    </linearGradient>
    <linearGradient id="greenBar" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#10b981"/><stop offset="100%" style="stop-color:#047857"/>
    </linearGradient>
    <linearGradient id="goldBar" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#f59e0b"/><stop offset="100%" style="stop-color:#b45309"/>
    </linearGradient>
  </defs>
  <rect width="880" height="440" fill="url(#sbg)" rx="16"/>

  <!-- ===== CARD 1: GenAI & LLMs ===== -->
  <rect x="16" y="16" width="420" height="198" rx="12" fill="#06b6d406" stroke="#06b6d4" stroke-width="0.8"/>
  <rect x="16" y="16" width="4" height="198" rx="2" fill="url(#cyanBar)"/>
  <text x="38" y="44" font-family="monospace" font-size="11" font-weight="bold" fill="#06b6d4" letter-spacing="2">🤖  GENERATIVE AI &amp; LLMs</text>
  <!-- Row 1: Models -->
  <g font-family="monospace" font-size="10" fill="#e2e8f0">
    <rect x="34" y="56" width="66" height="22" rx="11" fill="#06b6d418" stroke="#06b6d440" stroke-width="0.7"/><text x="67" y="71" text-anchor="middle">GPT-4o</text>
    <rect x="108" y="56" width="66" height="22" rx="11" fill="#06b6d418" stroke="#06b6d440" stroke-width="0.7"/><text x="141" y="71" text-anchor="middle">Claude 3</text>
    <rect x="182" y="56" width="78" height="22" rx="11" fill="#06b6d418" stroke="#06b6d440" stroke-width="0.7"/><text x="221" y="71" text-anchor="middle">Gemini Pro</text>
    <rect x="268" y="56" width="56" height="22" rx="11" fill="#06b6d418" stroke="#06b6d440" stroke-width="0.7"/><text x="296" y="71" text-anchor="middle">LLaMA</text>
    <rect x="332" y="56" width="58" height="22" rx="11" fill="#06b6d418" stroke="#06b6d440" stroke-width="0.7"/><text x="361" y="71" text-anchor="middle">Mistral</text>
    <!-- Row 2: Frameworks -->
    <rect x="34" y="86" width="80" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="74" y="101" text-anchor="middle">LangChain</text>
    <rect x="122" y="86" width="80" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="162" y="101" text-anchor="middle">LangGraph</text>
    <rect x="210" y="86" width="68" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="244" y="101" text-anchor="middle">AutoGen</text>
    <rect x="286" y="86" width="60" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="316" y="101" text-anchor="middle">CrewAI</text>
    <rect x="354" y="86" width="54" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="381" y="101" text-anchor="middle">ReAct</text>
    <!-- Row 3: RAG -->
    <rect x="34" y="116" width="82" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="75" y="131" text-anchor="middle">LlamaIndex</text>
    <rect x="124" y="116" width="54" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="151" y="131" text-anchor="middle">FAISS</text>
    <rect x="186" y="116" width="70" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="221" y="131" text-anchor="middle">Pinecone</text>
    <rect x="264" y="116" width="64" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="296" y="131" text-anchor="middle">Chroma</text>
    <rect x="336" y="116" width="72" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="372" y="131" text-anchor="middle">Haystack</text>
    <!-- Row 4: Fine-tuning -->
    <rect x="34" y="146" width="50" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="59" y="161" text-anchor="middle">LoRA</text>
    <rect x="92" y="146" width="60" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="122" y="161" text-anchor="middle">QLoRA</text>
    <rect x="160" y="146" width="50" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="185" y="161" text-anchor="middle">PEFT</text>
    <rect x="218" y="146" width="100" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="268" y="161" text-anchor="middle">Prompt Eng.</text>
    <rect x="326" y="146" width="86" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="369" y="161" text-anchor="middle">HuggingFace</text>
  </g>
  <text x="34" y="200" font-family="monospace" font-size="8.5" fill="#475569" letter-spacing="1">RAG · AGENTIC AI · FINE-TUNING · MULTIMODAL · VECTOR SEARCH</text>

  <!-- ===== CARD 2: Cloud & MLOps ===== -->
  <rect x="444" y="16" width="420" height="198" rx="12" fill="#8b5cf606" stroke="#8b5cf6" stroke-width="0.8"/>
  <rect x="444" y="16" width="4" height="198" rx="2" fill="url(#purpleBar)"/>
  <text x="466" y="44" font-family="monospace" font-size="11" font-weight="bold" fill="#a78bfa" letter-spacing="2">☁️  CLOUD &amp; MLOPS</text>
  <g font-family="monospace" font-size="10" fill="#e2e8f0">
    <rect x="462" y="56" width="48" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="486" y="71" text-anchor="middle">AWS</text>
    <rect x="518" y="56" width="80" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="558" y="71" text-anchor="middle">SageMaker</text>
    <rect x="606" y="56" width="72" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="642" y="71" text-anchor="middle">Bedrock</text>
    <rect x="686" y="56" width="72" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="722" y="71" text-anchor="middle">Azure ML</text>
    <rect x="766" y="56" width="72" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="802" y="71" text-anchor="middle">Vertex AI</text>

    <rect x="462" y="86" width="62" height="22" rx="11" fill="#06b6d418" stroke="#06b6d440" stroke-width="0.7"/><text x="493" y="101" text-anchor="middle">Docker</text>
    <rect x="532" y="86" width="84" height="22" rx="11" fill="#06b6d418" stroke="#06b6d440" stroke-width="0.7"/><text x="574" y="101" text-anchor="middle">Kubernetes</text>
    <rect x="624" y="86" width="76" height="22" rx="11" fill="#06b6d418" stroke="#06b6d440" stroke-width="0.7"/><text x="662" y="101" text-anchor="middle">Terraform</text>
    <rect x="708" y="86" width="100" height="22" rx="11" fill="#06b6d418" stroke="#06b6d440" stroke-width="0.7"/><text x="758" y="101" text-anchor="middle">GitHub Actions</text>

    <rect x="462" y="116" width="62" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="493" y="131" text-anchor="middle">MLflow</text>
    <rect x="532" y="116" width="48" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="556" y="131" text-anchor="middle">W&amp;B</text>
    <rect x="588" y="116" width="80" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="628" y="131" text-anchor="middle">LangSmith</text>
    <rect x="676" y="116" width="92" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="722" y="131" text-anchor="middle">PromptLayer</text>

    <rect x="462" y="146" width="82" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="503" y="161" text-anchor="middle">CloudWatch</text>
    <rect x="552" y="146" width="82" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="593" y="161" text-anchor="middle">Prometheus</text>
    <rect x="642" y="146" width="66" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="675" y="161" text-anchor="middle">Grafana</text>
  </g>
  <text x="466" y="200" font-family="monospace" font-size="8.5" fill="#475569" letter-spacing="1">AWS · AZURE · GCP · CI/CD · MLOPS · LLMOPS · OBSERVABILITY</text>

  <!-- ===== CARD 3: Full Stack ===== -->
  <rect x="16" y="226" width="420" height="198" rx="12" fill="#10b98106" stroke="#10b981" stroke-width="0.8"/>
  <rect x="16" y="226" width="4" height="198" rx="2" fill="url(#greenBar)"/>
  <text x="38" y="254" font-family="monospace" font-size="11" font-weight="bold" fill="#34d399" letter-spacing="2">🛠️  FULL STACK DEVELOPMENT</text>
  <g font-family="monospace" font-size="10" fill="#e2e8f0">
    <rect x="34" y="266" width="62" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="65" y="281" text-anchor="middle">Python</text>
    <rect x="104" y="266" width="62" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="135" y="281" text-anchor="middle">Django</text>
    <rect x="174" y="266" width="62" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="205" y="281" text-anchor="middle">FastAPI</text>
    <rect x="244" y="266" width="52" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="270" y="281" text-anchor="middle">Flask</text>
    <rect x="304" y="266" width="66" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="337" y="281" text-anchor="middle">Node.js</text>

    <rect x="34" y="296" width="56" height="22" rx="11" fill="#06b6d418" stroke="#06b6d440" stroke-width="0.7"/><text x="62" y="311" text-anchor="middle">React</text>
    <rect x="98" y="296" width="62" height="22" rx="11" fill="#06b6d418" stroke="#06b6d440" stroke-width="0.7"/><text x="129" y="311" text-anchor="middle">Next.js</text>
    <rect x="168" y="296" width="86" height="22" rx="11" fill="#06b6d418" stroke="#06b6d440" stroke-width="0.7"/><text x="211" y="311" text-anchor="middle">TailwindCSS</text>
    <rect x="262" y="296" width="78" height="22" rx="11" fill="#06b6d418" stroke="#06b6d440" stroke-width="0.7"/><text x="301" y="311" text-anchor="middle">AngularJS</text>

    <rect x="34" y="326" width="82" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="75" y="341" text-anchor="middle">PostgreSQL</text>
    <rect x="124" y="326" width="72" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="160" y="341" text-anchor="middle">MongoDB</text>
    <rect x="204" y="326" width="52" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="230" y="341" text-anchor="middle">Redis</text>
    <rect x="264" y="326" width="66" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="297" y="341" text-anchor="middle">Firebase</text>
    <rect x="338" y="326" width="60" height="22" rx="11" fill="#8b5cf618" stroke="#8b5cf640" stroke-width="0.7"/><text x="368" y="341" text-anchor="middle">MySQL</text>

    <rect x="34" y="356" width="66" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="67" y="371" text-anchor="middle">PyTorch</text>
    <rect x="108" y="356" width="86" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="151" y="371" text-anchor="middle">TensorFlow</text>
    <rect x="202" y="356" width="56" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="230" y="371" text-anchor="middle">Keras</text>
    <rect x="266" y="356" width="82" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="307" y="371" text-anchor="middle">Scikit-learn</text>
  </g>

  <!-- ===== CARD 4: Data, BI & Certs ===== -->
  <rect x="444" y="226" width="420" height="198" rx="12" fill="#f59e0b06" stroke="#f59e0b" stroke-width="0.8"/>
  <rect x="444" y="226" width="4" height="198" rx="2" fill="url(#goldBar)"/>
  <text x="466" y="254" font-family="monospace" font-size="11" font-weight="bold" fill="#fbbf24" letter-spacing="2">📊  DATA, BI &amp; CERTIFICATIONS</text>
  <g font-family="monospace" font-size="10" fill="#e2e8f0">
    <rect x="462" y="266" width="66" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="495" y="281" text-anchor="middle">Tableau</text>
    <rect x="536" y="266" width="66" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="569" y="281" text-anchor="middle">Power BI</text>
    <rect x="610" y="266" width="56" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="638" y="281" text-anchor="middle">R Lang</text>
    <rect x="674" y="266" width="62" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="705" y="281" text-anchor="middle">Jupyter</text>
    <rect x="744" y="266" width="50" height="22" rx="11" fill="#f59e0b18" stroke="#f59e0b40" stroke-width="0.7"/><text x="769" y="281" text-anchor="middle">QGIS</text>

    <rect x="462" y="296" width="46" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="485" y="311" text-anchor="middle">Git</text>
    <rect x="516" y="296" width="56" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="544" y="311" text-anchor="middle">Figma</text>
    <rect x="580" y="296" width="70" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="615" y="311" text-anchor="middle">Postman</text>
    <rect x="658" y="296" width="58" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="687" y="311" text-anchor="middle">NGINX</text>
    <rect x="724" y="296" width="76" height="22" rx="11" fill="#10b98118" stroke="#10b98140" stroke-width="0.7"/><text x="762" y="311" text-anchor="middle">Bootstrap</text>
  </g>
  <text x="466" y="340" font-family="monospace" font-size="10" font-weight="bold" fill="#fbbf24">🏅 CERTIFICATIONS</text>
  <text x="466" y="358" font-family="monospace" font-size="9" fill="#94a3b8">AWS Solutions Architect · Six Sigma Green Belt</text>
  <text x="466" y="374" font-family="monospace" font-size="9" fill="#94a3b8">MongoDB Python Dev · Python DS/ML · PostgreSQL</text>
  <text x="466" y="390" font-family="monospace" font-size="9" fill="#94a3b8">Complete SQL · PowerBI + Tableau · Product Mgmt</text>
</svg>

</div>

---

## `> github --stats`

<div align="center">

<a href="https://github.com/soham2710">
<img height="180em" src="https://github-readme-stats.vercel.app/api?username=soham2710&show_icons=true&count_private=true&title_color=06b6d4&text_color=ffffff&icon_color=a78bfa&bg_color=020817&hide_border=true&border_radius=12&rank_icon=github&include_all_commits=true" alt="GitHub Stats"/>
</a>
<a href="https://github.com/soham2710">
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=soham2710&langs_count=8&title_color=06b6d4&text_color=ffffff&icon_color=a78bfa&bg_color=020817&hide_border=true&border_radius=12&layout=compact" alt="Top Languages"/>
</a>

<br/>

<img width="70%" src="https://github-readme-streak-stats.herokuapp.com/?user=soham2710&theme=transparent&hide_border=true&stroke=0891b2&ring=06b6d4&fire=a78bfa&currStreakNum=ffffff&currStreakLabel=06b6d4&sideNums=ffffff&sideLabels=94a3b8&dates=64748b&background=020817&border_radius=12" alt="GitHub Streak"/>

<br/>

<img width="96%" src="https://github-readme-activity-graph.vercel.app/graph?username=soham2710&bg_color=020817&color=06b6d4&line=0891b2&point=a78bfa&area=true&area_color=06b6d420&hide_border=true&radius=12" alt="Activity Graph"/>

</div>

---

## `> history --career`

<div align="center">

<!-- ===== CAREER TIMELINE ===== -->
<svg width="880" height="380" viewBox="0 0 880 380" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="tbg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#020817"/>
      <stop offset="100%" style="stop-color:#0a1628"/>
    </linearGradient>
    <linearGradient id="tline" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#06b6d4"/>
      <stop offset="50%" style="stop-color:#8b5cf6"/>
      <stop offset="100%" style="stop-color:#fbbf24"/>
    </linearGradient>
    <filter id="ng">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>
  <rect width="880" height="380" fill="url(#tbg)" rx="16"/>

  <!-- Animated dashed timeline -->
  <line x1="60" y1="185" x2="830" y2="185" stroke="url(#tline)" stroke-width="2" stroke-dasharray="10 5" opacity="0.6">
    <animate attributeName="stroke-dashoffset" values="0;-30" dur="2s" repeatCount="indefinite"/>
  </line>

  <!-- Node 1: Education -->
  <circle cx="95" cy="185" r="22" fill="#020817" stroke="#06b6d4" stroke-width="2" filter="url(#ng)">
    <animate attributeName="r" values="22;25;22" dur="4s" repeatCount="indefinite"/>
  </circle>
  <text x="95" y="191" text-anchor="middle" font-size="16">✈️</text>
  <text x="95" y="222" text-anchor="middle" font-family="monospace" font-size="8" fill="#94a3b8" letter-spacing="1">2012–16</text>
  <text x="95" y="236" text-anchor="middle" font-family="monospace" font-size="10" font-weight="bold" fill="#e2e8f0">Aircraft</text>
  <text x="95" y="249" text-anchor="middle" font-family="monospace" font-size="10" fill="#e2e8f0">Engineer</text>
  <text x="95" y="152" text-anchor="middle" font-family="monospace" font-size="8" fill="#64748b">Singhania</text>
  <text x="95" y="140" text-anchor="middle" font-family="monospace" font-size="8" fill="#64748b">University</text>

  <text x="152" y="189" text-anchor="middle" font-size="14" fill="#06b6d4" opacity="0.5">→</text>

  <!-- Node 2: Genesys -->
  <circle cx="215" cy="185" r="22" fill="#020817" stroke="#8b5cf6" stroke-width="2" filter="url(#ng)">
    <animate attributeName="r" values="22;25;22" dur="4s" begin="0.5s" repeatCount="indefinite"/>
  </circle>
  <text x="215" y="191" text-anchor="middle" font-size="16">🌍</text>
  <text x="215" y="222" text-anchor="middle" font-family="monospace" font-size="8" fill="#94a3b8" letter-spacing="1">2017–19</text>
  <text x="215" y="236" text-anchor="middle" font-family="monospace" font-size="10" font-weight="bold" fill="#e2e8f0">GIS &amp; QC</text>
  <text x="215" y="249" text-anchor="middle" font-family="monospace" font-size="10" fill="#e2e8f0">Trainer</text>
  <text x="215" y="152" text-anchor="middle" font-family="monospace" font-size="8" fill="#64748b">Genesys</text>
  <text x="215" y="140" text-anchor="middle" font-family="monospace" font-size="8" fill="#64748b">International</text>

  <text x="275" y="189" text-anchor="middle" font-size="14" fill="#8b5cf6" opacity="0.5">→</text>

  <!-- Node 3: Powerweave -->
  <circle cx="340" cy="185" r="22" fill="#020817" stroke="#06b6d4" stroke-width="2" filter="url(#ng)">
    <animate attributeName="r" values="22;25;22" dur="4s" begin="1s" repeatCount="indefinite"/>
  </circle>
  <text x="340" y="191" text-anchor="middle" font-size="16">🛠️</text>
  <text x="340" y="222" text-anchor="middle" font-family="monospace" font-size="8" fill="#94a3b8" letter-spacing="1">2020–21</text>
  <text x="340" y="236" text-anchor="middle" font-family="monospace" font-size="10" font-weight="bold" fill="#e2e8f0">Tech</text>
  <text x="340" y="249" text-anchor="middle" font-family="monospace" font-size="10" fill="#e2e8f0">Support</text>
  <text x="340" y="152" text-anchor="middle" font-family="monospace" font-size="8" fill="#64748b">Powerweave</text>
  <text x="340" y="140" text-anchor="middle" font-family="monospace" font-size="8" fill="#64748b">Software</text>

  <text x="400" y="189" text-anchor="middle" font-size="14" fill="#06b6d4" opacity="0.5">→</text>

  <!-- Node 4: Ziplyne -->
  <circle cx="460" cy="185" r="22" fill="#020817" stroke="#8b5cf6" stroke-width="2" filter="url(#ng)">
    <animate attributeName="r" values="22;25;22" dur="4s" begin="1.5s" repeatCount="indefinite"/>
  </circle>
  <text x="460" y="191" text-anchor="middle" font-size="16">📣</text>
  <text x="460" y="222" text-anchor="middle" font-family="monospace" font-size="8" fill="#94a3b8" letter-spacing="1">2021–24</text>
  <text x="460" y="236" text-anchor="middle" font-family="monospace" font-size="10" font-weight="bold" fill="#e2e8f0">GTM</text>
  <text x="460" y="249" text-anchor="middle" font-family="monospace" font-size="10" fill="#e2e8f0">Lead</text>
  <text x="460" y="152" text-anchor="middle" font-family="monospace" font-size="8" fill="#64748b">Ziplyne</text>
  <text x="460" y="140" text-anchor="middle" font-family="monospace" font-size="8" fill="#64748b">Inc.</text>

  <text x="520" y="189" text-anchor="middle" font-size="14" fill="#8b5cf6" opacity="0.5">→</text>

  <!-- Node 5: Botmartz -->
  <circle cx="580" cy="185" r="22" fill="#020817" stroke="#06b6d4" stroke-width="2" filter="url(#ng)">
    <animate attributeName="r" values="22;25;22" dur="4s" begin="2s" repeatCount="indefinite"/>
  </circle>
  <text x="580" y="191" text-anchor="middle" font-size="16">🤖</text>
  <text x="580" y="222" text-anchor="middle" font-family="monospace" font-size="8" fill="#94a3b8" letter-spacing="1">2024–Now</text>
  <text x="580" y="236" text-anchor="middle" font-family="monospace" font-size="10" font-weight="bold" fill="#e2e8f0">GenAI</text>
  <text x="580" y="249" text-anchor="middle" font-family="monospace" font-size="10" fill="#e2e8f0">Trainer</text>
  <text x="580" y="152" text-anchor="middle" font-family="monospace" font-size="8" fill="#64748b">Botmartz</text>
  <text x="580" y="140" text-anchor="middle" font-family="monospace" font-size="8" fill="#64748b">IT Solutions</text>

  <text x="642" y="189" text-anchor="middle" font-size="14" fill="#06b6d4" opacity="0.5">→</text>

  <!-- Node 6: CURRENT — IntelliPaaS (golden, bigger, pulsing) -->
  <circle cx="710" cy="185" r="30" fill="#020817" stroke="#fbbf24" stroke-width="2.5" filter="url(#ng)">
    <animate attributeName="r" values="30;34;30" dur="2.5s" repeatCount="indefinite"/>
    <animate attributeName="stroke-opacity" values="1;0.5;1" dur="2.5s" repeatCount="indefinite"/>
  </circle>
  <text x="710" y="192" text-anchor="middle" font-size="20">🏗️</text>
  <text x="710" y="228" text-anchor="middle" font-family="monospace" font-size="8" fill="#fbbf24" letter-spacing="1">AUG 2025</text>
  <text x="710" y="242" text-anchor="middle" font-family="monospace" font-size="11" font-weight="bold" fill="#fbbf24">AI Architect</text>
  <text x="710" y="256" text-anchor="middle" font-family="monospace" font-size="10" fill="#fbbf24">& AI PM</text>
  <text x="710" y="149" text-anchor="middle" font-family="monospace" font-size="9" font-weight="bold" fill="#fbbf24">IntelliPaaS</text>
  <text x="710" y="137" text-anchor="middle" font-family="monospace" font-size="8" fill="#fbbf24">Inc.</text>

  <!-- Future node -->
  <text x="778" y="189" text-anchor="middle" font-size="14" fill="#fbbf24" opacity="0.7">→</text>
  <circle cx="820" cy="185" r="18" fill="#020817" stroke="#fbbf24" stroke-width="1.5" stroke-dasharray="5 3" opacity="0.5">
    <animate attributeName="opacity" values="0.4;0.9;0.4" dur="2.5s" repeatCount="indefinite"/>
  </circle>
  <text x="820" y="191" text-anchor="middle" font-size="14">🚀</text>
  <text x="820" y="218" text-anchor="middle" font-family="monospace" font-size="8" fill="#475569">NEXT</text>

  <!-- Bottom captions -->
  <text x="440" y="310" text-anchor="middle" font-family="monospace" font-size="12" fill="#475569" letter-spacing="2">From Aircraft Maintenance → GenAI Architecture</text>
  <text x="440" y="338" text-anchor="middle" font-family="monospace" font-size="11" fill="#06b6d4" letter-spacing="1">The rarest kind of engineer: one who flies AND thinks at altitude ✈️🧠</text>
</svg>

</div>

---

## `> impact --metrics`

<div align="center">

<!-- ===== IMPACT METRICS BAR ===== -->
<svg width="880" height="160" viewBox="0 0 880 160" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="mbg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#020817"/>
      <stop offset="100%" style="stop-color:#0a1628"/>
    </linearGradient>
  </defs>
  <rect width="880" height="160" fill="url(#mbg)" rx="16"/>

  <!-- Card 1 -->
  <rect x="12" y="12" width="160" height="136" rx="12" fill="#06b6d406" stroke="#06b6d4" stroke-width="0.8">
    <animate attributeName="stroke-opacity" values="0.6;1;0.6" dur="3s" repeatCount="indefinite"/>
  </rect>
  <text x="92" y="56" text-anchor="middle" font-family="monospace" font-size="36" font-weight="900" fill="#06b6d4">20+</text>
  <text x="92" y="78" text-anchor="middle" font-family="monospace" font-size="9" fill="#94a3b8" letter-spacing="1.5">CORPORATE</text>
  <text x="92" y="92" text-anchor="middle" font-family="monospace" font-size="9" fill="#94a3b8" letter-spacing="1.5">CLIENTS</text>
  <text x="92" y="126" text-anchor="middle" font-size="22">🏢</text>

  <!-- Card 2 -->
  <rect x="184" y="12" width="160" height="136" rx="12" fill="#8b5cf606" stroke="#8b5cf6" stroke-width="0.8">
    <animate attributeName="stroke-opacity" values="0.6;1;0.6" dur="3s" begin="0.5s" repeatCount="indefinite"/>
  </rect>
  <text x="264" y="56" text-anchor="middle" font-family="monospace" font-size="36" font-weight="900" fill="#a78bfa">15+</text>
  <text x="264" y="78" text-anchor="middle" font-family="monospace" font-size="9" fill="#94a3b8" letter-spacing="1.5">ACADEMIC</text>
  <text x="264" y="92" text-anchor="middle" font-family="monospace" font-size="9" fill="#94a3b8" letter-spacing="1.5">INSTITUTIONS</text>
  <text x="264" y="126" text-anchor="middle" font-size="22">🎓</text>

  <!-- Card 3 -->
  <rect x="356" y="12" width="160" height="136" rx="12" fill="#10b98106" stroke="#10b981" stroke-width="0.8">
    <animate attributeName="stroke-opacity" values="0.6;1;0.6" dur="3s" begin="1s" repeatCount="indefinite"/>
  </rect>
  <text x="436" y="56" text-anchor="middle" font-family="monospace" font-size="36" font-weight="900" fill="#34d399">95%</text>
  <text x="436" y="78" text-anchor="middle" font-family="monospace" font-size="9" fill="#94a3b8" letter-spacing="1.5">SATISFACTION</text>
  <text x="436" y="92" text-anchor="middle" font-family="monospace" font-size="9" fill="#94a3b8" letter-spacing="1.5">RATE</text>
  <text x="436" y="126" text-anchor="middle" font-size="22">⭐</text>

  <!-- Card 4 -->
  <rect x="528" y="12" width="160" height="136" rx="12" fill="#f59e0b06" stroke="#f59e0b" stroke-width="0.8">
    <animate attributeName="stroke-opacity" values="0.6;1;0.6" dur="3s" begin="1.5s" repeatCount="indefinite"/>
  </rect>
  <text x="608" y="56" text-anchor="middle" font-family="monospace" font-size="36" font-weight="900" fill="#fbbf24">10K+</text>
  <text x="608" y="78" text-anchor="middle" font-family="monospace" font-size="9" fill="#94a3b8" letter-spacing="1.5">MONTHLY</text>
  <text x="608" y="92" text-anchor="middle" font-family="monospace" font-size="9" fill="#94a3b8" letter-spacing="1.5">READERS</text>
  <text x="608" y="126" text-anchor="middle" font-size="22">📖</text>

  <!-- Card 5 -->
  <rect x="700" y="12" width="166" height="136" rx="12" fill="#ec489906" stroke="#ec4899" stroke-width="0.8">
    <animate attributeName="stroke-opacity" values="0.6;1;0.6" dur="3s" begin="2s" repeatCount="indefinite"/>
  </rect>
  <text x="783" y="56" text-anchor="middle" font-family="monospace" font-size="36" font-weight="900" fill="#f472b6">11+</text>
  <text x="783" y="78" text-anchor="middle" font-family="monospace" font-size="9" fill="#94a3b8" letter-spacing="1.5">YEARS</text>
  <text x="783" y="92" text-anchor="middle" font-family="monospace" font-size="9" fill="#94a3b8" letter-spacing="1.5">EXPERIENCE</text>
  <text x="783" y="126" text-anchor="middle" font-size="22">🔥</text>
</svg>

</div>

---

## `> status --now`

```bash
$ soham --current-mission

🏗️  BUILDING    →  Production-grade GenAI SaaS @ IntelliPaaS Inc.
🎓  TEACHING    →  AI/ML Corporate Training for MNCs (India & US)
📚  MASTERING   →  Multi-Agent Systems · LLM Fine-Tuning · AI Safety
✍️  WRITING     →  Technical blogs on Prompt Engineering, AI Agents & LLMs
🤝  OPEN FOR    →  AI Consulting · GenAI Architecture · Collaboration

$ uptime
11 years, still running... no signs of stopping 🚀
```

---

## `> connect --handshake`

<div align="center">

<!-- ===== CONNECT / QUOTE BANNER ===== -->
<svg width="880" height="120" viewBox="0 0 880 120" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="cbg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#020817"/>
      <stop offset="100%" style="stop-color:#0a1628"/>
    </linearGradient>
    <linearGradient id="qGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#67e8f9"/>
      <stop offset="45%" style="stop-color:#ffffff"/>
      <stop offset="100%" style="stop-color:#a78bfa"/>
    </linearGradient>
    <filter id="tg2">
      <feGaussianBlur stdDeviation="2" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>
  <rect width="880" height="120" fill="url(#cbg)" rx="16"/>
  <rect x="2" y="2" width="876" height="116" rx="15" fill="none" stroke="url(#qGrad)" stroke-width="1" opacity="0.4">
    <animate attributeName="opacity" values="0.3;0.7;0.3" dur="4s" repeatCount="indefinite"/>
  </rect>
  <text x="440" y="44" text-anchor="middle" font-family="'Courier New',monospace" font-size="18" font-weight="bold" fill="url(#qGrad)" filter="url(#tg2)" letter-spacing="1.5">"Don't just use AI. Architect it. Ship it. Scale it."</text>
  <text x="440" y="70" text-anchor="middle" font-family="monospace" font-size="12" fill="#475569">— Soham Sharma · GenAI Architect · IntelliPaaS Inc.</text>
  <text x="440" y="100" text-anchor="middle" font-family="monospace" font-size="10" fill="#334155" letter-spacing="1.5">📧 sohamnsharma@gmail.com  ·  📍 Indore, India  ·  🐙 soham2710</text>
</svg>

<br/>

[![LinkedIn](https://img.shields.io/badge/Let's_Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/soham-sharma/)
[![Email](https://img.shields.io/badge/Email_Me-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sohamnsharma@gmail.com)
[![Medium](https://img.shields.io/badge/Read_My_Blog-12100E?style=for-the-badge&logo=medium&logoColor=white)](http://www.medium.com/@sohamnsharma)
[![BuyMeACoffee](https://img.shields.io/badge/Support_My_Work-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/sohamnsharma)

<br/>

<!-- ===== ANIMATED WAVE FOOTER ===== -->
<svg width="880" height="60" viewBox="0 0 880 60" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="wg" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#06b6d4;stop-opacity:0.9"/>
      <stop offset="50%" style="stop-color:#8b5cf6;stop-opacity:0.9"/>
      <stop offset="100%" style="stop-color:#06b6d4;stop-opacity:0.9"/>
    </linearGradient>
  </defs>
  <path d="M0,30 C146,60 293,0 440,30 C587,60 734,0 880,30 L880,60 L0,60 Z" fill="url(#wg)" opacity="0.7">
    <animate attributeName="d" values="M0,30 C146,60 293,0 440,30 C587,60 734,0 880,30 L880,60 L0,60 Z;M0,40 C146,10 293,50 440,20 C587,0 734,50 880,30 L880,60 L0,60 Z;M0,30 C146,60 293,0 440,30 C587,60 734,0 880,30 L880,60 L0,60 Z" dur="6s" repeatCount="indefinite"/>
  </path>
  <text x="440" y="48" text-anchor="middle" font-family="monospace" font-size="11" fill="white" letter-spacing="3">✨ Building tomorrow's AI infrastructure, today ✨</text>
</svg>

</div>
