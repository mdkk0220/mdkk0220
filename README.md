# 성명규

> 서버와 네트워크를 직접 구축하고, 반복되는 작업을 코드로 자동화합니다.

- 🏢 **브이엠솔루션** · 기술지원 엔지니어 (2026.11 ~)
- 🎯 관심 분야: 인프라 운영 자동화 · 보안 관제
- 📫 audrby2000@gmail.com

---

## 🔭 대표 프로젝트

### 🖧 [VMS-hw](https://github.com/mdkk0220/VMS-hw)
**가상화 환경 인프라 실습 (진행 중)**
VirtualBox에 Rocky Linux 9.8 · 8.10 서버를 구축하고, 네트워크 이중화(bonding)부터 WEB · DB 이중화, 백업 자동화까지 단계별로 실습하고 있습니다.
- 서버 두 대에 bond를 두 개씩 구성하고, 랜선 하나를 끊어도 ping 손실 1~2개로 넘어가는 것을 확인했습니다
- 겪은 장애와 일부러 낸 장애를 증상 · 원인 · 조치 · 재발 방지 순서로 기록합니다
- `Rocky Linux` `VirtualBox` `nmcli` `Bonding` `Shell Script`

### 🛡️ [security-agent-toolkit](https://github.com/mdkk0220/security-agent-toolkit)
**보안 관제 자동화 에이전트 (SK ALEPH 실습)**
로그 수집 → 정규화 → 룰 탐지 → LLM 요약 · 판단 → 사람 승인 → 보고서 · 알림까지, 보안 관제의 한 사이클을 파이썬으로 구현했습니다. 기본 코드는 교육과정에서 제공받았습니다.
- 핵심 원칙: **LLM은 고르기만 하고, 실행은 코드가 하고, 되돌리기 어려운 결정은 사람이 한다**
- 계정 잠금 같은 위험한 조치는 승인 게이트를 거치고, 승인이 없으면 실행하지 않고 기록만 남깁니다
- 단계별 실습
  - [네트워크 · 제로트러스트](https://github.com/mdkk0220/security-agent-toolkit/tree/main/network_zt_2): 서브넷 설계 · VLAN · DNS · VPN · 방화벽 · Wireshark 패킷 분석
  - [접근 제어](https://github.com/mdkk0220/security-agent-toolkit/tree/main/access_control_3): RBAC · 예외 권한 · 권한 점검과 회수
  - [이상 탐지](https://github.com/mdkk0220/security-agent-toolkit/tree/main/anomaly_detection_4): 로그 정규화 · 규칙 탐지 · 위험 점수 · 오탐 · 미탐 조정
  - [자동 대응(SOAR)](https://github.com/mdkk0220/security-agent-toolkit/tree/main/soar_response_5): 플레이북 · 승인 게이트 · 인시던트 상태 전이 (진행 중)
- `Python` `Flask` `Gemini API` `requests`

### 🧭 [AI-agent](https://github.com/mdkk0220/AI-agent)
**채용 공고 수집 · 분석 자동화 에이전트 (진행 중)**
채용 공고를 매일 수집해 기술 스택 기준으로 점수를 매기고, 문서 초안을 만든 뒤 팩트체크와 사람 승인을 거치는 LangGraph 파이프라인입니다.
- 흐름: 공고 수집 → 분석 · 맞춤 점수 → 초안 생성 → 팩트체크 → 사람 승인
- 근거 없는 문장은 팩트체크 단계에서 지우고, 승인 후에도 외부로 보내지 않고 저장만 합니다
- `Python` `LangGraph` `Streamlit` `SQLite` `REST API`

### 🦵 [knee-oa-classifier](https://github.com/mdkk0220/knee-oa-classifier)
**무릎 X-ray 관절염 등급 분류 (5인 팀 프로젝트)**
ResNet50으로 Kellgren–Lawrence 0~4등급을 분류하고, Grad-CAM으로 모델이 본 부위를 시각화했습니다.
- 담당: 저장소 구조 설계 · Git 관리 · ResNet50 모델 구현
- 테스트 결과: 정확도 0.72 · Macro-F1 0.73 · QWK 0.85 (테스트 이미지 3,052장)
- `Python` `PyTorch` `OpenCV` `Grad-CAM` `Gradio`

### 🤝 그 외 프로젝트

**BodySync** · 4인 팀 · 2026.05 ~ 06
BMI · 기초대사량을 계산하고 식단과 운동을 안내하는 Android 앱입니다.
- 담당: 앱 구조 설계 주도, 식단 탭 · 운동 탭 기능 구현, Gemini API 연동
- `Kotlin` `Jetpack Compose` `Gemini API`

**[SHydent](https://github.com/mdkk0220/Shydent)** · 6인 팀 · 2025.03 ~ 06
수업 중 학생이 교수에게 익명으로 질문하고, 교수용 앱 화면 위에 질문을 오버레이로 띄우는 시스템입니다.
- 담당: 학생용 앱 설계, GitHub 데이터 관리, 웹 · 앱 통합
- `Electron` `Vite` `Firebase`

**[SK-ALEPH](https://github.com/mdkk0220/SK-ALEPH)** · 개인 · 2026.09 ~ 10
SK ALEPH 부트캠프 웹 실습 5개 모음입니다. 정적 페이지부터 React 앱까지 만들고, 마지막에는 앱의 저장 버그를 고치는 과정을 검사 수치로 기록했습니다 (6/10 → 10/10).
- 다섯 개 모두 Vercel에 배포
- `HTML` `JavaScript` `React` `Vite` `Playwright`

---

## 🛠️ 기술 스택

**인프라 · 도구**
![Rocky Linux](https://img.shields.io/badge/Rocky_Linux-10B981?style=flat-square&logo=rockylinux&logoColor=white)
![VirtualBox](https://img.shields.io/badge/VirtualBox-183A61?style=flat-square&logo=virtualbox&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

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
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Electron](https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
