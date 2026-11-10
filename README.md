# 성명규

서버와 네트워크를 직접 구축하고, 반복되는 작업을 코드로 자동화하는 실습과 프로젝트를 해 왔습니다.
지금은 망분리 · 가상화 솔루션 회사 브이엠솔루션 입사를 앞두고 Rocky Linux 기반 이중화 환경을 실습하며 기록하고 있습니다.

## 지금 하고 있는 것

**[VMS-hw](https://github.com/mdkk0220/VMS-hw)** · 가상화 환경 인프라 실습 (진행 중)

VirtualBox에 Rocky Linux 9.8 · 8.10 서버를 구축하고, 네트워크 이중화부터 WEB · DB 이중화, 백업 자동화까지 단계별로 진행하고 있습니다.

- 서버 두 대에 active-backup bond를 두 개씩 구성하고, 랜선을 하나 끊어도 ping 손실 1~2개로 넘어가는 것을 확인했습니다
- 실습 중 겪은 장애와 일부러 낸 장애를 증상 · 원인 · 조치 · 재발 방지 순서로 기록합니다
- Rocky Linux, VirtualBox, nmcli, Bonding, Shell Script

## 프로젝트

**[AI-agent](https://github.com/mdkk0220/AI-agent)** · 채용 공고 기반 취업 준비 에이전트 (진행 중)

채용 공고를 매일 모으고, 내 기술과 맞는 공고를 골라 주고, 자소서 초안까지 써 주는 에이전트입니다.

- 공고 수집, 분석과 맞춤 점수, 자소서 초안, 팩트체크, 사람 승인 순서로 흐릅니다
- 프로필에 없는 경험을 지어낸 문장은 팩트체크 단계에서 지우고, 승인 후에도 제출하지 않고 저장만 합니다
- Python, LangGraph, Streamlit, SQLite, REST API

**[security-agent-toolkit](https://github.com/mdkk0220/security-agent-toolkit)** · 보안 관제 자동화 에이전트 (SK ALEPH 실습)

로그 수집, 정규화, 룰 탐지, LLM 요약과 판단, 사람 승인, 보고서와 알림까지 보안 관제의 한 사이클을 파이썬으로 구현했습니다. 기본 코드는 교육과정에서 제공받았습니다.

- LLM은 선택만 하고, 실행은 코드가 하고, 되돌리기 어려운 결정은 사람이 하도록 나눴습니다
- 계정 잠금처럼 위험한 조치는 승인 게이트를 거치고, 승인이 없으면 실행하지 않고 기록만 남깁니다
- Python, Flask, Gemini API

**[knee-oa-classifier](https://github.com/mdkk0220/knee-oa-classifier)** · 무릎 X-ray 관절염 등급 분류 (5인 팀)

ResNet50으로 Kellgren–Lawrence 0~4등급을 분류하고, Grad-CAM으로 모델이 본 부위를 시각화했습니다.

- 저장소 구조 설계, Git 관리, ResNet50 모델 구현을 맡았습니다
- 테스트 이미지 3,052장 기준 정확도 0.72, Macro-F1 0.73, QWK 0.85
- Python, PyTorch, OpenCV, Grad-CAM, Gradio

**[SK-ALEPH](https://github.com/mdkk0220/SK-ALEPH)** · 부트캠프 웹 실습 5개

자기소개 페이지, 브라우저 게임, React 팬카드 편집기, 환율 정보판을 만들었고, 마지막에는 팬카드 앱의 저장 버그를 두 AI 작업자가 이어서 고치는 과정을 검사 수치로 기록했습니다 (검사 6/10 → 10/10). 다섯 개 모두 Vercel에 배포되어 있습니다.

- HTML, JavaScript, React, Vite, Playwright, Vercel

**그 외 팀 프로젝트**

- BodySync (4인, 2026.05 ~ 06): BMI와 기초대사량을 계산하고 식단과 운동을 안내하는 Android 앱. 앱 구조 설계를 주도하고 식단 · 운동 탭과 Gemini API 연동을 구현했습니다. Kotlin, Jetpack Compose
- [SHydent](https://github.com/mdkk0220/Shydent) (6인, 2025.03 ~ 06): 수업 중 학생이 교수에게 익명으로 질문하고, 교수용 앱 화면 위에 질문을 오버레이로 띄우는 시스템. 학생용 앱 설계, GitHub 데이터 관리, 웹 · 앱 통합을 맡았습니다. Electron, Vite, Firebase

## 공부 기록

- 네트워크 · 보안: OSI 7계층, Wireshark 패킷 분석, 서브넷 설계, VLAN, DNS, VPN, 방화벽, 제로트러스트 ([기록](https://github.com/mdkk0220/security-agent-toolkit/tree/main/network_zt_2))
- 접근 제어: RBAC, 예외 권한, 권한 점검과 회수 ([실습](https://github.com/mdkk0220/security-agent-toolkit/tree/main/access_control_3))
- 이상 탐지: 로그 정규화, 규칙 탐지, 위험 점수, 오탐 · 미탐 조정 ([실습](https://github.com/mdkk0220/security-agent-toolkit/tree/main/anomaly_detection_4))
- 자동 대응(SOAR): 플레이북, 승인 게이트, 인시던트 상태 전이, 감사 기록 ([실습](https://github.com/mdkk0220/security-agent-toolkit/tree/main/soar_response_5), 진행 중)

## 다루는 기술

| 분야 | 기술 |
| --- | --- |
| 인프라 | Rocky Linux, VirtualBox, Docker, Git, Shell Script |
| 언어 | Python, JavaScript, Kotlin |
| 웹 · 앱 | React, Vite, Flask, Streamlit, Electron, Firebase, Vercel |
| AI | LangGraph, PyTorch, OpenCV, Gemini API |
| 네트워크 · 데이터 | Wireshark, SQLite |

## 연락처

audrby2000@gmail.com
