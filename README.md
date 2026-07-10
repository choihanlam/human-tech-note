# Human Tech Note — 포트폴리오

최한람 · 정보보호 PMO / IT Governance / 기술경영(MOT) / AI

정보보호·IT 거버넌스 실무 9년을 바탕으로 2026년 7월~12월 매주 3편, 총 75편을 연재하는
기술 블로그 **Human Tech Note**의 포트폴리오 사이트입니다.

## 구성

```
HumanTechNote_portfolio/
├─ index.html          # 포트폴리오 메인 (소개·경력·수상·대표작·연재 아카이브·진행률 대시보드)
├─ posts/              # 글 75편 (post-01.html ~ post-75.html)
│                      #  - 대표작 4편(16·36·48·64)은 실제 원고, 나머지는 데모용 더미
├─ .nojekyll           # GitHub Pages에서 그대로 서빙하도록 지정
└─ README.md
```

- 모든 파일은 **자체 완결형**입니다. 스타일(Tailwind CSS)·폰트(Pretendard)·아이콘(Tabler)은 CDN으로 로드되며 별도 빌드가 필요 없습니다.
- 진행률(예정/작성중/발행완료) 상태는 브라우저 `localStorage`에 저장됩니다.

## GitHub Pages 배포 방법

1. GitHub에서 새 저장소 생성 (예: `human-tech-note`)
2. 이 폴더의 **내용물 전체**를 저장소 루트에 업로드
   - 웹 업로드: 저장소 → **Add file → Upload files** → 폴더 안 파일/폴더를 드래그
   - 또는 Git:
     ```bash
     git init
     git add .
     git commit -m "Add Human Tech Note portfolio"
     git branch -M main
     git remote add origin https://github.com/<아이디>/human-tech-note.git
     git push -u origin main
     ```
3. 저장소 **Settings → Pages** → Source: `Deploy from a branch` → Branch: `main` / `/(root)` → Save
4. 잠시 후 `https://<아이디>.github.io/human-tech-note/` 에서 공개됩니다.

## 배포 전 수정할 곳 (index.html)

- 상단 `연락하기` 버튼의 이메일: `mailto:your.email@example.com` → 실제 이메일
- 필요 시 대표작 외 더미 글 본문을 실제 원고로 교체

## 라이선스

© 2026 최한람 · Human Tech Note
