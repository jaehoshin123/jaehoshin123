# 신재호 (Jaeho Shin)

**전자전기공학부 4학년** | 성균관대학교 (2022315911) | fluffyck@skku.edu 

---

##  학력

| 기간 | 학교 | 전공 |
|------|------|------|
| 2022.03 – 2026.08 | 성균관대학교 | 전자전기공학부 |

---

개요

스마트팩토리 비전 검사 환경에서, 사전학습된 시각-언어 모델 CLIP을 추가 학습 없이 활용하여 자연어 텍스트로 임의 클래스를 지정하는 개방어휘 의미 분할(Open-Vocabulary Semantic Segmentation, OVSS) 시스템 ScopeCLIP을 구성하였다. CLIP 패치 특징의 inter-class correlation 문제를 SAM2 영역 마스크 기반의 두 연산으로 보완한다.


Scope Reconstruction (SR): SAM2 마스크를 patch grid로 변환하여 같은 영역 내 패치끼리만 어텐션이 일어나도록 마지막 어텐션의 softmax 직전에 타 영역 가중치를 −∞로 차단. CLS 토큰 행·열은 마스킹 제외하여 전역 표현 유지.
Map Correction (MC): 풀해상도 예측맵에서 각 영역 내 화소 라벨을 최빈 라벨로 통일하여 고립 오분류 제거.


마스크를 생성하는 SAM2 백본(Hiera-L vs. Hiera-Tiny)의 정확도–비용 trade-off를 7개 OVSS 벤치마크에서 정량 분석하여, 경량 백본의 현장 적용 가능성을 검증하였다.

개발 환경

항목내용HardwareNVIDIA A100 80GB (단일 GPU)기반 모델CLIP ViT-B/16, SAM2 (Hiera-L / Hiera-Tiny)FrameworkPython, PyTorch, mmsegmentation데이터셋공개 OVSS 벤치마크 7종 (VOC20/21, PC59/60, COCO-Object/Stuff, ADE20K)마스크 생성points_per_side=8, pred-IoU·stability threshold=0.4, FP16, 마스크 병합 미사용

정량 결과

모델VOC21VOC20PC60PC59ObjectStuffADE평균 mIoU지연시간 (ms/img)파라미터NACLIP (baseline)58.8979.7132.2035.1933.1523.3017.4239.9842.97—ScopeCLIP (Hiera-L)72.0787.1137.9141.0139.7926.4618.9346.18128.87224.4MScopeCLIP (Hiera-Tiny)68.1183.4636.3239.3236.8725.2618.1143.92100.7638.9M


SR·MC 통합(Hiera-L)으로 평균 mIoU +6.20 향상 (베이스라인 대비 +15.5%)
객체 중심 벤치마크에서 향상 두드러짐: VOC21 +13.18, COCO-Object +6.64
Hiera-Tiny: Hiera-L 대비 파라미터 약 5.8배 절감, 지연시간 약 22% 단축(−28ms/img), peak memory 약 0.35GB 감소, 평균 정확도 약 95% 유지

---

## 연구논문

### 팀 논문

| 제목 | 학회/저널 | 상태 |
|------|-----------|------|
| ScopeCLIP: Region-Mask Training-Free Open-Vocabulary Semantic Segmentation with Lightweight SAM2 | ACCV 2026 | 투고 예정 |

---

## 연구성과

### 특허 출원

<img width="1576" height="219" alt="13팀_SW신청 (1)" src="https://github.com/user-attachments/assets/18c1e140-8567-45ce-bab4-95d2ac215d26" />

### SW 저작권 등록

<img width="740" height="613" alt="image" src="https://github.com/user-attachments/assets/81126f21-4a43-46b2-b3cf-9eb0a9bfb99c" />

