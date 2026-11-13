
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:102A43,45:176B9A,100:23B5A5&height=190&section=header&text=ZZONG-MEE&fontSize=46&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Software%20Development%20%7C%20Systems%20%7C%20Research&descAlignY=58&descSize=16" width="100%" alt="Profile banner" />

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1100&color=37B6CF&center=true&vCenter=true&width=680&lines=Software+Developer;Python+%7C+Kotlin+%7C+C%2B%2B+%7C+JavaScript;Network+Simulation+%26+Software+Engineering;Design+%7C+Implementation+%7C+Verification" alt="Typing animation" />

### Software Developer

**문제를 분석하고, 구현하고, 실험과 테스트를 통해 검증하는 개발자입니다.**

네트워크 시뮬레이션 · 응용 소프트웨어 · Android · 웹 개발

<img src="https://img.shields.io/badge/Software_Development-2563EB?style=flat-square" />
<img src="https://img.shields.io/badge/Problem_Solving-7C3AED?style=flat-square" />
<img src="https://img.shields.io/badge/Team_%26_Solo_Projects-0891B2?style=flat-square" />

</div>

---

## 👨‍💻 About Me

C++과 Python을 활용한 네트워크 시뮬레이션 연구를 진행하고 있으며, Python 기반 서비스 개발과 웹·Android 팀 프로젝트를 통해 설계, 구현, 테스트 경험을 쌓고 있습니다.

특히 시스템의 동작을 분석하고 실험 조건을 구성하며 결과를 정량적으로 비교하는 개발 과정에 관심이 있습니다.

### Core Competencies

| 분야 | 실제 경험 |
|:---|:---|
| **Software Development** | Python 서비스 로직, SQLite 데이터 저장, Windows 유틸리티 개발 |
| **Simulation & Analysis** | ns-3 OLSR 라우팅 실험 및 Python 결과 분석 |
| **Testing & Verification** | unittest, GitHub Actions CI, 대표 실험 재현 및 비교 |
| **System Integration** | Android 앱의 USB 데이터 처리, AI 추론 및 음성 안내 팀 개발 |
| **Frontend & UI/UX** | Figma 설계와 HTML·CSS·JavaScript 화면 구현 |

---

## 🛠️ Technical Skills

<div align="center">

**Programming Languages**

<img src="https://skillicons.dev/icons?i=cpp,python,kotlin,js,html,css,dart&theme=dark" alt="Languages" />

**Development Tools**

<img src="https://skillicons.dev/icons?i=git,github,linux,vscode,androidstudio,figma,flutter&theme=dark" alt="Tools" />

</div>

### Languages & Practical Experience

| Language | 활용 프로젝트 및 경험 |
|:---|:---|
| **C++** | ns-3 OLSR 라우팅 알고리즘 연구 및 시뮬레이션 |
| **Python** | FANET 실험 자동화, 결과 분석, Discord 봇, Windows 유틸리티 |
| **Kotlin** | Third Eye Android 팀 프로젝트 |
| **JavaScript / HTML / CSS** | AI Voice Interview 프론트엔드 구현 |
| **Dart** | Flutter 실습 |

### Technologies & Engineering Tools

| Category | Technologies |
|:---|:---|
| **Networking** | ns-3, OLSR, MPR, LET, CVaR |
| **AI / Vision** | YOLOX-Nano, ONNX Runtime |
| **Application** | Android, discord.py, SQLite |
| **Testing** | Python unittest, GitHub Actions |
| **Development** | Git, GitHub, Linux / WSL, VS Code |
| **Design** | Figma, Android XML UI |

---

## 🔬 Research & Publications

### Risk-Aware Redundant MPR Selection for Reliable OLSR Routing in Flying Ad-Hoc Networks

<img src="https://img.shields.io/badge/SOLO_RESEARCH-176B9A?style=flat-square" />
<img src="https://img.shields.io/badge/FANET-087E8B?style=flat-square" />
<img src="https://img.shields.io/badge/ns--3_Simulation-365486?style=flat-square" />

**드론 애드혹 네트워크의 안정적인 라우팅을 위한 위험 인지 기반 MPR 선택 연구**

고속으로 이동하는 드론 네트워크의 링크 단절과 토폴로지 변화에 따른 패킷 전달 성능을 분석하고, 위험도를 고려한 중복 MPR 선택 방식을 연구했습니다.

**Research & Implementation**

- ns-3 기반 OLSR 라우팅 시뮬레이션 구성
- 표준 OLSR, 고정 중복, LET 기반 중복 및 CVaR 기반 제안 방식 비교
- Link Expiration Time(LET) 및 히스테리시스 제어 연구
- Python 기반 실험 자동화와 PDR·지연·제어 오버헤드 분석

**Experiment Design**

| Parameter | Configuration |
|:---|:---|
| UAV Nodes | 30 |
| Mobility | 3D Gauss-Markov |
| UAV Speed | 5, 10, 15, 20, 25 m/s |
| Algorithms / Seeds | 4 modes / 10 seeds |
| Experiment Matrix | 200 configurations |

**Research Results — Historical Dataset**

15 m/s 조건에서 제안 방식의 평균 PDR은 **72.59%**, 표준 OLSR은 **67.49%**로, 관찰된 차이는 **+5.10%p**였습니다.

다만 대응 비교의 95% 신뢰구간은 **−4.42~+14.63%p**로 0을 포함하므로, 통계적으로 유의한 개선으로 단정할 수 없습니다.

**Reproducibility:** 대표 조건의 4개 모드 결과 재현 및 기존 200회 데이터 분석을 검증했습니다. 전체 200회 신규 재실행 검증은 아직 완료되지 않았습니다.

**Tech Stack:** `C++` `Python` `ns-3` `OLSR` `LET` `CVaR`

> 개인 연구 · 비공개 저장소. 논문 제목은 연구 저장소에 기재된 제목이며, 학술지 게재·저자·DOI 정보는 확인 후 추가할 예정입니다.

---

## 🚀 Featured Projects

### 🤖 [Hawawa Dosiyo](https://github.com/zzong-mee/hawawa-dosiyo)

<img src="https://img.shields.io/badge/SOLO_PROJECT-7C3AED?style=flat-square" alt="개인 프로젝트" />
<img src="https://img.shields.io/badge/ACTIVE_DEVELOPMENT-F59E0B?style=flat-square" alt="활발히 개발 중" />

**Python 기반 Discord 서버 운영·커뮤니티 봇 — 모듈화, 데이터 영속성, 테스트 자동화**

기존 dosiyo-bot과 takoyaki의 개발 경험을 바탕으로, 기능별 Cog와 한국어 로컬라이즈 슬래시 명령어를 중심으로 개발하고 있습니다.

- Discord.py 2.x 기반 슬래시 명령어와 기능별 Cog 구성
- 정보 조회, 투표·게임, 메시지 관리와 공통 오류 안내
- SQLite 기반 서버별 설정·태그·경고 기록과 재시작 복구 예약 작업
- 자동 역할·기간 역할·재입장 복원, 건의·추첨·추천 게시판·레벨 보상
- 서버 멘션에만 응답하는 선택형 AI 대화 기능과 권한·Intent 설정
- Python 3.13과 unittest 기반 오프라인 테스트 및 GitHub Actions CI

**Tech Stack:** `Python 3.13` `discord.py 2.x` `SQLite` `unittest` `GitHub Actions`

> Solo Project · Public Repository · Active Development  
> 전체 Carl-bot 기능과 외부 서비스 연동을 목표로 하지 않으며, AI·멤버 이벤트 기능은 환경변수와 Discord Developer Portal Intent 설정이 필요합니다. 기존 봇과 데이터는 별도로 보존합니다.

---

### 🎙️ AI Voice Interview

<img src="https://img.shields.io/badge/TEAM_PROJECT-2563EB?style=flat-square" />
<img src="https://img.shields.io/badge/ROLE-Frontend_%26_UI%2FUX-8B5CF6?style=flat-square" />
<img src="https://img.shields.io/badge/IN_PROGRESS-F59E0B?style=flat-square" />

**로컬 AI 기반 음성 모의 면접 웹 서비스**

실제 면접과 유사한 환경에서 사용자가 AI 음성 면접을 경험할 수 있도록 개발하는 팀 프로젝트입니다.

**My Responsibilities**

- 웹 프론트엔드 개발 및 UI/UX 담당
- 실제 면접 환경을 반영한 화면 구성과 사용자 흐름 설계
- Figma 기반 인터페이스 디자인
- HTML, CSS, JavaScript 기반 웹 화면 개발
- 백엔드 및 AI 기능과의 연동을 고려한 화면 구조 구성

**Tech Stack:** `HTML` `CSS` `JavaScript` `Figma`

> Team Project · In Progress

---

### 👁️ [Third Eye](https://github.com/zzong-mee/PBL1)

**팀 프로젝트 · 공개 저장소 · 통합 테스트 단계**

시각장애인의 주변 인지와 보행을 보조하기 위한 Android 앱입니다. 팀은 USB 카메라 영상에서 YOLOX-Nano로 중앙 물체를 인식하고 한국어 TTS로 안내하는 기능과, 좌·우 ToF 센서의 거리 데이터를 히트맵과 소리로 표현하는 기능을 개발하고 있습니다.

**검증 상태:** 카메라 인식과 ToF 데이터 처리를 개발하고 있으며, 접근 속도 기반 자동 경고 실험 코드도 있습니다. 다만 센서 융합과 자동 경고의 실기기 검증 및 보행 안전성 검증은 완료되지 않았습니다.

**Tech Stack:** `Kotlin` `Android` `ONNX Runtime` `YOLOX-Nano` `USB` `ToF`

---

## 🤖 Discord Bot Development

| Project | Status | Development | Tech Stack |
|:---|:---:|:---|:---|
| 🤖 [Hawawa Dosiyo](https://github.com/zzong-mee/hawawa-dosiyo) | 공개 · 재설계 중 | 슬래시 명령어와 서버 운영 기능을 새 구조로 개발 | Python, discord.py, SQLite |
| 💬 **dosiyo-bot** | 비공개 · 보관 | 기존 Discord 봇 개발 경험 및 원본 보존 | Python, Discord |
| 🍡 **takoyaki** | 비공개 · 보관 | 기존 Discord 봇 설계·구현 및 원본 보존 | Discord |

현재 봇 개발은 **Hawawa Dosiyo**에서 진행합니다. 이전 프로젝트의 코드와 데이터는 보존하며, 데이터 이전은 별도 계획으로 진행합니다.

---

## 📂 Other Experiences

| Project | Type | Description | Tech Stack |
|:---|:---:|:---|:---|
| ⚔️ [Elden Ring Presets](https://github.com/zzong-mee/elden-ring-presets) | Solo | 오프라인 장비 프리셋 Windows 테스트 앱. 장비 읽기·저장 구현, 키보드 단축키 동작 확인. 실게임 복원과 게임패드 동작은 미검증 | Python, Windows |
| ⛏️ Minecraft Dashboard | Solo | Minecraft 대시보드 개발 | Python |
| 📱 Flutter Practice | Solo | Flutter 및 Dart 모바일 앱 개발 학습 | Flutter, Dart |

---

## 📌 Public Repositories

| Repository | Description |
|:---|:---|
| [Hawawa Dosiyo](https://github.com/zzong-mee/hawawa-dosiyo) | Python·discord.py 기반 Discord 서버 운영·커뮤니티 봇 |
| [Elden Ring Presets](https://github.com/zzong-mee/elden-ring-presets) | Windows용 오프라인 장비 프리셋 테스트 앱 |
| [Third Eye](https://github.com/zzong-mee/PBL1) | USB 카메라 객체 인식과 ToF 거리 처리를 실험하는 Android 팀 프로젝트 |

---

## 📊 GitHub Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=zzong-mee&show_icons=true&theme=tokyonight&hide_border=true" height="165" alt="GitHub statistics" />

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=zzong-mee&layout=compact&theme=tokyonight&hide_border=true" height="165" alt="Top languages" />

</div>

<sub>GitHub 통계는 공개 저장소 중심으로 표시되며 비공개 프로젝트의 개발 경험 전체를 반영하지 않을 수 있습니다.</sub>

---

## 🐍 Contribution Activity

<div align="center">

<img src="https://raw.githubusercontent.com/zzong-mee/zzong-mee/output/github-contribution-grid-snake.svg" width="100%" alt="Contribution Snake Animation" />

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:102A43,45:176B9A,100:23B5A5&height=110&section=footer" width="100%" alt="Footer wave" />

**Design · Implement · Verify · Improve**

</div>

