<!-- Design follows my portfolio: beige canvas, black ink, one yellow accent, Schibsted Grotesk + Hanken Grotesk. -->

<img src="assets/header.svg" width="100%" alt="Muhammad Hamza: AI Researcher & Engineer. Researching Intelligent Systems. 1 publication (IBCAST 2026, accepted), 3 projects. B.S. Artificial Intelligence, FAST-NUCES Islamabad, expected May 2027.">

<p>
  <a href="mailto:hamza35502@gmail.com"><img src="https://img.shields.io/badge/Email-FFFF23?style=for-the-badge&logo=gmail&logoColor=000000" alt="Email"></a>
  <a href="https://linkedin.com/in/hamza35502"><img src="https://img.shields.io/badge/LinkedIn-222222?style=for-the-badge" alt="LinkedIn"></a>
</p>

Undergraduate AI researcher at FAST-NUCES Islamabad working across **computer vision**, **NLP** and **agentic systems**, with an accepted IBCAST 2026 paper.

It started with machines that could hold a conversation with people. I wanted to know how they worked, and the work below is where that question took me.

| **Agentic AI** | **Computer Vision** | **NLP** |
|---|---|---|
| Tool-using LLM agents with structured retrieval and long-horizon reasoning. | Foundation models like SAM, segmentation and medical imaging. | Retrieval-augmented generation over long, structured documents, and assistants that answer in English and Urdu. |

<br>

<img src="assets/01-research.svg" width="100%" alt="01 · Research & Publications">

Papers and ongoing research in computer vision, medical imaging and machine learning.

### Feature-Level Fusion of Complementary Vision Transformers for Generalizable Medical Image Classification

Hassan Abdullah, **Muhammad Hamza**, Muhammad Ibrahim, Dr. Qurat Ul Ain · *IBCAST 2026* · **Accepted**

<img src="assets/research-vit-fusion.png" width="100%" alt="Fusion architecture: an input image goes through three frozen backbones (MedViT2, MedFormer and DeiT); each feature vector passes through its own linear projection layer, the projected vectors are concatenated into one 768-dimensional vector, and a shared classifier makes the prediction.">

Fuses three frozen Vision Transformer backbones and trains only **0.75%** of the parameters, reaching **95.73%** on chest X-ray pneumonia, **93.17%** on brain MRI and **78.58%** on ISIC 2018 skin lesions across seven medical imaging datasets.

**My part:** led the ablation study across 7 backbone configurations and the cross-domain evaluation on 4 MedMNIST benchmarks.

[Code →](https://github.com/Hamza0590/Feature_Level_Fusion_of_Vision_Transformers)

### Resource- and Contention-Aware Edge Triage for Astronomical Transients · *ongoing*

<img src="assets/work-edge-astronomical-triage.png" width="100%" alt="Diagram: a stream of candidates enters a model tier (Tiny, Medium, Large); each candidate is then discarded, compressed or transmitted.">

An edge system that decides, under limited compute, which model tier screens each astronomical transient candidate, how many inferences run at once, and whether the data is discarded, compressed or transmitted. A Tiny/Medium/Large CNN family classifies real versus bogus candidates from MeerCRAB/MeerLICHT cutouts; a resource-aware scheduler picks the tier and concurrency, and MC-dropout uncertainty escalates ambiguous candidates.

**Status:** in implementation. Results will be added once the experiments are complete.
**My part:** literature review, code and system review.

`Python` `PyTorch` `NumPy` `pandas` `scikit-learn` · [Code →](https://github.com/Hamza0590/Edge_Triage_System)

<br>

<img src="assets/02-work.svg" width="100%" alt="02 · Selected Work: Systems I've Built">

AI systems and research projects, from agentic retrieval to remote-sensing segmentation and edge AI.

### Tax Sathi — Agentic Tax Assistant for Pakistan

<img src="assets/work-fbr-taxation-agentic-system.png" width="100%" alt="Diagram: a chat message flows through four stages (extract, retrieve, interpret, calculate) into a result citing law sections.">

Turns a plain-English or Urdu description of income into a full Pakistani income-tax calculation, with FBR section citations and an auditable reasoning trace.

- **4-stage LangGraph pipeline:** extraction → retrieval → interpretation → calculation.
- **80+ ordinance sections** in a tree index over the Income Tax Ordinance 2001, searched in two passes that follow cross-references.
- **The LLM classifies, Python calculates:** the model only makes legal classification decisions; tax is computed deterministically from the FY 2025-26 rate tables, so every number is reproducible.
- Reads salary slips, withholding certificates and challans through a vision model, and shows the full reasoning trace in a live panel.

`LangGraph` `LiteLLM` `Groq LLaMA 3.3 70B` `FastAPI` `Pydantic` `Supabase` `React` · Solo · [Code →](https://github.com/Hamza0590/fbr-taxation-agent)

### Glacial Lake Semantic Segmentation — Reproduction Study

<img src="assets/work-glacial-lake-segmentation.png" width="100%" alt="Two predicted glacial lake masks in yellow on a dark background.">

Reproduced the IEEE JSTARS 2025 study by Xue et al. in PyTorch: U-Net, Simple CNN and ASPP-SegNet trained on 410 Sentinel-2 tiles of the Himalayas, with a FastAPI + React app to compare their masks.

| Model | Val IoU | Val F1 |
|---|---|---|
| **ASPP-SegNet** | **0.9010** | **0.9479** |
| U-Net | 0.8693 | 0.9301 |
| Simple CNN | 0.8410 | 0.9136 |

Every deviation from the paper is documented with its reason. Lead developer in a two-person project.

`PyTorch` `Albumentations` `OpenCV` `FastAPI` `React` · [Code →](https://github.com/Hamza0590/glacial-lake-semantic-segmentation)

<br>

<img src="assets/03-experience.svg" width="100%" alt="03 · Experience: Where I've Worked">

Internships across computer vision research and applied AI engineering.

**Computer Vision Research Intern** · SYSTEMS · Islamabad · *Jul – Aug 2026*
- Reproduced a supervisor-authored paper's architecture in PyTorch and fine-tuned SAM's mask decoder on the Massachusetts Buildings Dataset, raising mean IoU from **0.169 to 0.679** (4.02×) over zero-shot.
- Benchmarked fine-tuned SAM against RemoteSAM and vanilla zero-shot SAM on held-out aerial tiles, cutting segmentation errors by **2.59×** (F1 0.240 → 0.802).

**AI Intern** · Software Productivity Strategists · Islamabad · *Jul – Sep 2025*
- Designed an AI chatbot with IBM Watson Assistant, integrating NLP flows to automate client support and cutting manual response time by about **40%**.
- Provisioned 3 Azure VMs with site-to-site VPN and automated daily backups, reducing the data-loss window from **72h to under 24h**.
- Automated CI/CD with GitHub Actions and Azure DevOps (environment-gated approvals, automatic rollback), reducing manual deployment effort by about **60%**.

<br>

<img src="assets/04-stack.svg" width="100%" alt="04 · Tech Stack: Tools I Build With">

**Languages**
<img src="https://img.shields.io/badge/Python-EBEADA?style=flat-square&logo=python&logoColor=000000" alt="Python">
<img src="https://img.shields.io/badge/C%2B%2B-EBEADA?style=flat-square&logo=cplusplus&logoColor=000000" alt="C++">
<img src="https://img.shields.io/badge/JavaScript-EBEADA?style=flat-square&logo=javascript&logoColor=000000" alt="JavaScript">

**ML & Deep Learning**
<img src="https://img.shields.io/badge/PyTorch-EBEADA?style=flat-square&logo=pytorch&logoColor=000000" alt="PyTorch">
<img src="https://img.shields.io/badge/TensorFlow-EBEADA?style=flat-square&logo=tensorflow&logoColor=000000" alt="TensorFlow">
<img src="https://img.shields.io/badge/Hugging%20Face-EBEADA?style=flat-square&logo=huggingface&logoColor=000000" alt="Hugging Face">
<img src="https://img.shields.io/badge/scikit--learn-EBEADA?style=flat-square&logo=scikitlearn&logoColor=000000" alt="scikit-learn">
<img src="https://img.shields.io/badge/NumPy-EBEADA?style=flat-square&logo=numpy&logoColor=000000" alt="NumPy">
<img src="https://img.shields.io/badge/pandas-EBEADA?style=flat-square&logo=pandas&logoColor=000000" alt="pandas">

**LLMs & Agents**
<img src="https://img.shields.io/badge/LangGraph-EBEADA?style=flat-square" alt="LangGraph">
<img src="https://img.shields.io/badge/LangChain-EBEADA?style=flat-square&logo=langchain&logoColor=000000" alt="LangChain">
<img src="https://img.shields.io/badge/LiteLLM-EBEADA?style=flat-square" alt="LiteLLM">
<img src="https://img.shields.io/badge/Groq-EBEADA?style=flat-square" alt="Groq">
<img src="https://img.shields.io/badge/FAISS-EBEADA?style=flat-square" alt="FAISS">
<img src="https://img.shields.io/badge/IBM%20Watson%20Assistant-EBEADA?style=flat-square" alt="IBM Watson Assistant">

**Computer Vision**
<img src="https://img.shields.io/badge/OpenCV-EBEADA?style=flat-square&logo=opencv&logoColor=000000" alt="OpenCV">
<img src="https://img.shields.io/badge/YOLOv8-EBEADA?style=flat-square" alt="YOLOv8">
<img src="https://img.shields.io/badge/SAM-EBEADA?style=flat-square" alt="SAM">
<img src="https://img.shields.io/badge/Albumentations-EBEADA?style=flat-square" alt="Albumentations">

**Backend & Deployment**
<img src="https://img.shields.io/badge/FastAPI-EBEADA?style=flat-square&logo=fastapi&logoColor=000000" alt="FastAPI">
<img src="https://img.shields.io/badge/Pydantic-EBEADA?style=flat-square&logo=pydantic&logoColor=000000" alt="Pydantic">
<img src="https://img.shields.io/badge/React-EBEADA?style=flat-square&logo=react&logoColor=000000" alt="React">
<img src="https://img.shields.io/badge/Supabase-EBEADA?style=flat-square&logo=supabase&logoColor=000000" alt="Supabase">
<img src="https://img.shields.io/badge/Azure-EBEADA?style=flat-square" alt="Azure">
<img src="https://img.shields.io/badge/Azure%20DevOps-EBEADA?style=flat-square" alt="Azure DevOps">
<img src="https://img.shields.io/badge/GitHub%20Actions-EBEADA?style=flat-square&logo=githubactions&logoColor=000000" alt="GitHub Actions">

**On GitHub**

<img height="165" src="https://github-readme-stats.vercel.app/api?username=Hamza0590&show_icons=true&count_private=true&hide_border=true&border_radius=12&bg_color=E4E0CE&title_color=000000&text_color=000000&icon_color=000000&ring_color=000000" alt="GitHub stats">
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Hamza0590&layout=compact&hide_border=true&border_radius=12&bg_color=E4E0CE&title_color=000000&text_color=000000" alt="Top languages">

<br>

<img src="assets/exploring.svg" width="100%" alt="What's Next? Currently exploring: building Agentic AI systems that see with Computer Vision and understand people through NLP.">

<br>

<img src="assets/contact.svg" width="100%" alt="Let's Build Something Worth Researching. Working on something interesting? Open to research collaborations, research internships and AI engineering roles.">

<p>
  <a href="mailto:hamza35502@gmail.com"><img src="https://img.shields.io/badge/hamza35502%40gmail.com-FFFF23?style=for-the-badge&logo=gmail&logoColor=000000" alt="hamza35502@gmail.com"></a>
  <a href="https://linkedin.com/in/hamza35502"><img src="https://img.shields.io/badge/LinkedIn-222222?style=for-the-badge" alt="LinkedIn"></a>
</p>

<sub>© 2026 Muhammad Hamza</sub>
