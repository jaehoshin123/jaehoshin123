# Jaeho Shin

[![GitHub](https://img.shields.io/badge/GitHub-jaehoshin123-181717?logo=github)](https://github.com/jaehoshin123)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Jaeho%20Shin-0A66C2?logo=linkedin)](https://www.linkedin.com/in/jaeho-shin)
[![Blog](https://img.shields.io/badge/Blog-Personal%20Blog-orange)](https://jaehoshin123.github.io)
[![Email](https://img.shields.io/badge/Email-fluffyck%40naver.com-EA4335?logo=gmail)](mailto:fluffyck@naver.com)

---

## Summary

Passionate about intelligent systems, I aim to solve real-world problems by bridging electronic engineering, AI, and production software. My experience spans MCU-based control, autonomous systems, computer vision, and cloud-based AI services, with a focus on building reliable end-to-end systems from hardware to application.

---

## Work Experience

### MegazoneCloud &nbsp;`Jan 2025 – Mar 2025`
- Developed a LangChain-based RAG chatbot starting from an internal document QA prototype, and extended it to support AWS official documentation leveraging SearXNG and Perplexica for retrieval.
- Collaborated with a team lead using GitLab for version control and project management.
- Conducted benchmarking of multiple open-source LLMs using Ollama to evaluate performance across different models.
- Performed data quality validation for documents ingested into OpenSearch for the GenAI360 service, including chunking strategy optimization, embedding quality assessment, and LLM response accuracy evaluation.

### NTT DATA &nbsp;`July 2024 – Aug 2024`
- Conducted internal Generative AI training for the IT department at NTT Korea, introducing core pipelines and practical case studies as part of the transition beyond traditional DT initiatives.

---

## Education

| Period | Degree |
|---|---|
| 2024 – Present | B.E. in Electronic and Electric Engineering, **Sungkyunkwan University (SKKU)** (GPA: 3.9/4.5) |
| 2015 – 2018 | Kyunggi High School |

---

## Certifications

| Category | Certification |
|---|---|
| AWS | AWS Certified Solutions Architect – Associate (SAA), AWS Certified AI Practitioner |
| Data | SQLD, ADsP |
| IT | Computer Specialist in Spreadsheet & Database Level-1 |

---

## Research Outputs

### Publications

| Title | Venue | Authors | Status |
|---|---|---|---|
| ScopeCLIP: Region-Mask Training-Free OVSS with Lightweight SAM2 | **ACCV 2026** | Kim Junghun, **Shin Jaeho**, Kim Kyuri, Lim Seoyeon, Jeong Jongpil | Submitted (2026/06/23) |

> **Abstract:** Vision–language models such as CLIP provide strong open vocabulary recognition, but turning them into spatially coherent per-patch predictions for open-vocabulary semantic segmentation (OVSS) remains difficult. Region-mask methods improve training-free OVSS by using class-agnostic region masks to restrict patch attention within a region (Scope Reconstruction, SR) and to enforce a single label per region by majority voting (Map Correction, MC). We study whether a much smaller mask backbone is a practical alternative to the large SAM2 Hiera-L (224.4M params). With Hiera-Tiny (38.9M, 5.8× fewer params), ScopeCLIP reaches 43.92 avg mIoU (95% of the Hiera-L score of 46.18), while lowering average end-to-end latency by ~22% and peak memory by ~0.35 GB across 7 OVSS benchmarks.
>
> [[GitHub](https://github.com/KimJH0919/SCOPECLIP)] [[Conference](https://accv2026.org/)]

### Patents

| Title | Applicant | Inventors | Status |
|---|---|---|---|
| 경량 분할 백본 기반 영역 마스크를 이용한 학습 불요 개방형 어휘 의미론적 영상 분할 방법 및 장치 | 성균관대학교 산학협력단 | 정종필, 김정훈, **신재호**, 김규리, 임서연 | Pending (Ref: R-2026-0537-KR-1) |

### Software Copyright

| Title | Creators | Created | Status |
|---|---|---|---|
| 경량SAM2백본기반학습불요개방어휘의미론적분할소프트웨어 | 정종필, 김정훈, **신재호**, 임서연, 김규리 | 2026-06-08 | Registration pending |

---

## Projects

### ScopeCLIP: Region-Mask Training-Free Open-Vocabulary Semantic Segmentation with Lightweight SAM2
**SmartFactory Capstone Design 1, SKKU** &nbsp;`Mar 2026 – Jun 2026`

> Team SF13 | Advisor: Prof. Jeong Jongpil | Industry partner: Duplex

- Built the SAM2 mask generation pipeline (automatic mask generator setup, patch grid conversion) and implemented Hiera-L / Hiera-Tiny backbone switching.
- Integrated Scope Reconstruction (SR) — region-constrained attention masking in the final CLIP transformer block — and Map Correction (MC) into the NACLIP baseline to form the ScopeCLIP system.
- Evaluated across 7 OVSS benchmarks (VOC20/21, PC59/60, COCO-Object/Stuff, ADE20K): ScopeCLIP (Hiera-L) achieves **46.18 avg mIoU** (+6.20 over NACLIP baseline); lightweight Hiera-Tiny reaches **43.92 mIoU** (95% of Hiera-L) with −22% latency and −0.35 GB peak memory.
- Outcomes: ACCV 2026 paper submission, patent application, SW copyright registration.

### U-Net-based Semantic Segmentation &nbsp;`(ICE-3056)`
- Built a fully convolutional semantic segmentation model inspired by U-Net, using an encoder-bottleneck-decoder architecture for pixel-wise classification.
- Designed convolutional encoder and transposed-convolution decoder blocks with BatchNorm and ReLU to capture semantic context and restore spatial resolution.
- Combined Cross-Entropy Loss with Dice Loss to address class imbalance in under-represented segmentation classes.
- Evaluated with 5-fold validation, achieving a best validation mAP of 0.874 and a test mAP of 0.754.

### AI-Powered Emergency Support System &nbsp;`(SKT Fly AI 8th)`
[www.aegis119.com](http://www.aegis119.com) *(closed)*
- Designed a LangGraph-based multi-agent system with conditional routing, improving performance by 20% over baseline RAG.
- Integrated LLM/SLM for cost-efficient inference and aligned workflow with KTAS triage logic.
- Built and deployed containerized Spring/FastAPI services with CI/CD on AWS ECS.

### Pregnancy Success Prediction Model &nbsp;`(LG Aimers 6th)`
- Developed a classification model to predict pregnancy outcomes for infertility patients.
- Applied multivariate imputation, normalization (StandardScaler), and ensemble learning (Random Forest, XGBoost, stacking).
- Improved performance over single models, achieving a final ROC-AUC of ~0.75.

### Smart Process Monitoring &nbsp;`(SKKU Capstone Project)`
- Built an IoT monitoring system integrating sensor networks with MQTT-based data pipelines.
- Designed real-time data storage and visualization using InfluxDB and Grafana.
- Developed a real-time fire detection module by fine-tuning the FireNet deep neural network.

### CV Lab Intern – 3D Map Project
- Built a campus-scale feature map using Visual SLAM (ORB-SLAM3).
- Improved robustness via IMU sensor fusion to address mapping discontinuities.
- Resolved calibration and sensor integration issues using 3DoF transformations and ROS node implementation.

### Autonav Lab Intern – ERP-42 Autonomous Driving System &nbsp;`(with MORAI)`
- Contributed to decision and control modules for an autonomous driving system using ERP-42 in collaboration with MORAI.
- Implemented path tracking using the Pure Pursuit algorithm and developed rule-based stopping logic for traffic lights and pedestrian scenarios.
- Resolved coordinate system inconsistencies by converting LLA to ENU, enabling accurate simulation-based localization.

### FPGA Analog Clock System &nbsp;`(ICE-2005)`
- Implemented VGA display modules and contributed to main clock logic for a Verilog-based FPGA analog clock system.
- Designed VGA timing and rendering logic to display an analog clock face with hour, minute, and second hands.
- Integrated FPGA I/O features including DIP/PUSH switch-based time setting, speed scaling, LED time indication, piezo-buzzer alerts, and 7-segment display output.
- Improved hardware interaction reliability by applying debouncing logic and modularizing the system into main clock, VGA, LED, buzzer, 7-segment, and top-level modules.

### Driving Lift Robot &nbsp;`(ICE-3015)`
- Developed a driving lift robot by integrating a custom H-Bridge motor driver, lift mechanism, and embedded control logic.
- Designed the motor driver circuit from scratch without dedicated driver ICs, selecting NMOS/PMOS components based on voltage, current, and power constraints.
- Implemented register-level motor control using timer/counter configuration and interrupt-based logic for precise operation.
- Resolved hardware-software integration issues through datasheet analysis, circuit redesign, and systematic debugging.

### Tambourine Expense Management App Backend &nbsp;`(UMC 5th)`
- Developed backend services for "Tambourine," an expense management application, as a backend developer in the UMC 5th university club program.
- Built RESTful APIs using Node.js and Express, applying a DTO-based structure to improve code consistency, maintainability, and request-response validation.
- Designed the service database schema and ERD for core domains including users, categories, items, notifications, and search history, considering scalability and query efficiency.
- Utilized AWS EC2 for backend server deployment and AWS S3 for file/static asset storage.

### Real-time ADAS with YOLOv5 and Sensor Fusion &nbsp;`(ICE-4104)`
- Adapted a COCO-pretrained YOLOv5 object detection model for Korean road environments by adding a custom water deer class through transfer learning.
- Built a custom-labeled dataset with LabelImg and expanded the YOLOv5 detection label space from 80 COCO classes to 81 classes.
- Optimized model training by tuning epochs, batch size, and optimizer settings, improving detection reliability for vehicles, pedestrians, and wildlife objects.
- Developed a real-time ADAS prototype by combining YOLOv5 inference, Arduino serial communication, and ultrasonic sensor-based distance recognition to control motor speed according to detected hazards.

---

## Skills

| Category | Tools |
|---|---|
| Programming | C/C++, JavaScript, Python, Java |
| AI / ML | PyTorch |
| Backend | Express.js, Spring |
| Frontend | React |
| DevOps | Linux, AWS, CI/CD, Docker, Kubernetes |
| Databases | MySQL, MongoDB, PostgreSQL |

---

*Last updated: June 2026*
