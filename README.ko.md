# Open Software Defined Building (Open SDB)

> **"차세대 빌딩 운영 시스템(OS)을 정의하다."**
> 
> 정적인 디지털 트윈을 넘어, 스스로 판단하고 제어하는 **Physical AI**를 향해.
> 각 분야에서 발전해 온 전문 기술을 통합하여 Software Defined Building(SDB) 아키텍처를 연구합니다.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status: Research](https://img.shields.io/badge/Status-Research_&_Prototyping-blue.svg)](https://github.com/mossland/open-sdb)

## 📖 소개 (Introduction)
**Open Software Defined Building (Open SDB)**은 **Mossland**가 주도하는 오픈소스 리서치 프로젝트입니다. 우리는 지능형 소프트웨어 아키텍처가 건물 운영의 핵심이 되는 **Software Defined Building (SDB)** 의 기반을 연구하고 구축하고자 합니다.

스마트 빌딩의 궁극적인 목표는 단순한 관제(Monitoring)가 아닌, AI가 현실 세계를 지능적으로 제어하는 **Physical AI**의 실현입니다. 이를 위해 우리는 설계, 시공, 시뮬레이션 각 분야에서 깊이 있게 발전해 온 소프트웨어 생태계를 하나의 유기적인 제어 루프로 통합하는 방법을 연구합니다.

## 🔭 비전 및 미션 (Vision & Mission)

### Vision
**통합을 통한 자율 운영 빌딩(Autonomous Building)의 실현**
건축 산업의 다양한 기술 요소들이 서로 단절되지 않고 융합되는 환경을 조성하여, 건물이 스스로 인지하고 판단하며 행동하는 자율 운영 환경을 구현합니다.

### Mission
**전문가 영역의 유기적 통합과 폐쇄 루프(Closed-Loop) 구축**
CAD, BIM, BEM(에너지 모델링) 등 각 영역에서 고도화된 레거시 시스템들을 연결합니다. 설계 데이터와 시뮬레이션 결과, 그리고 실제 운영 제어가 실시간으로 상호작용하는 **폐쇄 루프 제어 시스템(Closed-Loop Control System)** 을 완성하는 것이 우리의 미션입니다.

## 🧩 과제: 전문화된 영역의 연결 (The Challenge)

AEC(건축, 엔지니어링, 건설) 산업은 각 도메인별로 눈부신 기술 발전을 이뤘습니다. 하지만 고도로 전문화된 소프트웨어들은 종종 독립적으로 작동합니다.

* **설계(CAD):** 정밀한 건축 도면 작성을 위한 표준.
* **구축(BIM):** 건물의 상세 정보와 기하학적 데이터를 담은 저장소.
* **시뮬레이션(BEM):** 에너지 흐름과 물리적 현상을 해석하는 고도화된 도구.
* **운영(BMS):** 건물의 설비와 기능을 관리하는 시스템.

각 분야는 이미 훌륭한 완성도를 갖추고 있지만, 이들 사이의 실시간 통합 부재는 운영 데이터가 즉시 시뮬레이션과 제어에 반영되는 진정한 의미의 **폐쇄 루프(Closed-Loop)** 구현을 어렵게 만들고 있습니다.

## 💡 해결책: SDB (Software Defined Building)

우리는 **SDB**를 통해 이들을 통합하는 아키텍처를 제안합니다. 기존 기술을 대체하는 것이 아니라, 레거시 시스템들의 가치를 Physical AI 관점에서 엮어내는 새로운 소프트웨어 계층을 연구합니다:

1.  **Seamless Integration:** BIM 및 시뮬레이션 툴의 데이터를 수작업 변환이나 데이터 손실 없이 직접 파싱하고 활용하는 방법 연구.
2.  **Real-time Interoperability:** 정적인 모델(BIM)과 동적인 엔진(시뮬레이션/제어) 간의 실시간 데이터 흐름 구현.
3.  **Physical AI & Closed-Loop:** 검증된 기존 도메인 소프트웨어들의 역량을 결합하여, AI가 계획(시뮬레이션), 행동(제어), 관찰(센서)하는 순환 구조 완성.

## 📂 리포지토리 구조

이 리포지토리는 SDB 구현을 위한 **리서치 문서**와 **PoC(개념 증명) 코드**를 모두 포함합니다.

```bash
open-sdb/
├── docs/               # 리서치 페이퍼 및 아키텍처 설계 문서
│   ├── integration/    # IFC, IDF, gbXML 등 이기종 포맷 통합 전략
│   ├── architecture/   # SDB 코어 아키텍처 정의
│   └── vision/         # Physical AI와 시스템 통합 철학
├── src/                # 실험적 코드 및 프로토타입
│   ├── adapters/       # 다양한 레거시 포맷 연동을 위한 어댑터 모듈
│   ├── core/           # 데이터 흐름을 관장하는 SDB 오케스트레이션 엔진
│   └── agent/          # 폐쇄 루프 제어를 수행하는 AI 에이전트 프로토타입
└── README.ko.md

```

## 🚀 로드맵 (Roadmap)

* [ ] **Phase 1: Research & Analysis** - 레거시 포맷 분석 및 통합 프로토콜 정의
* [ ] **Phase 2: Core Prototyping** - BIM 데이터와 시뮬레이션 엔진을 연결하는 SDB Core 개발
* [ ] **Phase 3: AI Orchestration** - 통합된 시스템 위에서 폐쇄 루프를 제어하는 Physical AI 구현

## 🤝 기여하기 (Contribution)

이 프로젝트는 건축 기술의 새로운 가능성을 탐구합니다. 우리는 **"Vibe Coding"**의 정신으로 AI와 멀티 에이전트 기술을 적극 활용하여 연구를 가속화하고 있습니다. 다양한 분야의 전문 기술을 하나의 지능형 시스템으로 통합하는 데 열정을 가진 아키텍트, 엔지니어, 개발자분들의 참여를 환영합니다.

## 📜 라이선스 (License)

이 프로젝트는 MIT 라이선스를 따릅니다. 자세한 내용은 [LICENSE](https://www.google.com/search?q=LICENSE) 파일을 참고하세요.
