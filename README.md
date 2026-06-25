# Bias Autopsy

A surgical bias detection tool for datasets — powered by Groq + LLaMA.**

Upload any structured dataset and get a plain-English autopsy of every bias lurking inside: gender gaps, racial skews, temporal drift, class imbalance — with actionable fixes for each.

🔗 **Live Demo:** [bias-autopsy.vercel.app](https://bias-autopsy-git-main-seetharam2000s-projects.vercel.app/)

---

What It Does

Bias Autopsy walks your dataset through four pipeline stages:

| Stage | What happens |
|---|---|
| **01 · Ingest** | Upload CSV, XLSX, JSON, Parquet, or TSV — or paste raw CSV / provide a URL |
| **02 · Profiling** | Automated column-level statistics, null rates, cardinality, and distribution summaries |
| **03 · Dissection** | LLaMA (via Groq) detects bias patterns: representation gaps, skewed distributions, temporal drift, label imbalance |
| **04 · Report** | Plain-English findings with severity ratings and concrete mitigation strategies |

---

Tech Stack

- **Frontend:** Vanilla HTML/CSS/JS — zero frameworks, zero dependencies
- **AI:** LLaMA 3 via [Groq API](https://console.groq.com) (ultra-low latency inference)
- **Deployment:** Vercel (static hosting)
- **Supported Formats:** CSV · XLSX · JSON · Parquet · TSV

---

Getting Started

1. Clone the repo

```bash
git clone https://github.com/Seetharam2000/Bias-Autopsy.git
cd Bias-Autopsy
```

 2. Get a Groq API key

Sign up at [console.groq.com](https://console.groq.com) → API Keys → Create key.

Enter the key when prompted in the app. It stays in memory only — never stored or sent anywhere except Groq's API.

3. Run locally

Static site — just open `index.html` or serve it:

```bash
npx serve .
```

 4. Deploy to Vercel

```bash
vercel --prod
```

---

Project Structure

```
Bias-Autopsy/
├── index.html        # Entry point
└── src/
    └── ...           # App source
```

---

Use Cases

- **ML Engineers** — audit training data before model training
- **Data Analysts** — surface hidden skews in reporting datasets
- **Researchers** — validate dataset fairness for academic work
- **Hiring / HR Teams** — detect demographic imbalances in candidate pipelines

---

 Roadmap

- [ ] Export bias report as PDF
- [ ] Column-level bias heatmap visualization
- [ ] Support for multi-file comparison
- [ ] Integration with Hugging Face datasets

---

Author

Seetharam — B.Tech CSE (Big Data Analytics), SRM Institute of Science and Technology  
GitHub: [@Seetharam2000](https://github.com/Seetharam2000)

---

License

MIT
