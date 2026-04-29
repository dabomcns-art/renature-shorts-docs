markdown# 리네이처 제올라이트 숏폼 프로젝트 — 현재 상태 (STATE.md)

> **최종 업데이트**: 2026년 4월 29일  
> **관리 주체**: Claude (총괄) + ChatGPT (시각자산) + 설계봇 (Kling 프롬프트)  
> **저장소**: https://github.com/dabomcns-art/renature-shorts-docs

---

## 🚨 팀원 필독 (대화 시작 시 반드시 확인)

이 문서는 리네이처 숏폼 프로젝트의 **단일 진실 소스**입니다.  
Claude, ChatGPT, 설계봇 중 어느 팀원이든 새 대화를 시작할 때 이 문서를 먼저 읽고 맥락을 복원하세요.

### 가장 최근 핵심 결정사항 (2026-04-29 기준)
1. **4편 (반려동물 편) 제작 완주** — 9개 씬/샷 모두 완성 ✅
2. **End image 타이밍 제어 학습**: 단일샷 + Start/End image 방식의 한계 발견 → 정확한 타이밍 제어 필요시 멀티샷 2분할로 샷 경계 활용
3. **Kling 빔 차단의 함정 학습**: "외부로 발산" vs "몸으로 박힘" 구분 필요. 사쿠라 변신 같은 임팩트 컷에선 방사형 빔 허용해야 함
4. **STATE.md 금지 표현은 상황별 적용**: 가스 흡착 컷 vs 일상 컷에서 입 동작/접촉 규칙이 정반대
5. **3자 협업 패턴 정착**: Claude(분석/검수) + ChatGPT(압축/실전) + 다봄님(판단/방향)

---

## 📋 현재 진행 상태

| 항목 | 값 |
|---|---|
| 제작 완료한 편 | **4편 (반려동물·암모니아) 완주** ✅ |
| 다음 단계 | 4편 후반 작업 (음성·편집·자막·업로드) |
| 그 다음 | 4편 KPI 수치 확인 → 1편 제작 시작 |

---

## 🎬 4편 씬별 진행 상태

| 씬 | 역할 | 상태 | 비고 |
|---|---|---|---|
| 씬 1 | Hook intro (가로 패닝) | ✅ 완료 | 좌→우 패닝, End image 활용 |
| 씬 2 | Problem (방향제 스프레이) | ✅ 완료 | 기존 영상 편집 |
| 씬 3 | Villain entrance (암모니아) | ✅ 완료 | 기존 영상 편집 |
| 씬 4 | Villain rampage | ✅ 완료 | 그대로 사용 |
| 씬 5 | Hero entrance | ✅ 완료 | 그대로 사용 |
| 씬 6 Shot 1 | Hero action (회전 + 손 들기) | ✅ 완료 | 카드캡터 사쿠라 변신 컨셉 |
| 씬 6 Shot 2A | 사쿠라 변신 빛 폭발 | ✅ 완료 | 3번 시도 끝에 임팩트 도달 |
| 씬 6 Shot 2B | 가스 흡착 + 정화 | ✅ 완료 | 5번 시도 끝에 도달 |
| 씬 7 | CTA + 윙크 마무리 | ✅ 완료 | 멀티샷 2분할로 윙크 타이밍 제어 |

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

### 2. 제올라이트 색상 이원화 규칙
- **본체 색상**: 평상시 연한 연녹색 (pale mint green)
- **스킬 발동 시**: 파스텔 민트-시안 오로라 (soft pastel mint-cyan aurora)
- 절대 금지: 형광 네온 라임 (neon lime green) — 빌런 암모니아 색과 혼동됨

### 3. Solve 컷 프롬프트 규칙

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
- `vapor dissolves at the outer edge of aura halo`

### 4. 시작 프레임 선택 원칙

**이전 씬 마지막 프레임을 시작 프레임으로 직접 사용하는 것은 환경 continuity + 캐릭터 identity 둘 다 유지될 때만 허용**

**직접 사용 금지 조건**:
1. 캐릭터 외형이 원본과 달라졌을 때
2. 배경은 맞지만 캐릭터 퀄리티가 흔들릴 때
3. 다음 씬의 스킬/액션 PNG와 연결 시 이질감이 예상될 때

**대체 원칙**:
- 이전 프레임은 **환경 reference**로만 사용
- 원본 PNG는 **캐릭터 identity reference**로만 사용
- 필요 시 ChatGPT가 새 시작 스틸을 별도 생성

### 5. 2샷 분리 구조 (Solve 컷 적용)
- Solve 컷은 "인지 단계 + 정화 단계"로 분리하여 각각 생성
- 각 샷은 Multi-shot OFF
- Shot 2의 시작 프레임 = Shot 1의 마지막 프레임

### 6. 액션 단계 설계 (씬 6 기준)
**4단계 구조**:
1. 둘러보기 (주변 스캔)
2. 잔재 발견 (응시, 결의)
3. 자세잡기 (발 고정, 중심 낮춤)
4. 스킬 발동 (정화장 발동 + 가스 소멸)

### 7. End image 타이밍 제어 (4편 제작 중 신규 학습)

**문제 상황**: 단일샷 + Start frame + End image 사용 시
- Kling이 End image를 영상 끝에 정확히 착지시키지 않음
- 중간부터 점진적 보간 → 의도한 타이밍보다 변화가 일찍 나타남
- 예시: 씬 7에서 5초 끝에 윙크 의도했으나 단일샷에서 3초쯤부터 윙크 시작

**해결책**: 변화 시점을 정확히 제어해야 하는 컷은 커스텀 멀티샷 2분할
- Shot 1: 안정 상태 유지 (변화 없음, 눈 뜬 상태로 대사 등)
- Shot 2: 짧은 변화 (0.5~1초, 윙크/표정 변화)
- 샷 경계가 시간 지시(0~5초 식)보다 강력한 타이밍 제어 도구

**적용 케이스**:
- 윙크/표정 변화 마무리
- 액션 종료 시점 정확히 제어 필요
- 대사 끝 + 별도 동작

### 8. 빔/광선 차단의 함정 (4편 제작 중 신규 학습)

**문제 상황**: 씬 6 Shot 2A에서 "NO straight beams" 강하게 차단했더니 사쿠라 변신 임팩트가 죽음

**구분 필요**:
- ❌ 캐릭터 몸으로 들어오는 빔 (가스 흡수 시 변질 위험) — 차단 유지
- ✅ 캐릭터 손에서 외부로 발산되는 빔 (변신/스킬 임팩트) — 허용

**프롬프트 권장 표현**:
Light beams MUST radiate OUTWARD from the hero (hero → outside),
NEVER inward (outside → hero). Beams shoot away from the body,
not into it.

### 9. 상황별 입/접촉 규칙 (4편 제작 중 신규 학습)

**핵심 원칙**: STATE.md 금지 표현은 상황에 따라 정반대로 적용됨

**가스 흡착 컷** (씬 6 Shot 2A/2B):
- ❌ "mouth opens" → 가스가 입으로 들어가는 변질
- ❌ "gas touching body" → 가스가 몸에 박히는 변질
- ✅ 영웅은 passive, 입 닫힘, 가스는 aura 가장자리에서 소멸

**일상/CTA 컷** (씬 7):
- ✅ "natural talking lip motion" → 영웅이 시청자에게 말함
- ✅ 시바견이 영웅 핥는 친밀한 접촉 OK
- 같은 단어("mouth", "touch")라도 컨텍스트에 따라 정반대 적용

### 10. 가스 표현 변질 패턴 (4편 제작 중 신규 학습)

**Kling이 가스를 캐릭터화시키는 트리거**:
- "ammonia" 단어 자체 (학습된 의인화 경향)
- "gas stretching toward hero" → 영웅 형태로 변신
- "gas reacting" → 표정 있는 캐릭터로 변질

**안전 표현**:
- "pale green smoke / vapor / haze" (ammonia 단어 회피)
- "formless atmospheric mist, no creature, no eyes, no face" 명시
- "shrinks and fades in place" or "dissolves at aura boundary" 

### 11. 거실 톤 변화 과욕 함정 (4편 제작 중 신규 학습)

**문제**: 5초 안에 "어두운 거실 → 따뜻한 햇살"까지 가려고 하면 배경 재해석 발생

**원칙**: 5초 클립에서 배경 분위기 변화는 **자연스러운 정도**로만
- ❌ "warm golden afternoon sunlight fills the space"
- ✅ "softer and clearer ambient light"
- 거실 자체는 같은 공간 유지, 톤만 미세 조정

---

## 📖 프로젝트 기본 정보

### 브랜드
- **이름**: 리네이처 제올라이트 (ReNature Zeolite)
- **웹사이트**: renaturezeolite.com
- **플랫폼**: YouTube Shorts · Instagram Reels · TikTok · Naver Clip
- **총 편수**: 30편 (Phase 1: 1~10편 / Phase 2: 11~20편 / Phase 3: 21~30편)

### 파이프라인
Claude (대본·샷리스트)
→ ChatGPT (캐릭터 PNG 제작)
→ 설계봇 (Kling 프롬프트 설계)
→ Kling AI Pro (클립 생성)
→ ElevenLabs (음성)
→ Vrew (편집·자막)
→ ContentAuto Pro (배포)

### 캐릭터 6종
| 구분 | 색상/톤 | 주요 공간 |
|---|---|---|
| 이소발레르산 | 노란 가스 | 신발장·신발 속 |
| 암모니아 | 초록 가스 | 반려동물·화장실·어항 |
| 트리메틸아민 | 보라 가스 | 냉장고·음식물 |
| 포름알데히드 | 회백색 안개 | 새집·가구·벽지 |
| 곰팡이균 | 검녹/검은 얼룩 | 옷장·욕실·베란다 |
| **제올라이트 (영웅)** | 연민트~백색 본체 / 민트-시안 스킬 | 모든 해결 장면 |

### 4편에 추가된 캐릭터
- **시바견** (반려동물): 갈색 + 흰색 털, Pixar 스타일, 영웅과 동거 친구

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

## 🤝 3자 협업 패턴 (4편 제작 중 정립)

| 영역 | 담당 | 역할 |
|---|---|---|
| 분석 / 검수 / 문제 진단 | Claude | 결과물 분석, STATE.md 함정 체크, 문제 원인 파악 |
| 압축 / 실전 톤 조정 / 타이밍 진단 | ChatGPT | 프롬프트 압축, 실전 투입용 다듬기, 타이밍 구조 제안 |
| 최종 판단 / 방향 결정 | 다봄님 | 채택/재투입 결정, 컨셉 방향 결정, 크레딧 게이트키핑 |

**활용 예시 (씬 6 Shot 2B)**:
1. Claude가 하이브리드 프롬프트 작성 → 길고 복잡함
2. ChatGPT가 압축본 제안 → 짧고 실전적
3. 다봄님이 ChatGPT 압축본 채택 → 5번째 시도에서 성공

**활용 예시 (씬 7)**:
1. Claude가 단일샷 설계안 작성
2. ChatGPT가 멀티샷 2분할로 타이밍 진단 → 윙크 타이밍 문제 해결
3. 다봄님 채택 → 한 번에 성공

---

## 📁 저장소 파일 구조
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
└── 2026-04-29_handoff.md       ← 대화별 인수인계 로그

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
2. 다봄님이 GitHub 웹에서 STATE.md 편집
3. 커밋 메시지 남기고 저장

---

## 📞 다음 대화 시작 시 사용할 프롬프트

새 대화 시작할 때 각 AI에게 다음과 같이 말씀하시면 됩니다:

### Claude에게
이 URL의 STATE.md 읽고 맥락 복원해줘:
https://raw.githubusercontent.com/dabomcns-art/renature-shorts-docs/main/STATE.md

### ChatGPT에게
이 URL의 STATE.md 먼저 확인하고 시작해줘:
https://raw.githubusercontent.com/dabomcns-art/renature-shorts-docs/main/STATE.md

### 설계봇 Instructions에 추가
[프로젝트 필수 참조]
대화 시작 시 다음 URL의 STATE.md를 반드시 확인하여
최신 프로젝트 상태와 규칙을 파악:
https://raw.githubusercontent.com/dabomcns-art/renature-shorts-docs/main/STATE.md
특히 "Solve 컷 프롬프트 규칙", "시작 프레임 선택 원칙",
"End image 타이밍 제어", "상황별 입/접촉 규칙" 섹션은
모든 씬 설계에 반드시 반영.

---

> **이 문서가 최신 상태를 반영하도록 팀 모두가 책임집니다.**  
> 변경사항이 있으면 반드시 이 문서에 기록하고 커밋하세요.
