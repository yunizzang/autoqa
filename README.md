# AutoQA 🧠
AI 기반 테스트 케이스 자동 생성 및 실행 시스템

## 📌 프로젝트 개요
**AutoQA**는 QA 테스트 자동화를 위해 개발된 Python 기반 플랫폼으로,  
테스트 케이스 생성 → 실행 → 리포트까지 전 과정을 자동화한 시스템입니다.  
본 프로젝트는 실제 B2C 서비스 QA 프로세스 개선 및 CI/CD 자동화를 목표로 합니다.

---

## ⚙️ 기술 스택
- **Language**: Python 3.11  
- **Frameworks**: pytest, Selenium, Requests  
- **CI/CD**: GitHub Actions  
- **Reporting**: Allure  
- **AI Integration**: OpenAI API (테스트케이스 자동 생성)

---

## 🚀 주요 기능
| 기능 | 설명 |
|------|------|
| 🤖 AI Test Generator | 서비스 플로우 설명만 입력하면 자동으로 테스트케이스를 생성 |
| 🔗 API & UI 테스트 | API 및 Selenium UI 테스트 자동 실행 |
| ⚙️ CI/CD 파이프라인 | GitHub Actions를 통해 자동 테스트 및 리포트 배포 |
| 📊 Allure 리포트 | 테스트 결과를 시각화한 리포트 자동 생성 |
| 🧠 Self-Learning | 실패 케이스를 기반으로 AI가 재학습 후 재테스트 제안 (optional) |

---

## 📈 기대 효과
- 테스트케이스 작성 시간 **60% 단축**
- QA 반복 업무 자동화로 **품질 안정성 향상**
- 테스트 커버리지 **30% 이상 증가**
- CI/CD 기반의 **지속적 품질 관리 체계 정립**

---

## 🧩 프로젝트 구조

autoqa/
├── tests/
│ ├── ui/
│ ├── api/
│ └── data/
├── reports/
│ └── allure-results/
├── utils/
│ ├── openai_helper.py
│ ├── config_loader.py
│ └── report_parser.py
├── requirements.txt
├── main.py
├── .github/workflows/ci.yml
└── README.md

## 🧩 실행 방법
pip install -r requirements.txt
pytest --alluredir=reports/allure-results
allure serve reports/allure-results

