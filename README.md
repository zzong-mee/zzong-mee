<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&amp;color=0:102A43,50:176B9A,100:23B5A5&amp;height=180&amp;section=header&amp;text=ZZONG-MEE&amp;fontSize=44&amp;fontColor=ffffff&amp;animation=fadeIn&amp;fontAlignY=37&amp;desc=Software%20Developer%20%7C%20Systems%20and%20Simulation&amp;descAlignY=59&amp;descSize=16" width="100%" alt="Profile banner" />

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

<img src="https://skillicons.dev/icons?i=cpp,python,kotlin,js&amp;theme=dark" alt="C++, Python, Kotlin, JavaScript" />

**Development Tools**

<img src="https://skillicons.dev/icons?i=git,github,linux,androidstudio&amp;theme=dark" alt="Git, GitHub, Linux, Android Studio" />

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

### 📄 [CVaR-RAMPR — Risk-Aware Redundant MPR Selection for Reliable OLSR Routing in FANETs](https://github.com/zzong-mee/CVaR-RAMPR)

**FANET 환경의 OLSR 라우팅 신뢰성 연구 · 논문 실험 재현 · 공개 저장소**

고속 이동 UAV 네트워크의 불안정한 링크에 대응하기 위해 **LET(Link Expiration Time), CVaR, 히스테리시스**를 활용한 위험 인지 중복 MPR 선택 방식을 연구했습니다.

- **구현:** ns-3의 OLSR 기반 표준 MPR, 고정 중복, LET 기반 중복, CVaR·히스테리시스 제안 방식 등 4개 모드 비교
- **실험 설계:** UAV 30대, 3D Gauss-Markov 이동, 속도 5~25 m/s, 4개 모드 × 5개 속도 × 10개 시드 = **200개 실험 구성**
- **분석:** Python을 활용한 PDR, 종단 간 지연, 제어 오버헤드 분석 및 실험 결과 비교
- **재현 검증:** 대표 조건에서 4개 모드의 기존 결과를 재현하고, 기존 200회 실험 데이터 분석 결과 확인

| 15 m/s · 기존 실험 데이터 | 평균 PDR |
|:---|---:|
| Standard OLSR | 67.49% |
| Proposed Method | 72.59% |
| **관찰된 차이** | **+5.10%p** |

**Stack:** `C++` · `Python` · `ns-3` · `OLSR` · `LET` · `CVaR`

**Repository:** [CVaR-RAMPR](https://github.com/zzong-mee/CVaR-RAMPR) (Public) · `main`: 논문 실험 재현 / `development`: 후속 연구

### 🚁 [APUR-OLSR — Risk-Aware and Predictive OLSR Routing for FANETs](https://github.com/zzong-mee/APUR-OLSR)

**예측 기반 FANET 라우팅 프로토콜 후속 연구 · 비공개 저장소 · 설계 단계**

기존 OLSR의 MPR 선택을 확장하여 **이동성 예측과 링크 위험 추정**을 라우팅 제어 및 경로 계산에 반영하는 APUR-OLSR 프로토콜을 설계하고 있습니다. 현재 명세는 **V1.4.3**입니다.

- **링크 예측 설계:** HELLO 기반 위치·속도 관측, 등속도 이동 예측, 불확실성 추적, 3D LET 및 링크 위험 점수
- **라우팅 설계:** 2-hop 커버리지를 고려한 위험 인지 중복 MPR 선택과 적응형 TC 제어
- **경로 계산 설계:** TC 토폴로지에 연계된 AP-METRIC 교환, 방향성 가중 그래프 및 Dijkstra 탐색
- **검증 계획:** ns-3.48 환경에서 PDR, 지연, 제어 오버헤드, 경로 안정성 비교 평가

**현재 상태:** 연구 저장소와 기준 실험 소스가 준비되어 있으며, 독립 HELLO 메시지 코덱 테스트 이력이 있습니다. APUR-OLSR의 **통합 ns-3 구현과 성능 비교는 아직 검증되지 않았습니다.**

**Stack:** `C++` · `ns-3.48` · `Ubuntu/WSL` · `OLSR` · `MPR` · `LET`

**Repository:** [APUR-OLSR](https://github.com/zzong-mee/APUR-OLSR) (Private · 외부 열람 제한)

---

## 🚀 Featured Projects

### 👁️ [Third Eye](https://github.com/zzong-mee/PBL1)

**외부 카메라·거리 센서 기반 Android 보행 보조 시스템 연구** · 팀 프로젝트 · 공개 저장소 · 기능 개발 및 통합 테스트

USB 카메라의 객체 인식 결과와 좌·우 ToF 센서의 거리 데이터를 Android 앱에서 처리하고, 시각·청각적으로 표현하는 프로젝트입니다.

**팀 프로젝트 구현 범위**
- **영상 인식:** XIAO ESP32-S3 Sense의 USB JPEG 입력, YOLOX-Nano·ONNX Runtime 기반 객체 인식, 한국어 TTS 안내
- **센서 처리:** 듀얼 VL53L8CX의 8×8 거리 데이터 수신, 유효성·신선도 검사, 히트맵 표시
- **음향 실험:** 거리 단음, 방향 투영 기반 공간 음향, 좌→우 레이더 청각 스캔
- **진단 기능:** 개발자 화면에서 USB·센서·추론·음향 상태 모니터링, 접근 속도 기반 자동 경고 실험 코드

**기술 역량:** `Kotlin` · `Android` · `USB` · `ONNX Runtime` · `YOLOX-Nano` · `ToF`

**검증 및 한계:** 위 항목은 **팀 전체의 구현 범위**이며 개인별 기여를 구분해 주장하지 않습니다. 객체 인식과 거리 센서 처리 경로의 완전한 통합, 자동 경고의 실기기 검증 및 실제 보행 안전성 검증은 완료되지 않았습니다.

---

### 🎙️ [AI Voice Interview](https://github.com/kth-0121/interview-agents)

**로컬 AI 기반 음성 모의 면접 웹 서비스** · 팀 프로젝트 · 프론트엔드 및 UI/UX 담당 · 개발 중

실제 면접 상황에 가까운 화면과 사용자 흐름을 목표로 한 웹 서비스 팀 프로젝트입니다.

**담당 역할**
- **UI/UX 설계:** Figma를 이용한 면접 화면 구성과 사용자 흐름 설계
- **프론트엔드 구현:** HTML·CSS·JavaScript로 면접 인터페이스 개발
- **협업:** 백엔드 및 로컬 AI 기능 연동을 고려한 화면 구조 설계

**기술 역량:** `HTML` · `CSS` · `JavaScript` · `Figma`

**검증 및 한계:** 직접 담당한 프론트엔드·UI/UX 작업을 중심으로 소개합니다. 전체 음성 면접 파이프라인의 통합 완료나 실제 서비스 운영은 주장하지 않습니다.

---

### 🤖 [Hawawa Dosiyo](https://github.com/zzong-mee/hawawa-dosiyo)

**Discord 서버 운영 자동화 및 커뮤니티 봇** · 개인 개발 · 공개 저장소 · 개발 중

서버별 설정과 운영 작업을 관리하는 Python 봇입니다. 단순 명령어 구현뿐 아니라 **기능 분리, 데이터 영속성, 재시작 복구, 자동 테스트**를 고려해 개발하고 있습니다.

**주요 구현**
- **모듈형 구조:** discord.py Cog 기반으로 역할·관리·예약·커뮤니티 기능을 분리하고, 슬래시 명령어와 옵션을 한국어로 표시
- **데이터 관리:** SQLite에 서버별 설정과 기록을 분리 저장하고, 재시작 후 리마인더·기간 역할·추첨 마감·버튼 역할 패널 복구
- **운영 자동화:** 자동·지연 역할, 재입장 역할 복원, 건의 승인/반려, 경고 기록, Discord AutoMod 연계, 가상 주식 기능
- **품질 관리:** 모의 Discord 객체와 임시 DB 기반 `unittest`, GitHub Actions CI 구성

**기술 역량:** `Python 3.13` · `discord.py 2.x` · `SQLite` · `unittest` · `GitHub Actions`

**검증 및 한계:** 오프라인 단위 테스트를 수행하지만 실제 Discord 서버의 모든 기능과 재시작 상황을 검증한 것은 아닙니다. DB 하나당 단일 봇 프로세스를 전제로 하며 일부 예약 작업은 강제 종료 시 중복 처리 가능성이 있습니다.

---

## 📂 Other Experiences

| Project | Experience |
|:---|:---|
| ⚔️ [Elden Ring Presets](https://github.com/zzong-mee/elden-ring-presets) | **Public** · Python·C++ 기반 Windows 오프라인 장비 프리셋 테스트 앱. 장비 데이터 읽기·저장 및 일부 단축키 검증, 실게임 복원·게임패드 검증 진행 과제 |
| 💬 dosiyo-bot / takoyaki | 기존 Discord 봇 개인 개발 경험 · **Private / Archived** |
| ⛏️ Minecraft Dashboard | Python 대시보드 개인 프로젝트 · **Private** |
| 📱 Flutter Practice | Dart·Flutter 학습 프로젝트 · **Private** |

---

## 📊 GitHub Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=zzong-mee&amp;show_icons=true&amp;theme=tokyonight&amp;hide_border=true" height="165" alt="GitHub statistics" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=zzong-mee&amp;layout=compact&amp;theme=tokyonight&amp;hide_border=true" height="165" alt="Top languages" />

<img src="https://raw.githubusercontent.com/zzong-mee/zzong-mee/output/github-contribution-grid-snake.svg" width="100%" alt="Contribution snake animation" />

</div>

<sub>GitHub 통계는 공개 저장소 기준이며 비공개 연구와 팀 프로젝트 경험을 모두 반영하지 않을 수 있습니다.</sub>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&amp;color=0:102A43,50:176B9A,100:23B5A5&amp;height=110&amp;section=footer" width="100%" alt="Footer wave" />

**Design · Implement · Verify · Improve**

</div>
