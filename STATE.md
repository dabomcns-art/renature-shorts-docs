# 리네이처 제올라이트 숏폼 프로젝트 — 현재 상태 (STATE.md)

> **최종 업데이트**: 2026년 4월 22일  
> **관리 주체**: Claude (총괄) + ChatGPT (시각자산) + 설계봇 (Kling 프롬프트)  
> **저장소**: https://github.com/dabomcns-art/renature-shorts-docs

---

## 🚨 팀원 필독 (대화 시작 시 반드시 확인)

이 문서는 리네이처 숏폼 프로젝트의 **단일 진실 소스**입니다.  
Claude, ChatGPT, 설계봇 중 어느 팀원이든 새 대화를 시작할 때 이 문서를 먼저 읽고 맥락을 복원하세요.

### 가장 최근 핵심 결정사항 (2026-04-22 기준)
1. **팀 운영 체계 확정**: ChatGPT=시각자산, 설계봇=Kling프롬프트, Claude=서사·총괄
2. **Solve 컷 금지 표현 확정**: `absorbed into the body`, `into the crystal pores` 등 사용 금지
3. **시작 프레임 신규 원칙**: 이전 씬 마지막 프레임 직접 사용은 환경+캐릭터 identity 둘 다 유지될 때만
4. **제올라이트 색상 이원화**: 본체 pale mint green / 스킬 발동 시 pastel mint-cyan aurora
5. **Solve 컷 2샷 분리 권장**: 인지샷 + 정화샷으로 나눠 각각 Multi-shot OFF로 생성

---

## 📋 현재 진행 상태

| 항목 | 값 |
|---|---|
| 제작 중인 편 | **4편 (반려동물·암모니아)** |
| 현재 씬 | **씬 6 — Solve (2샷 분리 구조 재제작 중)** |
| 직전 작업 | 씬 6 4차 재생성 실패 → 2샷 분리 구조 전환 결정 |
| 다음 단계 | 씬 6 시작 스틸 신규 제작 (ChatGPT 주관) → Shot 1 → Shot 2 |
| 그 다음 | 씬 7 (Reaction/승리) → 4편 완주 → 1편 제작 시작 |

---

## 🎬 4편 씬별 진행 상태

| 씬 | 역할 | 상태 | 비고 |
|---|---|---|---|
| 씬 1 | Problem (거실 배경) | ✅ 완료 | |
| 씬 2 | Problem (방향제 스프레이) | ✅ 완료 | |
| 씬 3 | Villain entrance (암모니아 등장) | ✅ 완료 | 재수정 완료 |
| 씬 4 | Villain rampage (암모니아 활보) | ✅ 완료 | |
| 씬 5 | Hero entrance (제올라이트 등장) | ⚠️ 완료 (후반 배경 flip 문제 있음) | 마지막 프레임이 스튜디오 배경으로 변질 |
| 씬 6 | Solve (기공 흡수) | 🔄 **진행 중 — 2샷 분리 재제작** | 4차 재생성 실패, 현재 Shot 1 시작 스틸 준비 단계 |
| 씬 7 | Reaction (승리 포즈) | ⬜ 대기 | Shot 2 마지막 프레임으로 연결 예정 |

---

## 👥 팀 역할 분담 (확정)

| 영역 | 주관자 | 책임 |
|---|---|---|
| **전체 총괄 + 크레딧 게이트키퍼** | Claude | 팀 조율, QC 최종 승인, 방향성 판단 |
| **시각 자산 + 이미지/영상 분석** | ChatGPT | PNG 제작, 시작/끝 프레임 결정, 프레임 검수 |
| **Kling 5-field 프롬프트 작성** | 설계봇 (ChatGPT 커스텀 GPT) | 5필드 구조로 실전 프롬프트 출력 |
| **씬 서사·대본·액션 구조** | Claude | 3단계/4단계 액션, 대본 정리, QC 체크리스트 |

**충돌 시 원칙**: 해당 영역 주관자 결정 우선. 총괄(Claude)은 크레딧 투입 전 최종 검수.

---

## 🔥 실전 학습사항 (4편 제작 중 축적)

### 1. Kling AI 설정 (v4 문서와 차이)
| 항목 | v4 문서 | 실전 확정값 |
|---|---|---|
| 모델 | VIDEO 2.6 | **VIDEO 3.0** |
| 길이 | 7초 기본 | 5초(멀티샷) / 10초(복합) 유연 |
| 끝 이미지 | 언급 없음 | **투명 배경 PNG 절대 투입 금지** |

### 2. 제올라이트 색상 이원화 규칙 (신규)
- **본체 색상**: 평상시 연한 연녹색 (pale mint green)
- **스킬 발동 시**: 파스텔 민트-시안 오로라 (soft pastel mint-cyan aurora)
- 절대 금지: 형광 네온 라임 (neon lime green) — 빌런 암모니아 색과 혼동됨

### 3. Solve 컷 프롬프트 규칙 (중대 수정)

**❌ 사용 금지 표현** (Kling이 "가스가 몸에 박힘"으로 오역):
- `absorbed into the crystal pores on the body`
- `gas being absorbed into the hero's body`
- `gas touching the character`
- `gas near the face / mouth`
- `gas merging with the body`
- `suction motion` (방향성 오역 유발)

**✅ 권장 표현**:
- `gas trail stretching toward the hero, dissipating in midair before reaching the body`
- `toxic gas shrinking and fading from its original location frame by frame`
- `gas pulled by invisible force, thinning out in the empty space`
- `the tail of the gas bends long like vacuumed dust, then vanishes in the air around the hero without touching the body`

### 4. 시작 프레임 선택 원칙 (팀 공통 규칙)

**이전 씬 마지막 프레임을 시작 프레임으로 직접 사용하는 것은 환경 continuity + 캐릭터 identity 둘 다 유지될 때만 허용**

**직접 사용 금지 조건**:
1. 캐릭터 외형이 원본과 달라졌을 때
2. 배경은 맞지만 캐릭터 퀄리티가 흔들릴 때
3. 다음 씬의 스킬/액션 PNG와 연결 시 이질감이 예상될 때

**대체 원칙**:
- 이전 프레임은 **환경 reference**로만 사용
- 원본 PNG는 **캐릭터 identity reference**로만 사용
- 필요 시 ChatGPT가 새 시작 스틸을 별도 생성

**씬 제작 순서**:
1. 시작 스틸 신규 제작 (환경 + 캐릭터 동시 유지)
2. Shot 1 생성
3. Shot 1 마지막 프레임으로 Shot 2 생성

### 5. 2샷 분리 구조 (Solve 컷 적용)
- Solve 컷은 "인지 단계 + 정화 단계"로 분리하여 각각 생성
- 각 샷은 Multi-shot OFF
- Shot 2의 시작 프레임 = Shot 1의 마지막 프레임

### 6. 액션 단계 설계 (씬 6 기준)
**4단계 구조 (챗지피티 확장안 수용)**:
1. 둘러보기 (주변 스캔)
2. 잔재 발견 (응시, 결의)
3. 자세잡기 (발 고정, 중심 낮춤)
4. 스킬 발동 (정화장 발동 + 가스 소멸)

---

## 📖 프로젝트 기본 정보

### 브랜드
- **이름**: 리네이처 제올라이트 (ReNature Zeolite)
- **웹사이트**: renaturezeolite.com
- **플랫폼**: YouTube Shorts · Instagram Reels · TikTok · Naver Clip
- **총 편수**: 30편 (Phase 1: 1~10편 / Phase 2: 11~20편 / Phase 3: 21~30편)

### 파이프라인
```
Claude (대본·샷리스트)
→ ChatGPT (캐릭터 PNG 제작)
→ 설계봇 (Kling 프롬프트 설계)
→ Kling AI Pro (클립 생성)
→ ElevenLabs (음성)
→ Vrew (편집·자막)
→ ContentAuto Pro (배포)
```

### 캐릭터 6종
| 구분 | 색상/톤 | 주요 공간 |
|---|---|---|
| 이소발레르산 | 노란 가스 | 신발장·신발 속 |
| 암모니아 | 초록 가스 | 반려동물·화장실·어항 |
| 트리메틸아민 | 보라 가스 | 냉장고·음식물 |
| 포름알데히드 | 회백색 안개 | 새집·가구·벽지 |
| 곰팡이균 | 검녹/검은 얼룩 | 옷장·욕실·베란다 |
| **제올라이트 (영웅)** | 연민트~백색 본체 / 민트-시안 스킬 | 모든 해결 장면 |

---

## 🚫 절대 금지 (브랜드 컴플라이언스)

### 표현 금지
- FDA / GRAS / 인증 / 승인 / 등록
- 발암물질 제거 / 예방 / 치료
- 100% / 완벽 / 확실하게
- 방사능·중금속 제거

### 캐릭터 규칙
- Kling으로 새 캐릭터 생성 금지
- 기본형 PNG 하나로 모든 씬 커버 금지
- 새 악당 추가 금지 (5종 유지)
- 신발장 편에 암모니아 사용 금지 (이소발레르산 사용)

### 제작 규칙
- 자막 먼저 만들기 금지 (음성 → 자막 순서)
- 수치 영상당 1회만
- 흰 배경 / 스튜디오 룩 / 고립된 캐릭터 금지 (environment integrated shot 필수)

---

## 📁 저장소 파일 구조 (계획)

```
renature-shorts-docs/
├── STATE.md                        ← 이 파일 (현재 상태)
├── 00_master_rules.md              ← 마스터 플랜 v5 (준비 중)
├── 01_character_bible.md           ← 캐릭터 바이블 (준비 중)
├── 02_scene_canon.md               ← 씬 카논 (준비 중)
├── 03_design_bot_patch.md          ← 설계봇 Instructions v5 (준비 중)
├── 04_claude_scene_guide.md        ← Claude 대본 가이드 (준비 중)
├── 05_qc_checklist.md              ← QC 체크리스트 (준비 중)
├── scripts/
│   └── renature_scripts_v2.md      ← 30편 완성 대본
└── handoffs/
    └── 2026-04-22_handoff.md       ← 대화별 인수인계 로그
```

---

## 🔄 STATE.md 업데이트 규칙

### 누가 업데이트하나
- **Claude (총괄)**: 대화 종료 시점마다 업데이트 제안 및 초안 생성
- **다봄님**: 최종 검토 후 GitHub에 커밋

### 언제 업데이트하나
1. 씬이 완료될 때마다
2. 새로운 규칙/금지 표현이 확정될 때마다
3. 팀 운영 체계가 변경될 때마다
4. 실전 학습사항이 축적될 때마다

### 어떻게 업데이트하나
1. Claude가 대화 종료 전 변경사항 요약
2. 다봄님이 GitHub 웹에서 STATE.md 편집 (연필 아이콘 클릭)
3. 커밋 메시지 남기고 저장

---

## 📞 다음 대화 시작 시 사용할 프롬프트

새 대화 시작할 때 각 AI에게 다음과 같이 말씀하시면 됩니다:

### Claude에게
```
이 URL의 STATE.md 읽고 맥락 복원해줘:
https://raw.githubusercontent.com/dabomcns-art/renature-shorts-docs/main/STATE.md
```

### ChatGPT에게
```
이 URL의 STATE.md 먼저 확인하고 시작해줘:
https://raw.githubusercontent.com/dabomcns-art/renature-shorts-docs/main/STATE.md
```

### 설계봇 Instructions에 추가
```
[프로젝트 필수 참조]
대화 시작 시 다음 URL의 STATE.md를 반드시 확인하여 
최신 프로젝트 상태와 규칙을 파악:
https://raw.githubusercontent.com/dabomcns-art/renature-shorts-docs/main/STATE.md

특히 "Solve 컷 프롬프트 규칙"과 "시작 프레임 선택 원칙" 
섹션은 모든 씬 설계에 반드시 반영.
```

---

> **이 문서가 최신 상태를 반영하도록 팀 모두가 책임집니다.**  
> 변경사항이 있으면 반드시 이 문서에 기록하고 커밋하세요.
