---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am an **AI Engineer / Data Scientist** with 3+ years building production ML systems. My expertise spans **Credit Scoring, LLMs, Generative AI (Diffusion Models), 3D Deep Learning, and Multi-Agent Systems**. Currently pursuing an **M.Sc. in Artificial Intelligence** at **Nanyang Technological University (NTU), Singapore**. Experienced in end-to-end model deployment on GCP/AWS, MLOps, and real-time inference at scale.

---

Education
======

**M.Sc. in Artificial Intelligence** — Nanyang Technological University, Singapore *(Aug 2025 – Jun 2026)*  
GPA: 4.30/5.00 · Expected Graduation: Jun 2026  
Relevant Courses: Generative AI for Visual Synthesis, Large Language Models, 3D Deep Learning, Multi-Agent Systems, Advanced Computer Vision

**B.Sc. in Computer Science** — Universitas Gadjah Mada, Indonesia *(Aug 2018 – Feb 2022)*  
GPA: 3.91/4.00 · Graduated Cum Laude

---

Technical Skills
======

* **Programming Languages:** Python, Java, SQL
* **LLM & GenAI:** LangChain, LlamaIndex, OpenAI API, Anthropic API, Hugging Face, PEFT/LoRA, Ollama, vLLM, Prompt Engineering
* **ML & Frameworks:** PyTorch, TensorFlow, Scikit-Learn, XGBoost, LightGBM, OpenCV, Librosa, DDPM/Diffusion Models
* **MLOps & Infra:** GCP (BigQuery, Vertex AI, Compute Engine), AWS (EC2, Redshift), Docker, FastAPI, CI/CD, Git/GitHub, Cloud Migration
* **Data & Databases:** PostgreSQL, BigQuery, Apache Airflow, Metabase, Tableau, A/B Testing, Feature Engineering
* **Domains:** Generative AI, RAG Pipelines, Computer Vision, Audio Signal Processing, NLP/Text Mining, Real-Time Inference, Smartwatch/Wearable Development
* **Other:** HarmonyOS, ArkTS (TypeScript for HarmonyOS)

---

Work Experience
======

**Data Scientist \| JULO (Fintech Lending), Jakarta, Indonesia** *(May 2022 – Jul 2025)*

* **Credit Scoring Engine:** Architected and deployed a full suite of credit models — Income Prediction, Application Score (B-Score), and Collection Prioritisation — on GCP using XGBoost and LightGBM. Models directly determined credit limits and recovery strategies across the user base.
* **Real-Time Risk System:** Engineered a low-latency, transaction-level risk scoring model achieving sub-second response times while increasing Risk-Adjusted Returns (RAR) by 30%.
* **Advanced Feature Engineering:** Designed complex feature logic in Python and SQL integrating internal behavioural data with external sources, improving model AUC by 10–20% across the credit model suite.
* **ML Infrastructure & MLOps:** Led migration of all ML workflows from AWS to GCP, reducing model retraining cycles from 3–5 days to 1 day.
* **Model Observability & Monitoring:** Built comprehensive dashboards in Metabase and BigQuery tracking concept drift (PSI), prediction score distributions, and business KPIs (ROI, CLV).
* **Technical Mentorship:** Mentored 2 Junior Data Scientists with weekly knowledge-sharing sessions on ML best practices and credit risk domain knowledge.

**AI Research Assistant \| Universitas Gadjah Mada, Yogyakarta, Indonesia** *(Oct 2020 – Mar 2021)*

* **Computer Vision:** Built a CCTV face-tracking pipeline with RetinaFace + detection-based tracking; improved recall by 4.47% in low-illumination conditions via a custom post-processing algorithm.
* **NLP:** Applied Latent Dirichlet Allocation (LDA) for automated MeSH biomedical indexing, achieving 74% topic similarity vs. human-expert labels.

**Data Science Intern \| Bukit Vista, Yogyakarta, Indonesia** *(Sep – Nov 2021)*

* Designed dynamic pricing strategies from historical booking data, adopted by the Business Intelligence unit to optimise occupancy revenue.
* Executed ETL and data validation workflows to ensure high-integrity datasets for downstream reporting.

---

Projects
======

### Deepfake Audio Detection — Runner-up, DeepDetect Hackathon 2025

[GitHub](https://github.com/Ardacandra/deepdetect_audio_deepfake_detection_challenge)

Developed a **Transformer-based classifier** for AI-synthesised speech (TTS & voice conversion) achieving **99.98% test accuracy** (Rank 2 on the public leaderboard). The pipeline progresses from classical ML baselines (CatBoost: 0.989) to wav2vec2 feed-forward networks (0.996) to a CNN + Transformer hybrid with Mixup augmentation (0.999), with an ML-committee post-hoc correction stage for uncertain samples.

![Leaderboard](/images/porto__deepfake__leaderboard.png)

**Audio Signal Analysis — Real vs. Fake:**

| | Real | Fake |
|---|---|---|
| Waveform | ![Real waveform](/images/porto__deepfake__waveform_real.png) | ![Fake waveform](/images/porto__deepfake__waveform_fake.png) |
| Spectrogram | ![Real spectrogram](/images/porto__deepfake__spectrogram_real.png) | ![Fake spectrogram](/images/porto__deepfake__spectrogram_fake.png) |

**HybridAudioClassifier Training (CNN + Transformer + Mixup):**

| Loss | F1-Score |
|---|---|
| ![Training Loss](/images/porto__deepfake__dl_hybrid_loss.png) | ![F1-Score](/images/porto__deepfake__dl_hybrid_f1.png) |

**Final Model Evaluation:**

| Confusion Matrix | ROC Curve |
|---|---|
| ![Confusion Matrix](/images/porto__deepfake__confusion_matrix.png) | ![ROC Curve](/images/porto__deepfake__roc_curve.png) |

| Stage | Leaderboard Score |
|---|---|
| HybridAudioClassifier + Mixup | 0.99939 |
| + ML committee blending | 0.99962 |
| **+ Qualitative corrections (final)** | **0.99984** |

*Stack: Python, PyTorch, Librosa*

---

### CelebAMask Face Parsing — Advanced Computer Vision (NTU AI6126)

[GitHub](https://github.com/Ardacandra/ai6126_CelebAMask_face_parsing)

Designed and trained a **Lite-Face Parser (LFP)** for semantic face segmentation on CelebAMask-HQ (1,000 training pairs at 512×512), achieving an **F1-score of 0.83**. The LFP architecture uses three parallel paths (Context, Detail, Texture) integrated via a Weighted Bi-Fusion Decoder with Prototype Refinement and Edge-Guided Fusion, with a combined CE + Dice + Boundary loss and post-processing (small component removal + majority filter).

**Architecture:**

![Lite-Face Parser Architecture](/images/porto__celebamask__architecture.png)

**Qualitative Results — Input vs. SRResNet Baseline vs. Lite-Face Parser:**

| Input Image | SRResNet Baseline | Lite-Face Parser |
|:---:|:---:|:---:|
| ![Input](/images/porto__celebamask__original.jpg) | ![SRResNet](/images/porto__celebamask__mask_srr.png) | ![LFP](/images/porto__celebamask__mask_lfp.png) |

| Model | Parameters | F-score |
|---|---|---|
| SRResNet | 1,428,762 | 0.6357 |
| **Lite-Face Parser** | **1,820,207** | **0.7429** |

*Stack: Python, PyTorch*

---

### 3D Shape Reconstruction & Generation — VQ-DeepSDF with AR Transformer Prior (NTU AI6131)

[GitHub](https://github.com/Ardacandra/ai6131_3d_deep_learning_final_project)

Implemented **Generative DeepSDF**: a Vector-Quantised (VQ) bottleneck over the DeepSDF autodecoder discretises the latent manifold into a learned codebook, then a **causal AR Transformer** models the distribution of discrete shape sequences for novel 3D synthesis. Evaluated on ShapeNet (Chair, Table, Airplane — 50 objects each).

**Reconstruction Fidelity:**

| Ground Truth | Baseline DeepSDF | Generative DeepSDF |
|:---:|:---:|:---:|
| ![Ground Truth](/images/porto__3d__gt.png) | ![Baseline Reconstruction](/images/porto__3d__baseline_recon.png) | ![Generative Reconstruction](/images/porto__3d__generative_recon.png) |

**Latent Space — Discrete Code Heatmap:**

![Latent Codes](/images/porto__3d__latent_codes.png)

**Novel Shape Generation (AR Prior vs. Gaussian Baseline):**

| AR Prior Gen 1 | AR Prior Gen 2 | AR Prior Gen 3 |
|:---:|:---:|:---:|
| ![AR Gen 1](/images/porto__3d__ar_gen_1.png) | ![AR Gen 2](/images/porto__3d__ar_gen_2.png) | ![AR Gen 3](/images/porto__3d__ar_gen_3.png) |

| Method | Chamfer Distance ↓ | Silhouette ↑ | MMD ↓ |
|---|---|---|---|
| Baseline DeepSDF | 0.1288 | 0.0522 | 0.3282 |
| **Generative DeepSDF** | 0.1396 | **0.1298** | **0.1046** |

*Stack: Python, PyTorch, HuggingFace*

---

### Local RAG Document Q&A

[GitHub](https://github.com/Ardacandra/rag_document_qna)

Built a **privacy-first Retrieval-Augmented Generation** pipeline for unstructured PDFs using LlamaIndex and local LLMs via Ollama — no external API calls. Implements two-stage retrieval (High-K + reranking) to maximise context precision.

![RAG Sample Output](/images/porto__rag__sample_output.png)

*Stack: Python, LlamaIndex, Ollama*

---

### Tileworld Multi-Agent System (NTU AI6125)

[GitHub](https://github.com/ntu-ai6125-2026-group-2/ai6125_tileworld_agent)

Designed and implemented intelligent **Java agents** for the Tileworld simulation environment, incorporating planning, working memory, and inter-agent communication modules. Agents evaluated across multiple environment configurations (50×50 and 80×80 grids, varying object creation rates and lifetimes) over 10-run statistical benchmarks maximising cumulative reward.

Key design:
* **Planning module** — reacts to sensed environment and updates memory for next-action planning
* **Memory module** — `TWAgentWorkingMemory` stores environmental state across steps
* **Communication module** — per-step broadcast messaging between agents

*Stack: Java*

---

### Anchor — Wearable Safety Companion for Seniors (Hackathon)

[GitHub](https://github.com/Runtime-Terrors-v2/Anchor)

**ANCHOR** is a HarmonyOS smartwatch app for senior safety combining **dual-signal geofencing** (accelerometer + GPS) and a **logistic regression fall detector** trained on the SisFall dataset. A full-stack wearable system with watch-to-phone P2P messaging, push notifications, and caregiver alert pipeline.

**Key features:**
* Geofencing with three drift states: `SAFE` → `DRIFTING` (30–50m) → `ALERT` (>50m), requiring both walking and GPS signals to minimise false alarms
* Two parallel fall detectors: threshold-based (>25 m/s² impact) and ML classifier
* Caregiver phone app with alert history, emergency contacts, and watch disconnect notifications
* Community card for first-responders stored on the watch

**Watch App:**

![Watch UI](/images/porto__anchor__watch_ui.png)

**Caregiver Phone App:**

![Phone UI](/images/porto__anchor__phone_ui.png)

**Watch App Demo:**

![Watch App Demo](/images/porto__anchor__demo_watch.gif)

**Phone App Demo:**

![Phone App Demo](/images/porto__anchor__demo_mobile.gif)

*Stack: ArkTS, HarmonyOS, TypeScript*

---

Publications
======

* **Human Face Detection and Tracking Using RetinaFace Network**  
  *47th Annual Conference of the IEEE Industrial Electronics Society (IECON 2021)*  
  Engineered a CCTV face tracking pipeline using RetinaFace and detection-based tracking, improving face detection recall by 4.47% in low-illumination environments.  
  [Paper Link](https://ieeexplore.ieee.org/document/9589577)

* **Medical Subject Headings (MeSH) Indexing Using Unsupervised Learning**  
  *2021 International Conference on Computer, Control, Informatics and Its Applications (ICCCIA 2021)*  
  Applied Latent Dirichlet Allocation (LDA) for automated MeSH biomedical indexing, achieving 74% topic similarity vs. human-expert labels.  
  [Paper Link](https://dl.acm.org/doi/10.1145/3489088.3489096)

---

Languages
======

English (Full Professional) · Bahasa Indonesia (Native)

---

Let's Connect
======

Based in **Singapore**. Open to collaborations in AI research and engineering.

* **Email:** [ardacandrasubiantoro@gmail.com](mailto:ardacandrasubiantoro@gmail.com)
* **LinkedIn:** [linkedin.com/in/ardacandra-subiantoro](https://linkedin.com/in/ardacandra-subiantoro)
* **GitHub:** [github.com/Ardacandra](https://github.com/Ardacandra)
