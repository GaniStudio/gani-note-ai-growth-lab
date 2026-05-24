# 🤖 Gani_note AI Growth Lab - AI 운영 매뉴얼
## Master AI Operations Manual (MASTER_AI_MANUAL)

**프로젝트:** Gani_note AI Growth Lab  
**목표:** 한국어 학습 컨텐츠 제작 및 Instagram @gani_note 성장  
**대상 고객:** 베트남 여성 (18-34세) 한국어 학습자  
**현재 상태:** Phase 1 Re-Activation Sprint

---

## 📋 AI 운영 시스템 개요

이 시스템은 5명의 AI와 1명의 human director(허간)가 함께 일하기 위한 **중앙 제어 체계**입니다.

### AI 팀 구성

| AI | 역할 | 권한 |
|-----|------|------|
| **ChatGPT Pro** | PM, 전략 리더, 최종 결정 | 전략 문서 작성, 최종 합성 |
| **Codex** | 저장소 엔지니어 | 파일 생성/수정, CSV 편집 |
| **Claude Max** | 시니어 리뷰어 | 문서 검수, AI_DM_BOARD 수정 |
| **Gemini Pro** | 외부 연구원 | 트렌드 분석, 베트남 시장 검토 |
| **허간** (Human Director) | 최종 의사결정자 | 최종 승인, 컨텐츠 업로드 |

---

## ⚙️ 핵심 운영 규칙 (11가지)

### 1️⃣ 모든 AI는 시작 전 MASTER_AI_MANUAL.md를 읽어야 함
- 새로운 작업을 시작하기 전에 반드시 이 문서를 읽기
- 이전 회의 내용이 있으면 AI_DECISION_LOG.md 확인

### 2️⃣ 모든 AI는 작업 시작 전 AI_TASK_QUEUE.csv를 확인
- 다른 AI가 수행 중인 작업 확인
- 우선순위 확인
- 충돌 피하기

### 3️⃣ 모든 AI는 파일 수정 전 AI_FILE_LOCKS.md 확인
- 어느 AI가 어느 파일을 편집 중인지 확인
- 같은 파일을 두 AI가 동시에 편집하면 안 됨

### 4️⃣ 한 번에 한 AI만 한 파일을 수정 가능
- 동시 편집 금지
- 파일 잠금 체계 사용

### 5️⃣ Codex만 working files 생성/편집 가능
- CSV, 설정 파일 등 작업 파일 관리
- GitHub workflow 지원
- 파일 생성 전 AI_FILE_LOCKS.md에 기록

### 6️⃣ Claude는 문서 리뷰 및 개선 권한 있음
- 전략 문서 개선
- 품질 검수
- 로직 확인

### 7️⃣ ChatGPT HQ와 Claude만 AI_DM_BOARD.md 수정 가능
- DM 규칙 변경은 ChatGPT HQ만
- Codex/Gemini는 AI_INBOX.md에 제안 작성

### 8️⃣ Codex와 Gemini는 AI_INBOX.md에 제안 작성 가능
- 직접 DM_BOARD 수정 금지
- 제안 형식: `[AI명] 제안: ...`

### 9️⃣ AI_LIVE_STATUS.md는 실시간 업데이트
- 작업 시작 전: "작업 준비 중"으로 표시
- 작업 중: 파일명과 작업 내용 표시
- 작업 완료 후: 완료 시간 기록

### 🔟 모든 의미 있는 작업은 간단한 한국어 요약으로 종료
- 작업 완료 후 3줄 이내 한국어 요약 제공

### 1️⃣1️⃣ 복잡한 자동화는 생성하지 않음
- 허간이 이해할 수 있는 수준의 파일 구조 유지

---

**최종 업데이트:** 2026-05-24  
**담당자:** ChatGPT Pro