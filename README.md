# Claude 업무 워크스페이스 템플릿

Claude Code + Notion을 활용한 업무 관리 워크스페이스 템플릿입니다.

## 시작하기

### 1. 이 템플릿으로 내 레포 만들기
GitHub에서 **Use this template** → 내 계정에 레포 생성

### 2. 로컬에 클론
```bash
git clone https://github.com/{내계정}/{레포이름}
cd {레포이름}
```

### 3. Notion MCP 연결
Claude Desktop → 설정 → 통합(Integrations) → Notion 연결

### 4. Claude Code 실행 후 /setup
```
/setup
```
Claude가 질문에 따라 개인 설정 + 노션 연결을 자동으로 완료합니다.

### 5. 내 레포에 저장
```bash
git add .
git commit -m "setup: 워크스페이스 초기 설정"
git push
```

---

## 스킬 목록

| 스킬 | 설명 |
|------|------|
| `/setup` | 최초 1회 온보딩 |
| `/work-start` | 오늘 업무 시작 — 노션에 할 일 생성 |
| `/work-end` | 오늘 업무 마무리 — 노션에 한 일 기록 |
| `/meeting` | 회의록 노션 자동 저장 |
| `/memo` | 업무 메모 즉석 저장 |

---

## 구조

```
├── CLAUDE.md                    # Claude 행동 지침
├── .gitignore
└── .claude/
    ├── user-config.md           # 개인 설정 (setup 후 자동 생성)
    ├── notion-pages.md          # 노션 페이지 URL 맵 (setup 후 자동 생성)
    └── commands/
        ├── setup.md             # 온보딩 스킬
        ├── work-start.md        # 업무 시작 스킬
        └── work-end.md          # 업무 마감 스킬
```
