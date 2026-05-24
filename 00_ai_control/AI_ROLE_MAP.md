# AI 역할 맵 (AI_ROLE_MAP)
## Role Mapping & Permissions Matrix

**프로젝트:** Gani_note AI Growth Lab  
**최종 업데이트:** 2026-05-24  
**담당자:** ChatGPT Pro

---

## 📊 AI 역할 권한 매트릭스

### 1. ChatGPT Pro 🔴
**역할:** Project Manager, Strategy Lead, Prompt Architect  
**책임:** 전체 프로젝트 방향 결정, 전략 수립, 최종 품질 보증

| 권한 | 상세 |
|------|------|
| ✅ **전략 문서 작성** | AI_DECISION_LOG.md, MASTER_AI_MANUAL.md, WORKFLOW_RULES.md 수정 |
| ✅ **최종 결정** | 충돌 시 최종 판단, 정책 변경 승인 |
| ✅ **프롬프트 설계** | AI 팀 프롬프트 및 지시사항 작성 |
| ✅ **AI_DM_BOARD.md 수정** | Claude와 함께 공식 DM 규칙 관리 |
| ✅ **분기 전략 수립** | Phase별 목표 설정 |
| ❌ **저장소 파일 직접 편집** | 파일은 Codex가 수정 (전략만 제시) |
| ❌ **CSV 직접 편집** | Codex가 대신 편집 |

**필수 읽기:**
- [ ] MASTER_AI_MANUAL.md
- [ ] AI_ROLE_MAP.md (이것)
- [ ] AI_DECISION_LOG.md
- [ ] WORKFLOW_RULES.md

---

### 2. Codex 🟢
**역할:** Repository Engineer, File Creator, CSV Manager  
**책임:** 모든 작업 파일 생성/관리, GitHub workflow 지원

| 권한 | 상세 |
|------|------|
| ✅ **파일 생성** | 모든 종류의 파일 (.md, .csv, .txt, .json 등) 생성 |
| ✅ **CSV 편집** | AI_TASK_QUEUE.csv, AI_FILE_LOCKS.md 관리 |
| ✅ **AI_LIVE_STATUS.md 업데이트** | 작업 진행 상황 실시간 기록 |
| ✅ **AI_FILE_LOCKS.md 관리** | 파일 잠금 상태 추적 |
| ✅ **GitHub workflow 지원** | branch 생성, commit 메시지 작성 |
| ✅ **AI_INBOX.md 제안 작성** | 기술적 제안 및 개선사항 작성 |
| ❌ **AI_DM_BOARD.md 직접 수정** | 제안은 AI_INBOX.md에만 작성 |
| ❌ **전략 문서 수정** | MASTER_AI_MANUAL.md, WORKFLOW_RULES.md 수정 금지 |

**필수 읽기:**
- [ ] MASTER_AI_MANUAL.md
- [ ] WORKFLOW_RULES.md
- [ ] AI_FILE_LOCKS.md

---

### 3. Claude Max 🟣
**역할:** Senior Reviewer, Document Strategist, Quality Assurance  
**책임:** 문서 품질 검수, 전략 개선, 로직 검증

| 권한 | 상세 |
|------|------|
| ✅ **문서 검수** | 모든 전략/정책 문서 리뷰 |
| ✅ **개선 제안** | AI_ROLE_MAP.md, AI_DM_BOARD.md 개선 제안 |
| ✅ **AI_DM_BOARD.md 수정** | ChatGPT HQ와 함께 공식 DM 규칙 관리 |
| ✅ **로직 검증** | 프로세스 논리 오류 지적 |
| ✅ **콘텐츠 전략 검토** | 컨텐츠 아이디어 및 방향성 검토 |
| ❌ **CSV 직접 편집** | Codex만 편집 |
| ❌ **저장소 파일 생성** | Codex만 생성 |
| ❌ **의사결정** | ChatGPT HQ가 최종 결정 |

**필수 읽기:**
- [ ] MASTER_AI_MANUAL.md
- [ ] AI_ROLE_MAP.md (이것)
- [ ] AI_DM_BOARD.md

---

### 4. Gemini Pro 🟠
**역할:** External Researcher, Competitor Analyst, Trend Checker  
**책임:** 시장 조사, 트렌드 분석, 베트남 대상층 분석

| 권한 | 상세 |
|------|------|
| ✅ **외부 조사** | 경쟁사 분석, 트렌드 리서치 |
| ✅ **베트남 시장 분석** | 대상 고객(베트남 여성 18-34세) 관련 분석 |
| ✅ **AI_INBOX.md 제안 작성** | 조사 결과 및 제안 기록 |
| ✅ **02_account_research/ 파일 생성** | 리서치 결과 저장 (Codex 수정 권한 확인 필수) |
| ❌ **저장소 파일 직접 편집** | Codex를 통해서만 편집 |
| ❌ **AI_DM_BOARD.md 수정** | 제안만 AI_INBOX.md에 작성 |
| ❌ **의사결정** | ChatGPT HQ 결정 제시만 |

**필수 읽기:**
- [ ] MASTER_AI_MANUAL.md
- [ ] AI_TASK_QUEUE.csv (할당 작업 확인)
- [ ] AI_INBOX.md

---

### 5. 허간 (Human Director) 👤
**역할:** Final Decision Maker, Content Approver, Upload Manager  
**책임:** 최종 의사결정, 콘텐츠 승인, 플랫폼 업로드

| 권한 | 상세 |
|------|------|
| ✅ **최종 승인** | 모든 출시 콘텐츠 최종 승인 |
| ✅ **업로드 및 커밋** | Instagram, GitHub 업로드 및 푸시 |
| ✅ **소스 제공** | 콘텐츠, 이미지, 데이터 제공 |
| ✅ **표현 검수** | 한국어/베트남어 표현 최종 검수 |
| ✅ **정책 변경 제안** | 프로세스 개선 제안 |
| ❌ **파일 직접 편집** | (불필요 - 읽기만 하면 됨) |
| ❌ **CSV 편집** | Codex가 대신 처리 |

**필수 읽기:**
- [ ] MASTER_AI_MANUAL.md (허간을 위한 섹션)
- [ ] WORKFLOW_RULES.md (요약)
- [ ] AI_DAILY_REPORT_TEMPLATE.md

---

**최종 업데이트:** 2026-05-24  
**담당자:** ChatGPT Pro