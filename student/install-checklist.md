# 설치 체크리스트 — 인프런 · 3순위 Cursor 입문

> **실습 Template**: https://github.com/tjminho/mzmon-items-workshop/generate

---

## 환경

```text
□ Windows 10/11 또는 macOS
□ Node.js 22 LTS — https://nodejs.org
□ pnpm — npm install -g pnpm
□ Cursor — https://cursor.com
□ Git — https://git-scm.com
□ GitHub 계정
```

확인:

```bash
node -v    # v22.x
pnpm -v
git --version
```

---

## Template clone 후 (첫 실행)

```bash
pnpm install
npx prisma migrate deploy
pnpm db:seed
pnpm dev
```

브라우저: http://localhost:3000/items

---

## 문제 해결

| 증상 | 확인 |
|------|------|
| `prisma` 오류 | `npx prisma generate` 후 재시도 |
| 포트 충돌 | 다른 터미널에서 `pnpm dev` 중인지 확인 |
| Windows 경로 | 프로젝트 경로에 한글·공백 최소화 |

Q&A: 인프런 강의 Q&A 또는 cohort Notion
