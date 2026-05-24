# 🔄 AI 워크플로우 규칙 (WORKFLOW_RULES)
## Step-by-Step Workflow Procedures

**목적:** AI 팀의 작업 프로세스를 명확히 정의  
**담당자:** ChatGPT Pro  
**최종 업데이트:** 2026-05-24 16:45

---

## 🚀 일반적인 작업 프로세스 (7단계)

### Step 1️⃣: 작업 확인 (2분)
```
1. MASTER_AI_MANUAL.md 읽기
2. AI_TASK_QUEUE.csv에서 할당된 작업 확인
3. AI_FILE_LOCKS.md에서 파일 상태 확인
4. AI_LIVE_STATUS.md에서 현재 상태 확인
```

### Step 2️⃣: 상태 업데이트 (1분)
```
1. AI_LIVE_STATUS.md에 자신의 상태를 "작업 시작" 으로 변경
2. 시작 시간과 작업명 기록
3. 작업 대상 파일 명시
```

### Step 3️⃣: 파일 잠금 (1분)
```
1. AI_FILE_LOCKS.md에 수정할 파일 목록 추가
2. 상태를 "🔴 잠금"으로 변경
3. 예상 완료 시간 기록
```

### Step 4️⃣: 작업 실행
```
1. 할당된 작업 수행
2. 필요하면 AI_INBOX.md에 제안 작성
3. 다른 AI의 검수 필요시 요청
```

### Step 5️⃣: 파일 수정 (필요시)
```
1. 할당된 AI가 파일 생성/수정
2. 변경 사항 명확히 기록
3. 품질 검수 실시
```

### Step 6️⃣: 완료 기록 (1분)
```
1. AI_LIVE_STATUS.md에 "작업 완료" 기록
2. 완료 시간 기록
3. AI_FILE_LOCKS.md에서 파일 잠금 해제
```

### Step 7️⃣: 보고 (2분)
```
1. AI_DAILY_REPORT_TEMPLATE.md에 일일 보고 작성
2. 한국어 3줄 요약 작성
3. 필요시 허간에게 보고
```

---

## 🎯 상황별 워크플로우

### 콘텐츠 작업 흐름
```
ChatGPT Pro: 콘텐츠 전략 + 아이디어 생성
    ↓
Claude Max: 초안 작성 + 검수
    ↓
ChatGPT Pro: 최종 검수 + 승인
    ↓
Codex: 파일 저장 + 메타데이터 관리
    ↓
허간: 최종 승인 + 업로드
```

### 리서치 작업 흐름
```
Gemini Pro: 시장/경쟁사 조사
    ↓
AI_INBOX.md에 결과 기록
    ↓
ChatGPT Pro + Claude: 검토
    ↓
Codex: 결과 파일 저장 (02_account_research/)
    ↓
ChatGPT Pro: 전략에 반영
```

### 의사결정 흐름
```
문제 발생
    ↓
AI들의 의견 수렴
    ↓
AI_DM_BOARD.md에서 규칙 확인
    ↓
ChatGPT Pro 최종 결정
    ↓
AI_DECISION_LOG.md에 기록
    ↓
관련 파일 업데이트
```

---

## 📞 문제 해결 워크플로우

### 파일 충돌 발생
```
1. AI_FILE_LOCKS.md 확인
2. 담당 AI에게 연락
3. 작업 완료 대기 또는 순서 변경
4. ChatGPT Pro에 보고
```

### 작업 지연
```
1. AI_LIVE_STATUS.md에 지연 사유 기록
2. ChatGPT Pro에 즉시 보고
3. AI_TASK_QUEUE.csv에서 우선순위 재조정
```

### 의견 불일치
```
1. AI_DM_BOARD.md에서 공식 규칙 확인
2. AI_DECISION_LOG.md에서 유사 결정 참고
3. ChatGPT Pro에 최종 판단 요청
```

---

## ✅ 워크플로우 체크리스트

매 작업 시작 전:
- [ ] MASTER_AI_MANUAL.md 읽음
- [ ] AI_TASK_QUEUE.csv 확인
- [ ] AI_FILE_LOCKS.md 확인
- [ ] 자신의 권한 확인

작업 중:
- [ ] AI_LIVE_STATUS.md 업데이트함
- [ ] AI_FILE_LOCKS.md 파일 잠금함
- [ ] 주기적으로 진행 상황 기록

작업 완료:
- [ ] AI_LIVE_STATUS.md 완료 기록
- [ ] AI_FILE_LOCKS.md 파일 해제
- [ ] AI_DAILY_REPORT_TEMPLATE.md 보고
- [ ] 한국어 요약 작성

---

**담당자:** ChatGPT Pro  
**시행 일자:** 2026-05-24  
**다음 검토:** 2026-06-24