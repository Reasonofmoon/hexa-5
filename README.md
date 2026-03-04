# 🏗️ hexa-5: 건설/부동산 AX 마스터클래스

> "계약서를 AI가 리뷰한다" — 건설/부동산 중소기업을 위한 AI 자동화 실습 과정

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Reasonofmoon/hexa-5/blob/main/notebooks/M7_CONSTRUCTION_contract_lab.ipynb)

---

## 🎯 이 과정은?

**대상**: 건설업체, 부동산개발, 설계사무소, 인테리어 업체  
**목표**: 계약서 자동 분석·현장보고서·리스크 관리 3가지 핵심 자동화  
**시간**: 6시간 (강의 3h + 실습 3h)

---

## 🎯 수준별 활용 가이드

### 🟢 Starter — "5분 안에 계약서 리뷰"
1. `labs/M7-CONSTRUCTION/README.md` 열기
2. 프롬프트 복사 → ChatGPT/뤼튼에 붙여넣기
3. 계약서 종류·주요 조건만 수정 후 Enter
4. 리스크 분석 즉시 출력 ✅ (코딩 0줄)

### 🔵 Professional — Colab 자동화
```python
# Colab Secret에 저장 (이름: GEMINI_API_KEY)
from google.colab import userdata
api_key = userdata.get('GEMINI_API_KEY')
```
1. Colab 뱃지 클릭 → 노트북 오픈
2. 런타임 → 모두 실행
3. 계약서 정보 셀만 수정
4. 리뷰 결과 + 현장보고서 CSV 자동 다운로드

### 🟣 Enterprise — 멀티 에이전트 파이프라인
- OMC `/team 3:executor`로 계약→리스크→현장→보고서 자동화
- `AGENTS.md` 기반 법률/기준 준수 내재화
- `scripts/agents_config_validator.py` 셀프 검증

---

## ⚙️ 3모듈 커리큘럼

| 모듈 | 제목 | Colab | Labs |
|---|---|---|---|
| M1 | AX 진단 & 건설 벤치마킹 | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](notebooks/M1_AX_diagnosis.ipynb) | [labs/M1](labs/M1-diagnosis/) |
| M7-CONSTRUCTION | 계약서 분석 & 현장보고서 | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](notebooks/M7_CONSTRUCTION_contract_lab.ipynb) | [labs/M7-CONSTRUCTION](labs/M7-CONSTRUCTION/) |
| M9 | 현장관리 & 자동 보고 시스템 | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](notebooks/M9_site_management.ipynb) | [labs/M9](labs/M9-deploy/) |

---

## 📂 프로젝트 구조

```
hexa-5/
├── notebooks/
│   ├── M1_AX_diagnosis.ipynb              ← AX 진단 자동화
│   ├── M7_CONSTRUCTION_contract_lab.ipynb   ← 계약서 분석 ★
│   └── M9_site_management.ipynb           ← 현장관리 자동화
├── labs/
│   ├── M1-diagnosis/README.md              ← 진단 프롬프트 모음
│   ├── M7-CONSTRUCTION/README.md         ← 건설 실습 가이드
│   └── M9-deploy/README.md               ← 배포 체크리스트
├── scripts/
│   ├── contract_analyzer.py              ← 계약서 분석 (실행 가능)
│   ├── site_report_generator.py           ← 현장보고서 생성
│   └── agents_config_validator.py         ← AGENTS.md 검증
└── shared/
    └── construction_contracts_sample.csv   ← 샘플 계약서 데이터 (20행)
```

---

## 🌐 hexa 시리즈
- [hexa-1](https://github.com/Reasonofmoon/hexa-1): 🏭 제조업
- [hexa-2](https://github.com/Reasonofmoon/hexa-2): 🍽️ 외식/F&B
- [hexa-3](https://github.com/Reasonofmoon/hexa-3): 🛒 소매/유통
- [hexa-4](https://github.com/Reasonofmoon/hexa-4): 📚 교육/에드테크
- **hexa-5** (현재): 🏗️ 건설/부동산
- [hexa-6](https://github.com/Reasonofmoon/hexa-6): 💼 전문서비스/IT

Made with ❤️ by [Reasonofmoon × Antigravity](https://github.com/Reasonofmoon)  
중소기업 AX 전환을 위한 실전 교육