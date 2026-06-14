---
layout: page
title: Projects
icon: fas fa-code
order: 2
---

## 🧠 MemoryLink

> *기억을 잇다, 오늘을 기록하다*  
> **초기 치매·경도인지장애(MCI) 예방을 위한 종합 인지 건강 관리 앱**

| 항목 | 내용 |
|------|------|
| **역할** | Flutter 앱 개발 (캡스톤 디자인 프로젝트) |
| **기간** | 2026 |
| **기술 스택** | Flutter, Dart, Provider, Firebase, Gemini AI, SQLite |
| **플랫폼** | Android, iOS |
| **GitHub** | [저장소 보기](https://github.com/Logic-k) |

---

### 📱 주요 기능

| 기능 | 설명 |
|------|------|
| 🧠 **인지 훈련 게임** | 7종 게임 · 적응형 난이도 1~10단계 |
| 🚶 **보행 분석** | 스마트폰 센서 기반 CV(변동성 계수) 분석 |
| 🤖 **AI 회상 대화** | Google Gemini 기반 회상 요법 챗봇 |
| 📔 **감정 일기** | 달력 기반 Memory Garden 일기 |
| 📊 **주간 리포트** | 4개 인지 영역 점수 추이 · PDF 생성 |
| 👨‍👩‍👧 **보호자 연계** | QR 코드 연결 · 실시간 웹 대시보드 |

---

### 🎮 인지 훈련 게임 7종

1. **비교 게임** — 숫자/도형 크기 비교
2. **수열 게임** — 숫자 패턴 찾기
3. **도형 스도쿠** — 4×4 도형 스도쿠
4. **구구단 게임** — 구구단 퀴즈
5. **단어 분류** — 카테고리별 단어 분류
6. **도형 짝 맞추기** — 기억력 게임
7. **문장 읽기** — 문장 이해력 평가

모든 게임은 **3회 연속 정답 시 레벨업, 2회 연속 오답 시 레벨다운** 방식의 **적응형 난이도**를 적용했습니다.

---

### 🏗 아키텍처 하이라이트

```
📱 Flutter App
├── UI Layer (30+ 화면)
├── Provider State Management
├── Core Services
│   ├── SQLite (로컬 DB — 오프라인 우선)
│   ├── Firebase (클라우드 동기화)
│   └── Gemini AI (회상 대화)
└── Device Sensors
    ├── Accelerometer (보행 분석)
    ├── Microphone + STT (음성 평가)
    └── Pedometer (걸음 수)
```

- **로컬 우선(Local-First)** 전략: 모든 데이터를 SQLite에 먼저 저장하고, 네트워크 연결 시 Firestore에 동기화
- **적응형 난이도 알고리즘**: 사용자의 퍼포먼스를 실시간으로 분석해 난이도 자동 조절
- **보행 변동성(CV) 분석**: 스마트폰 가속도계로 걸음 간격의 불규칙성을 정량화

---

### 📸 스크린샷

| 홈 화면 | AI 챗봇 | 감정 일기 |
|:-------:|:--------:|:---------:|
| ![홈](/assets/img/memorylink_home.png) | ![AI](/assets/img/memorylink_ai.png) | ![일기](/assets/img/memorylink_diary.png) |

| 훈련 허브 | 보행 분석 | 주간 리포트 |
|:---------:|:---------:|:----------:|
| ![훈련](/assets/img/memorylink_training.png) | ![보행](/assets/img/memorylink_gait.png) | ![리포트](/assets/img/memorylink_report.png) |

---

### 📊 프로젝트 규모

| 항목 | 수치 |
|:----:|:----:|
| 📐 화면 수 | **30+** |
| 🎮 인지 훈련 게임 | **7종** |
| 📈 인지 평가 영역 | **4개** (계산·논리·기억·집중) |
| 🎯 적응형 난이도 | **10단계** |
| 🧪 자동화 테스트 | **단위 63 · 위젯 36 · 통합 5 · Maestro 19** |
| 📋 PDF 리포트 | **4페이지** |

---

## 다른 프로젝트

(추후 추가 예정)
