<h1 align="center">안녕하세요, 성명규입니다 👋</h1>
<h3 align="center">보안 자동화와 웹 개발을 공부하는 개발자</h3>

<p align="center">
  로그를 읽고, 위험을 판단하고, 사람이 결정할 수 있게 돕는 도구를 만듭니다.
</p>

---

## 🔭 대표 프로젝트

### 🛡️ [security-agent-toolkit](https://github.com/mdkk0220/security-agent-toolkit)
**보안 관제 자동화 에이전트**
로그 수집 → 정규화 → 룰 탐지 → LLM 요약 · 판단 → 사람 승인 → 보고서 · 알림까지, 보안 관제의 한 사이클을 파이썬으로 구현했습니다.
- 핵심 원칙: **LLM은 고르기만 하고, 실행은 코드가 하고, 되돌리기 어려운 결정은 사람이 한다**
- 계정 잠금 같은 위험한 조치는 승인 게이트를 거치고, 승인이 없으면 실행하지 않고 기록만 남깁니다
- `Python` `Flask` `Gemini API` `requests`

### 🦵 [knee-oa-classifier](https://github.com/mdkk0220/knee-oa-classifier)
**무릎 X-ray 관절염 등급 분류 (5인 팀 프로젝트)**
ResNet50 전이학습으로 Kellgren–Lawrence 0~4등급을 분류하고, Grad-CAM으로 모델이 본 부위를 시각화했습니다.
- 담당: 저장소 구조 설계 · Git 관리 · ResNet50 모델 구현
- 테스트 결과: 정확도 0.72 · Macro-F1 0.73 · QWK 0.85 (테스트 이미지 3,052장)
- `Python` `PyTorch` `OpenCV` `Grad-CAM` `Gradio`

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
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

**프레임워크 · 라이브러리**
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)

**도구 · 인프라**
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
