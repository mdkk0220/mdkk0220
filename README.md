<h1 align="center">안녕하세요, 성명규입니다 👋</h1>
<h3 align="center">보안 자동화와 웹 개발을 공부하는 개발자</h3>

<p align="center">
  로그를 읽고, 위험을 판단하고, 사람이 결정할 수 있게 돕는 도구를 만듭니다.
</p>

<p align="center">
  건양대학교 의료IT공학과 졸업예정 · SK ALEPH 부트캠프 수강 중 (~2026.12.09)<br>
  ✉️ audrby2000@gmail.com · audrby2000@naver.com
</p>

---

## 🔭 대표 프로젝트

### 🧭 [AI-agent](https://github.com/mdkk0220/AI-agent)
**채용 공고 데이터 기반 취업 준비 에이전트 (진행 중)**
채용 공고를 매일 모으고, 내 기술과 맞는 공고를 골라 주고, 자소서 초안까지 써 주는 에이전트입니다.
- 흐름: 공고 수집 → 분석 · 맞춤 점수 → 자소서 초안 → 팩트체크 → 사람 승인
- 프로필에 없는 경험을 지어낸 문장은 팩트체크가 지우고, 승인 후에도 제출하지 않고 저장만 합니다
- `Python` `LangGraph` `Streamlit` `SQLite` `REST API`

### 🛡️ [security-agent-toolkit](https://github.com/mdkk0220/security-agent-toolkit)
**보안 관제 자동화 에이전트 (SK ALEPH 실습)**
로그 수집 → 정규화 → 룰 탐지 → LLM 요약 · 판단 → 사람 승인 → 보고서 · 알림까지, 보안 관제의 한 사이클을 파이썬으로 구현한 실습 프로젝트입니다. (SK ALEPH 부트캠프 수강 중, 기본 코드는 교육과정에서 제공받았습니다)
- 핵심 원칙: **LLM은 고르기만 하고, 실행은 코드가 하고, 되돌리기 어려운 결정은 사람이 한다**
- 계정 잠금 같은 위험한 조치는 승인 게이트를 거치고, 승인이 없으면 실행하지 않고 기록만 남깁니다
- `Python` `Flask` `Gemini API` `requests`

### 🦵 [knee-oa-classifier](https://github.com/mdkk0220/knee-oa-classifier)
**무릎 X-ray 관절염 등급 분류 (5인 팀 프로젝트)**
ResNet50으로 Kellgren–Lawrence 0~4등급을 분류하고, Grad-CAM으로 모델이 본 부위를 시각화했습니다.
- 담당: 저장소 구조 설계 · Git 관리 · ResNet50 모델 구현
- 테스트 결과: 정확도 0.72 · Macro-F1 0.73 · QWK 0.85 (테스트 이미지 3,052장)
- `Python` `PyTorch` `OpenCV` `Grad-CAM` `Gradio`

### 🤝 그 외 팀 프로젝트

**BodySync** · 4인 팀 · 2026.05 ~ 06
BMI · 기초대사량을 계산하고 식단과 운동을 안내하는 Android 앱 (Kotlin, Jetpack Compose, Gemini API)
- 담당: 앱 구조 설계 주도, 식단 탭 · 운동 탭 기능 구현, Gemini API 연동

**SHydent** · 6인 팀 · 2025.03 ~ 06
수업 중 학생이 교수에게 익명으로 질문하는 시스템. 교수용 Electron 앱에서 질문을 화면 위 오버레이로 띄웁니다 (Electron, Vite, Firebase)
- 담당: 앱 개발

---

## 📚 공부하고 있는 것

**네트워크 · 보안** ([학습 기록](https://github.com/mdkk0220/security-agent-toolkit/tree/main/network_zt))
OSI 7계층 · TCP와 Wireshark 패킷 분석 · IP 서브넷 설계 · 스위치 · 라우터 · VLAN · DNS 이상 탐지 · VPN · 방화벽 · 제로트러스트 · Docker

**접근 제어** ([실습](https://github.com/mdkk0220/security-agent-toolkit/tree/main/access_control/config))
역할 기반 접근 제어(RBAC) · 접근 로그 감사

---

## 🛠️ 기술 스택

**언어**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

**프레임워크 · 라이브러리**
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![Electron](https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)

**도구 · 인프라**
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white)
