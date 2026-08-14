<h1 align="center">Hi, I'm Ariyan 👋</h1>
<h3 align="center">Computer Engineering @ York University · Computer Vision · AI/ML · Full-Stack · Embedded Systems</h3>

<p align="center">
  <a href="https://ariyanazami.com"><img src="https://img.shields.io/badge/Portfolio-111111?style=flat-square&logo=googlechrome&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/ariyan-azami"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" /></a>
  <a href="https://www.kaggle.com/ariyanazami"><img src="https://img.shields.io/badge/Kaggle-20BEFF?style=flat-square&logo=kaggle&logoColor=white" /></a>
  <a href="mailto:ariyan.azami84@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" /></a>
</p>

---

### 🧑‍💻 About me

I'm a Computer Engineering student at York University working mainly on **real-time computer vision**, most recently ROD, a 25-class urban obstacle benchmark we built for detectors that have to run on the device in someone's pocket. I'm also a Software Developer at [Appli Solutions](https://applisolutions.com) and a Machine Learning Research Assistant at York's Laboratory of Advanced Biotechnologies.

---

### 🎯 ROD · Real-Time Obstacle Detection

<p align="center">
  <a href="https://huggingface.co/datasets/Abtinzandi/Obstacle-Detection-Dataset-YOLO"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fhuggingface.co%2Fapi%2Fdatasets%2FAbtinzandi%2FObstacle-Detection-Dataset-YOLO%3Fexpand%255B%255D%3DdownloadsAllTime&query=%24.downloadsAllTime&label=%F0%9F%A4%97%20total%20downloads&color=yellow&style=for-the-badge" alt="Hugging Face total downloads" /></a>
</p>

A pedestrian-perspective detection benchmark for assistive navigation: warning people with visual impairment, or people walking distracted, about what's in front of them, on commodity hardware with no LiDAR and no depth camera.

| | |
| :-- | :-- |
| 📦 **Dataset** | 24,326 images · 40,195 bounding boxes · 25 classes, YOLO Darknet format |
| 🗺️ **Sources** | 29 public collections reconciled by hand onto one class index, plus original street-level capture in Tehran 🇮🇷 and Toronto 🇨🇦 |
| 🏷️ **Labeling** | SAM 3 auto-annotation in a Roboflow Workflow, human-verified, with a YOLOv8n quality gate every capture campaign had to clear before release |
| 📊 **Benchmark** | 6 nano-scale detectors, YOLOv8n through YOLO26n, identical protocol on a held-out 1,629-image test split |
| 🥇 **Best results** | **0.889 recall** (YOLO12n) · **0.925 precision** (YOLO26n) · **0.882 mAP@0.50 / 0.750 mAP@0.50:0.95** from just 1.98M params (YOLOv9t) |
| ⚡ **Speed** | 12.5 ms/image, **79.7 FPS** on a single T4 |

Recall is the operating metric here, not mAP. A false positive costs a buzz the user can ignore; a false negative is an obstacle they walk into. The two rankings disagree, so picking a model on aggregate mAP does *not* give you the one that misses the fewest obstacles.

📥 [Kaggle](https://www.kaggle.com/datasets/abtinzandi/obstacle-detection-dataset) · 🤗 [Hugging Face](https://huggingface.co/datasets/Abtinzandi/Obstacle-Detection-Dataset-YOLO) · 📄 dataset paper submitted

---

### 🚀 Projects

| Project | Stack | What it is |
| :-- | :-- | :-- |
| 🤖 [**SyncAgent**](https://github.com/AriyanAzami/SyncAgent) | `Python` · zero deps | Claude Code, Gemini CLI and Codex CLI on one task, coordinated through markdown files in a folder. One agent drives and holds context; the other two run as stateless one-shot reviewers that never see the repo, which is what makes review affordable. A local dashboard shows what each one is doing and costing. |
| ⚖️ [**Prosecuto**](https://github.com/sahandsamadirad/prosecuto) | `Python` · `LangGraph` · `vLLM` · `Chroma` · `Next.js` | AI assistant for disputing Ontario red-light-camera tickets, built at **NVIDIA Spark Hack Toronto** with a team of four on ASUS GX10 / NVIDIA GB10 hardware. My part was the local-LLM path: routing inference to on-device llama-server and vLLM NVFP4 instead of a hosted API, a per-agent "thinking" toggle so fast agents skip reasoning, and the Redis lock fix that stopped long LLM turns from killing the WebSocket. |
| 🚗 [**Undercut**](https://github.com/SoroushRF/Undercut) · [live ↗](https://undercut-seven.vercel.app) | `Next.js` · `TypeScript` · `FastAPI` · `Go` · `PostgreSQL` | Used-car deal finder for the GTA that flags mathematically underpriced listings. I worked on the visualization layer: total-cost-of-ownership and price-history charts comparing market vs. listed price with percentage deltas, plus the refactor that moved the frontend to a modular design. |

---

### 🔭 What I'm working on right now

- 🤖 **Growing ROD:** extending the benchmark and the on-device detection work above.
- 💻 **Production software at Appli Solutions:** shipping backend and frontend features across the full stack of an AI-powered hiring platform.
- 🧠 **Medical imaging research:** training U-Net segmentation models and exploring Stable Diffusion-based generative pipelines for diagnostic imaging at York's Laboratory of Advanced Biotechnologies.

---

### 🛠️ Tech I work with

<table>
  <tr>
    <td valign="top" width="50%">
      <b>🧠 AI / Machine Learning</b><br><br>
      <img src="https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
      <img src="https://img.shields.io/badge/-TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white" />
      <img src="https://img.shields.io/badge/-Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
      <img src="https://img.shields.io/badge/-YOLO-00FFFF?style=flat-square&logo=yolo&logoColor=black" />
      <img src="https://img.shields.io/badge/-OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white" />
      <img src="https://img.shields.io/badge/-NumPy-013243?style=flat-square&logo=numpy&logoColor=white" />
      <img src="https://img.shields.io/badge/-Pandas-150458?style=flat-square&logo=pandas&logoColor=white" />
      <br><br>
      <i>Real-time computer vision (YOLO, OpenCV) and deep learning for medical imaging (U-Net, diffusion models).</i>
    </td>
    <td valign="top" width="50%">
      <b>⌨️ Languages</b><br><br>
      <img src="https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white" />
      <img src="https://img.shields.io/badge/-C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" />
      <img src="https://img.shields.io/badge/-Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" />
      <img src="https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
      <br><br>
      <i>Python for ML and backends; C++ for embedded and performance-critical code.</i>
    </td>
  </tr>
  <tr>
    <td valign="top" width="50%">
      <b>🌐 Full-Stack & Tools</b><br><br>
      <img src="https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" />
      <img src="https://img.shields.io/badge/-CSS3-1572B6?style=flat-square&logo=css3&logoColor=white" />
      <img src="https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white" />
      <img src="https://img.shields.io/badge/-Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
      <br><br>
      <i>Building and shipping production features end to end at Appli Solutions.</i>
    </td>
    <td valign="top" width="50%">
      <b>🔌 Hardware & Embedded</b><br><br>
      <img src="https://img.shields.io/badge/-Arduino-00979D?style=flat-square&logo=arduino&logoColor=white" />
      <img src="https://img.shields.io/badge/-Altium%20Designer-A5915F?style=flat-square&logo=altiumdesigner&logoColor=white" />
      <img src="https://img.shields.io/badge/-SolidWorks-D32E2E?style=flat-square&logo=dassaultsystemes&logoColor=white" />
      <img src="https://img.shields.io/badge/-Fusion%20360-FF6F00?style=flat-square&logo=autodesk&logoColor=white" />
      <img src="https://img.shields.io/badge/-ArduPilot-0E4D92?style=flat-square" />
      <br><br>
      <i>PCB design, CAD, and flight-controller firmware from robotics and drone builds.</i>
    </td>
  </tr>
</table>

---

### 🏆 A few highlights

- 📊 **50,000+ downloads** on the ROD dataset across [Hugging Face](https://huggingface.co/datasets/Abtinzandi/Obstacle-Detection-Dataset-YOLO) and [Kaggle](https://www.kaggle.com/datasets/abtinzandi/obstacle-detection-dataset)
- 🥇 **1st Place:** ATF Robotics Cup, National (5,000+ participants) *(competitive robotics, junior high)*
- 🥈 **2nd Place:** FIRA RoboWorldCup, National | World Finals Qualifier *(junior high)*
- 🚁 Built and tuned **custom quadcopters** with ArduPilot firmware and DJI flight controllers

---

### 📈 Activity

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.vercel.app/?user=AriyanAzami&hide_border=true&theme=github-dark-blue" />
    <img height="170" src="https://streak-stats.vercel.app/?user=AriyanAzami&hide_border=true" />
  </picture>
  &nbsp;&nbsp;
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=AriyanAzami&theme=github_dark" />
    <img height="170" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=AriyanAzami&theme=default" />
  </picture>
</p>

---

### 📫 Let's connect

- 🌐 **Portfolio:** [ariyanazami.com](https://ariyanazami.com)
- 💼 **LinkedIn:** [linkedin.com/in/ariyan-azami](https://www.linkedin.com/in/ariyan-azami)
- 📊 **Kaggle:** [kaggle.com/ariyanazami](https://www.kaggle.com/ariyanazami)
- 📧 **Email:** ariyan.azami84@gmail.com

---

<p align="center">
  <i>⚡ Open to internship and co-op opportunities in AI/ML, software, and computer vision.</i>
</p>
