<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:102A43,50:176B9A,100:23B5A5&height=180&section=header&text=ZZONG-MEE&fontSize=44&fontColor=ffffff&animation=fadeIn&fontAlignY=37&desc=Software%20Developer%20%7C%20Systems%20%26%20Simulation&descAlignY=59&descSize=16" width="100%" alt="Profile banner" />

### Software Developer

**문제를 분석하고, 소프트웨어로 구현하며, 실험과 테스트로 검증합니다.**

C++ · Python · Network Simulation · Application Development

</div>

---

## 👨‍💻 About Me

네트워크 라우팅 연구부터 Python 응용 소프트웨어, Android 및 웹 팀 프로젝트까지 다양한 개발 경험을 쌓고 있습니다. 특히 **구현 과정과 검증 결과를 설명할 수 있는 개발**을 중요하게 생각합니다.

- **Simulation & Research** — ns-3 기반 FANET 라우팅 알고리즘 구현·비교, Python 실험 분석
- **Software Engineering** — Discord 봇의 모듈 설계, SQLite 데이터 저장, 예약 작업 복구 및 CI
- **Application & Integration** — Android 센서·AI 연동 팀 개발, 웹 UI/UX 설계 및 구현

## 🛠️ Technical Skills

<div align="center">

**Programming Languages**

<img src="https://skillicons.dev/icons?i=cpp,python,kotlin,js&theme=dark" alt="C++, Python, Kotlin, JavaScript" />

**Development Tools**

<img src="https://skillicons.dev/icons?i=git,github,linux,androidstudio&theme=dark" alt="Git, GitHub, Linux, Android Studio" />

</div>

| 기술 | 실제 활용 경험 |
|:---|:---|
| **C++ / ns-3** | OLSR·MPR 라우팅 알고리즘 및 FANET 시뮬레이션 |
| **Python** | 실험 자동화·결과 분석, Discord 봇, Windows 유틸리티 |
| **Kotlin / Android** | 외부 USB 카메라·ToF 센서 및 AI 추론 팀 프로젝트 |
| **JavaScript / HTML / CSS** | AI 음성 면접 서비스 프론트엔드 |
| **SQLite / unittest / CI** | 서버별 설정 저장, 자동 테스트 및 GitHub Actions |

---

## 🔬 Research

### Risk-Aware Redundant MPR Selection for Reliable OLSR Routing in Flying Ad-Hoc Networks

**FANET 라우팅 신뢰성 연구 · 개인 연구 · 비공개 저장소**

이동성이 높은 드론 네트워크에서 링크 불안정성을 고려한 **중복 MPR 선택 알고리즘**을 연구했습니다. 표준 OLSR, 고정 중복, LET 기반 방식과 CVaR·히스테리시스 기반 제안 방식을 ns-3에서 비교합니다.

- **구현:** C++ 기반 OLSR 라우팅 수정, LET·CVaR·히스테리시스 활용
- **실험:** UAV 30대, 3D Gauss-Markov 이동, 속도 5~25 m/s, 4개 알고리즘 × 5개 속도 × 10개 시드 = **200개 실험 구성**
- **분석:** Python으로 PDR, 종단 간 지연, 제어 오버헤드 및 신뢰구간 분석
- **재현:** 대표 조건의 4개 모드 결과와 기존 200회 실험 데이터 분석 검증

| 15 m/s 조건 · 기존 실험 데이터 | 평균 PDR |
|:---|---:|
| Standard OLSR | 67.49% |
| Proposed Method | 72.59% |
| **관찰된 차이** | **+5.10%p** |

> 대응 비교 95% 신뢰구간은 **−4.42~+14.63%p**로 0을 포함합니다. 따라서 이 조건에서 통계적으로 유의한 개선이 입증되었다고 단정할 수 없습니다. 전체 200개 실험의 신규 재실행 검증도 아직 완료되지 않았습니다.

**Stack:** `C++` `Python` `ns-3` `OLSR` `MPR` `LET` `CVaR`

**Paper / Publication:** 연구 저장소에 위 논문 제목과 재현 코드가 기록되어 있습니다. 학술지 게재 정보, 저자 및 DOI는 확인 후 추가할 예정입니다.

---

## 🚀 Featured Projects

### 🤖 [Hawawa Dosiyo](https://github.com/zzong-mee/hawawa-dosiyo)

**Python 기반 Discord 서버 운영·커뮤니티 봇** · Solo · Public · In Development

기존 봇 개발 경험을 바탕으로 기능별 Cog 구조, 서버별 데이터 저장, 예약 작업과 자동 테스트를 고려하여 개발하고 있습니다.

- discord.py 2.x 슬래시 명령어 및 기능별 Cog 구성
- SQLite 기반 서버별 설정·기록 저장과 재시작 후 예약 작업 복구
- 역할 관리, 투표, 리마인더, 건의·추첨 등 커뮤니티 기능
- unittest 기반 오프라인 테스트와 GitHub Actions CI

**Stack:** `Python 3.13` `discord.py` `SQLite` `unittest` `GitHub Actions`

> 기능은 단계적으로 개발 중이며, Discord 권한·Intent 설정과 실제 서비스 환경에 따라 동작 범위가 달라질 수 있습니다.

### 👁️ [Third Eye](https://github.com/zzong-mee/PBL1)

**AI 기반 보행 보조 Android 애플리케이션** · Team · Public · Integration Testing

외부 USB 카메라와 ToF 거리 센서의 데이터를 Android 앱에서 처리하고, 객체 인식과 음향 안내를 실험하는 팀 프로젝트입니다.

- USB JPEG 입력, YOLOX-Nano·ONNX Runtime 기반 객체 인식
- 좌·우 VL53L8CX 센서의 8×8 거리 데이터 처리 및 히트맵
- 한국어 TTS, 방향 음향 및 레이더 청각 스캔 실험
- 개발자 화면의 센서 상태 및 처리 단계 모니터링

**Stack:** `Kotlin` `Android` `USB` `ONNX Runtime` `YOLOX-Nano` `ToF`

> 위 항목은 **팀 프로젝트 전체의 구현 범위**입니다. 자동 접근 경고 관련 실험 코드가 있지만 센서 융합과 보행 안전성은 실기기 검증이 완료되지 않았습니다.

### 🎙️ [AI Voice Interview](https://github.com/kth-0121/interview-agents)

**로컬 AI 기반 음성 모의 면접 서비스** · Team · Frontend & UI/UX · In Progress

실제 면접 환경을 고려한 웹 인터페이스를 설계하고 구현하는 팀 프로젝트입니다.

**My Role**
- Figma 기반 면접 화면과 사용자 흐름 설계
- HTML·CSS·JavaScript 프론트엔드 구현
- 백엔드·AI 연동을 고려한 화면 구성

**Stack:** `HTML` `CSS` `JavaScript` `Figma`

> 전체 음성 면접 시스템의 완성 및 통합 검증을 의미하지 않습니다.

---

## 📂 Other Experiences

| Project | Experience |
|:---|:---|
| ⚔️ [Elden Ring Presets](https://github.com/zzong-mee/elden-ring-presets) | Python·C++ 기반 Windows 오프라인 장비 프리셋 테스트 앱. 장비 데이터 읽기·저장 및 일부 단축키 검증, 실게임 복원·게임패드 검증 진행 과제 |
| 💬 dosiyo-bot / takoyaki | 기존 Discord 봇 개인 개발 경험 · 비공개 보관 |
| ⛏️ Minecraft Dashboard | Python 대시보드 개인 프로젝트 · 비공개 |
| 📱 Flutter Practice | Dart·Flutter 학습 프로젝트 · 비공개 |

---

## 📊 GitHub Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=zzong-mee&show_icons=true&theme=tokyonight&hide_border=true" height="165" alt="GitHub statistics" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=zzong-mee&layout=compact&theme=tokyonight&hide_border=true" height="165" alt="Top languages" />

<img src="https://raw.githubusercontent.com/zzong-mee/zzong-mee/output/github-contribution-grid-snake.svg" width="100%" alt="Contribution snake animation" />

</div>

<sub>GitHub 통계는 공개 저장소 기준이며 비공개 연구와 팀 프로젝트 경험을 모두 반영하지 않을 수 있습니다.</sub>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:102A43,50:176B9A,100:23B5A5&height=110&section=footer" width="100%" alt="Footer wave" />

**Design · Implement · Verify · Improve**

</div>
