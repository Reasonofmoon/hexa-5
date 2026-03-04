<div align="center">

# 🏗️ hexa-5: 건설 AX 마스터클래스

### *AI로 건설 현장을 혁신하는 12주 실전 과정*

**계약서분석부터 공정KPI까지 — 현장 데이터로 직접 검증하는 AX 커리큘럼**

[![Version](https://img.shields.io/badge/version-1.0.0-6366f1?style=for-the-badge)](https://github.com/Reasonofmoon/hexa-5)
[![Colab](https://img.shields.io/badge/Google_Colab-12개_노트북-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)](https://github.com/Reasonofmoon/hexa-5/tree/main/notebooks)
[![Sector](https://img.shields.io/badge/Sector-Construction-2563eb?style=for-the-badge&logo=building&logoColor=white)](https://github.com/Reasonofmoon/hexa-5)
[![License](https://img.shields.io/badge/License-MIT-a78bfa?style=for-the-badge)](LICENSE)
[![Scripts](https://img.shields.io/badge/CLI_Scripts-8개-22d3ee?style=for-the-badge&logo=python)](scripts/)

> **"건설 현장에서 AI 도구를 사용할 수 있는 인력은 전체의 6% 미만이다."**  
> hexa-5는 코딩 경험이 없는 현장 관리자·시공사도 Colab 노트북으로  
> 바로 실전 결과를 내도록 설계된 **12주 실무 중심 AX 커리큘럼**입니다.

[📗 커리큘럼 시작](notebooks/) · [🔧 스크립트 도구](scripts/) · [📂 실습 데이터](shared/) · [🐛 이슈](../../issues)

</div>

---

## 🧠 Philosophy — "왜 건설 AX인가"

기존 건설업 AI 교육의 문제: **공정 데이터가 없이 이론만 있다**.

| 기준 | 기존 AI 교육 | hexa-5 AX 커리큘럼 |
|------|-------------|-------------------|
| 데이터 | 가상의 공정 데이터 | **실제 현장 CSV** (공정, 안전, 비용) |
| 결과물 | 모델 정확도 숫자 | **리스크 분석 + 현장보고서 + 견적서** |
| 난이도 | Python 필수 | **Colab 실행만으로 완성** |
| 기간 | 3개월+ 이론 | **Week 1부터 실전 결과** |
| 연결성 | 개별 실습 | **W1→W12 파이프라인으로 연결** |

```mermaid
graph LR
    A[📋 W1-2 계약서분석] --> B[📝 W3-4 공정보고]
    B --> C[📊 W5-6 공정KPI]
    C --> D[📨 W7-8 안전점검]
    D --> E[🔮 W9-10 견적자동화]
    E --> F[🎛️ W11-12 통합대시보드]
    
    style A fill:#6366f1,color:#fff
    style F fill:#22d3ee,color:#fff
```

---

## ⚙️ 시스템 레이어

### Layer 1 · Foundation (W1~W4) — AI 기초 도구화
> **Wow**: 10개 계약서 리스크를 AI가 **5초 안에** 자동 분석

| 주차 | 노트북 | 핵심 도구 |
|------|--------|-----------|
| W1 | M1_AX_diagnosis.ipynb | Gemini API, 자가진단 |
| W2 | W02_contract_analysis.ipynb | 계약서 리스크 분석, 조항 검토 |
| W3 | W03_progress_report.ipynb | 공정 보고서, 현장 상황 |
| W4 | W04_safety_inspection.ipynb | 안전 점검, 위험 요소 파악 |

### Layer 2 · Analytics (W5~W8) — 데이터 기반 의사결정
> **Wow**: 공정률·원가·안전지수를 **클릭 한 번**에 경영진 차트로 변환

| 주차 | 노트북 | 핵심 도구 |
|------|--------|-----------|
| W5 | W05_process_kpi.ipynb | pandas, matplotlib, 공정 KPI |
| W6 | W06_cost_analysis.ipynb | 원가 분석, 예측 |
| W7 | W07_estimate_automation.ipynb | 견적서 자동화 |
| W8 | W08_partner_communication.ipynb | 협력사 커뮤니케이션 |

### Layer 3 · Intelligence (W9~W12) — 자동화 운영 시스템
> **Wow**: 공정 지연 시 **자동 원인분석 → 협력사 알림 → 일정 조정** 파이프라인

| 주차 | 노트북 | 핵심 도구 |
|------|--------|-----------|
| W9 | W09_anomaly_detection.ipynb | 이상 감지, 예지보전 |
| W10 | W10_site_photo_analysis.ipynb | 현장 사진 분석, 진행률 |
| W11 | W11_construction_dashboard.ipynb | 종합 건설 대시보드 |
| W12 | W12_integrated_operation.ipynb | 통합 운영 시스템 발표 |

---

## 🎯 수준별 활용 가이드

### 🟢 Starter — "5분 안에 첫 결과"
1. [W2 노트북](https://colab.research.google.com/github.com/Reasonofmoon/hexa-5/blob/main/notebooks/W02_contract_analysis.ipynb) 클릭 → Colab에서 열기
2. `CONSTRUCTION_INFO`에 공종·규모만 입력 (`✏️` 표시 찾기)
3. `Shift+Enter`로 위에서 아래로 실행
4. 계약서 리스크 분석 + 보고서 자동 다운로드

> ⚠️ API 키 발급: [Google AI Studio](https://aistudio.google.com/apikey) → GEMINI_API_KEY

### 🔵 Professional — "내 현장 데이터로 실전 분석"
1. `shared/construction_contracts_sample.csv` 구조 확인
2. 내 현장 데이터를 같은 형식으로 준비
3. W5~W6 노트북에서 CSV 업로드 → 공정 KPI·원가 자동 분석
4. W8 노트북에서 협력사 연결 → 일일 공정 자동 공유

```bash
# CLI 스크립트 직접 사용
python scripts/contract_analyzer.py --input shared/construction_contracts_sample.csv
python scripts/process_kpi_calculator.py --input data.csv --output results.csv
python scripts/site_report_generator.py --input data.csv --webhook [WEBHOOK_URL]
```

### 🟣 Enterprise — "팀 표준화 & 파이프라인"
1. `scripts/M9_demo_runner.py` 실행 → 전체 파이프라인 원클릭 시연
2. GitHub Actions로 매일 자동 공정 진도 스케줄링
3. W11~W12를 내부 대시보드로 배포 (Flask/Streamlit)
4. hexa-1, hexa-6과 연계해서 업종 간 벤치마킹

---

## 📂 디렉토리 구조

```
hexa-5/
├── notebooks/          ← 12주 Colab 노트북 (W01~W12)
│   ├── W02_contract_analysis.ipynb       # 계약서 리스크 분석
│   ├── W03_progress_report.ipynb         # 공정 보고서
│   ├── W04_safety_inspection.ipynb       # 안전 점검
│   ├── W05_process_kpi.ipynb            # 공정 KPI 분석
│   ├── W06_cost_analysis.ipynb           # 원가 분석
│   ├── W07_estimate_automation.ipynb     # 견적서 자동화
│   ├── W08_partner_communication.ipynb   # 협력사 커뮤니케이션
│   └── W09_anomaly_detection.ipynb       # 이상 감지
├── scripts/            ← CLI 실행 가능 Python 스크립트
│   ├── contract_analyzer.py              # 계약서 리스크 분석기
│   ├── progress_reporter.py             # 공정 보고서 생성기
│   ├── safety_inspector.py              # 안전 점검 자동화
│   ├── process_kpi_calculator.py       # 공정 KPI 계산기
│   ├── cost_analyzer.py                # 원가 분석기
│   ├── estimate_generator.py            # 견적서 생성기
│   ├── site_report_generator.py         # 현장 보고서 생성
│   └── M9_demo_runner.py              # 원클릭 데모 런처
├── shared/             ← 실습 데이터
│   ├── construction_contracts_sample.csv # 계약서 데이터 샘플
│   └── site_progress_sample.csv        # 현장 진행률 샘플
└── labs/               ← 실습 가이드 (M2~M7)
    ├── M2-contract/README.md
    ├── M3-progress/README.md
    ├── M4-safety/README.md
    └── M7-construction/README.md
```

---

## 🔧 확장 가이드

| 우선순위 | 커스터마이징 | 난이도 | 영향 범위 |
|----------|--------------|--------|-----------|
| **1st** | `CONSTRUCTION_INFO` 딕셔너리 수정 | ⭐ | 공종·규모·기간 |
| **2nd** | 샘플 CSV를 실제 데이터로 교체 | ⭐⭐ | 분석 결과 전체 |
| **3rd** | 협력사 Webhook 연결 | ⭐⭐ | 실시간 공유 |
| **4th** | 현장 사진 API 인증 설정 | ⭐⭐⭐ | 시각화 자동화 |
| **5th** | W11~W12 대시보드 서버 배포 | ⭐⭐⭐ | 팀 공유 시스템 |

---

## 🚀 빠른 시작

```bash
# 1. 레포 클론
git clone https://github.com/Reasonofmoon/hexa-5.git
cd hexa-5

# 2. 환경 설정 (로컬 실행 시)
pip install google-generativeai pandas matplotlib gspread requests

# 3. 데모 실행
python scripts/M9_demo_runner.py

# 4. 계약서 분석 바로 실행
python scripts/contract_analyzer.py --input shared/construction_contracts_sample.csv
```

또는 **Colab에서 바로 실행** (설치 불필요):  
[![W2 열기](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github.com/Reasonofmoon/hexa-5/blob/main/notebooks/W02_contract_analysis.ipynb)
[![W6 열기](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github.com/Reasonofmoon/hexa-5/blob/main/notebooks/W06_cost_analysis.ipynb)
[![W9 열기](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github.com/Reasonofmoon/hexa-5/blob/main/notebooks/W09_anomaly_detection.ipynb)

---

## 🔗 전체 AX 시리즈

| 레포 | 섹터 | 핵심 모듈 |
|------|------|-----------|
| [hexa-1](https://github.com/Reasonofmoon/hexa-1) | 🏭 제조업 | OEE, 불량분류, 예지보전 |
| [hexa-2](https://github.com/Reasonofmoon/hexa-2) | 🍽️ F&B | 리뷰분석, 메뉴카피, 재고예측 |
| [hexa-3](https://github.com/Reasonofmoon/hexa-3) | 🛒 소매/유통 | 상품카피, CRM, SEO |
| [hexa-4](https://github.com/Reasonofmoon/hexa-4) | 📚 교육 | 교안자동화, 성적분석, 챗봇 |
| **hexa-5** (현재) | 🏗️ 건설 | 계약서분석, 공정관리 |
| [hexa-6](https://github.com/Reasonofmoon/hexa-6) | 💼 IT/서비스 | 제안서, 코드리뷰, KPI |

---

## 🌐 다국어 지원

| 항목 | 현황 |
|------|------|
| 노트북 UI | 한국어 |
| 스크립트 출력 | 한국어 (컬럼 자동감지: 한/영) |
| 샘플 데이터 | 한국어 컬럼명 |
| README | 한국어 / English (예정) |

---

*AX Consulting Curriculum © 2026 | Powered by Google Gemini*