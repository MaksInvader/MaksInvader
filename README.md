# Muhammad Adrean Karim Syauqy

<p align="left">
  <b>Computer Engineering Graduate (Cum Laude, 3.62 GPA) — Telkom University</b><br>
  <i>Firmware Architecture (ESP-IDF, FreeRTOS) • Edge AI Inference • Data Engineering</i><br>
  Bandung, Indonesia
</p>

<p align="left">
  <a href="https://www.linkedin.com/in/muhammad-adrean-karim-syauqy-504793284/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://github.com/MaksInvader"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub" /></a>
  <a href="mailto:adreansyauqy@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://maksinvader.github.io/360Portfolio/"><img src="https://img.shields.io/badge/Portfolio-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="Portfolio" /></a>
</p>

<br>

## Overview

I am a Computer Engineering graduate from Telkom University working across the embedded firmware, computer vision, and distributed telemetry stack.

* **Published Research:** First author at **IEEE ICoDSA 2026** evaluating lightweight semantic segmentation (PIDNet-M) under extreme 1:342 pixel imbalance.
* **Firmware & RTOS:** Built production **C/C++ firmware (native ESP-IDF / FreeRTOS)** with custom partition tables, dual-bank OTA rollback, and dynamic I2C bus recovery for an externally commissioned agricultural capstone (IDR 8M budget).
* **Edge AI & Pipelines:** Deployed hardware-accelerated computer vision (CUDA/cuDNN), multi-stream RTSP ingestion (MediaMTX/FFmpeg), and vector search (LanceDB) with automated container telemetry.
* **DevOps & CI/CD:** Engineered automated Dockerized ESP-IDF cross-compilation workflows in GitHub Actions with binary header patching and automated release packaging.

<br>

## Featured Projects

### [🌱 HydroponicsIDF — Resilient ESP32-S3 Agricultural Firmware](https://github.com/MaksInvader/HydroponicsIDF)
Production firmware for an externally commissioned agricultural automation unit (IDR 8M budget) with continuous 14-day zero-downtime field resilience.
* Architected fail-safe **dual-bank Over-The-Air (OTA)** flashing with automatic rollback via custom flash partitions (`partitions.csv`), isolating sensor calibration states in NVS.
* Resolved multi-device I2C clock-stretching and bus-hang conditions across 4 concurrent sensor peripherals via timeout state machines and dynamic bus recovery.
* Implemented an embedded SoftAP captive HTTP web portal for headless network provisioning.
* Automated firmware builds, binary header patching (`esptool.py`), and release asset packaging via containerized **GitHub Actions CI/CD pipelines**.
* **Stack:** C, C++, Native ESP-IDF, FreeRTOS, ESP32-S3, MQTT (Mosquitto), NVS, Docker, GitHub Actions

### [🔥 PIDNet-Wildfire-Segmentation — IEEE Research Benchmark](https://github.com/MaksInvader/PIDNet-Wildfire-Segmentation)
Official codebase for our paper presented at the 9th IEEE International Conference on Data Science and Its Applications (ICoDSA 2026).
* Evaluated PIDNet-M across an extreme **1:342 Fire-to-Smoke pixel imbalance** (0.0016% active flame pixels) on the FIgLib dataset.
* Uncovered critical over-regularization failure modes where combined loss functions (Lovasz, Focal, Dice) inflated precision to 88.5% but collapsed Fire Recall from **91.1% down to 46.3%**.
* Benchmarked zero-shot cross-dataset generalization on the FLAME and MultiNatSmoke datasets to expose scale-shift vulnerabilities.
* **Stack:** Python, PyTorch, PIDNet-M, CUDA, FIgLib Dataset, SAHI Tiling

### [🍞 FOMO Sandwich — Full-Stack Web Ordering Platform](https://github.com/MaksInvader/Fomo-business)
Responsive food ordering application featuring type-safe forms, real-time Firestore persistence, and automated payment flows.
* End-to-end schema validation using React Hook Form and Zod with custom delivery and price calculations.
* Dynamic **QRIS payment payload generation** with live countdown timers.
* Reusable Firebase Firestore data layer with unique order tracking and cancellation safeguards.
* Configured unit test utilities using **Vitest**.
* **Stack:** React 19, TypeScript, Vite, Tailwind CSS, Firebase Firestore, Zod, Vitest

### [💬 Ruang Opini — Multi-Stage LLM Prompt Engineering & Alignment](https://github.com/StevannW/Ruang-Opini)
Automated 5-stage multimodal political content evaluation engine powered by Gemini 2.5 Flash.
* Authored comprehensive system prompts and persona guardrails ensuring API calls strictly adhered to factual objectivity and structured JSON schemas.
* Engineered prompt-based sarcasm and cultural slang detection logic to prevent polarity errors in Indonesian political sentiment analysis.
* Structured multi-stage prompts coordinating visual description, dynamic entity search query generation, and real-time RAG fact-verification.
* **Stack:** Google Gemini 2.5 Flash API, Prompt Engineering, RAG, Python

### [🚦 Taipei City Traffic Sensor Analysis Pipeline](https://github.com/StevannW/TaipeiPrediction)
High-volume data cleaning, statistical anomaly detection, and exploratory data analysis pipeline for urban traffic forecasting.
* Preprocessed and engineered temporal/spatial features across **2.4M+ sensor records** and **23,600+ detector nodes** from Taipei City.
* Built reusable data cleaning modules in Python (Pandas, NumPy, Scipy) implementing statistical anomaly detection, distribution tests, and outlier clipping.
* **Stack:** Python, Pandas, NumPy, Scipy, Seaborn, Matplotlib

<br>

## Experience & Leadership

### Laboratory Assistant (Practical Study Division)
**Everything Connected Laboratory — Telkom University** *(Feb. 2025 – Sep. 2025)*
* Mentored 32 engineering students across 8 cohort teams in practical IoT infrastructure, embedded networking, and hardware interfacing.
* Guided hands-on lab sessions covering physical Cisco routing appliances, dynamic routing topologies (OSPF, BGP), VLAN segmentation, and packet inspection using Wireshark.

### Computer Vision / Edge AI Engineering Intern
**Nusameta** *(Jul. 2025 – Aug. 2025)*
* Deployed real-time facial recognition pipelines (FaceNet, OpenCV) with hardware-accelerated CUDA and cuDNN execution.
* Integrated MediaMTX and FFmpeg for multi-camera RTSP ingestion, writing vector embeddings to LanceDB and telemetry to InfluxDB.
* Packaged multi-service vision stacks into isolated Docker Compose bridge networks with healthchecks and Prometheus/Grafana monitoring.

<br>

## Technical Stack

* **Languages:** C, C++, Python, TypeScript, JavaScript, SQL (MySQL), C# (ASP.NET Core)
* **Embedded & Hardware:** Native ESP-IDF, FreeRTOS, ESP32-S3, I2C/SPI/UART, Dual-Bank OTA, NVS, SoftAP, CMake
* **AI & Vision:** PyTorch, OpenCV, CUDA, cuDNN, LanceDB (Vector DB), FaceNet, PIDNet, Gemini API, RAG
* **DevOps & Linux:** Docker Compose, GitHub Actions (CI/CD), Headless Linux (Ubuntu), Prometheus, Grafana, WireGuard VPN
* **Data & Protocols:** InfluxDB, MySQL, MQTT (Mosquitto), RTSP, MediaMTX, Wireshark, Git

<br>

## Contact

* **Email:** [adreansyauqy@gmail.com](mailto:adreansyauqy@gmail.com)
* **LinkedIn:** [linkedin.com/in/muhammad-adrean-karim-syauqy-504793284](https://www.linkedin.com/in/muhammad-adrean-karim-syauqy-504793284/)
* **GitHub:** [github.com/MaksInvader](https://github.com/MaksInvader)
