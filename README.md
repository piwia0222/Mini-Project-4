# 4차 미니프로젝트
장보경, 박성호, 윤찬혁, 이가영, 이준형

# AI 표지 생성 도서관리시스템

## 실행 방법
1. `npm install -g json-server` (최초 1회)
2. `npm install`
3. 터미널 1: `npm run server` → http://localhost:3000/books
4. 터미널 2: `npm run dev` → http://localhost:5173

## 서비스 구조
- 라우트: `/` 목록, `/books/:id` 상세, `/books/new` 등록, `/books/:id/edit` 수정
- API: GET·POST `/books`, GET·PATCH·DELETE `/books/:id`
- 데이터(db.json): id, title, author, content, coverImageUrl, createdAt, updatedAt

## 팀 R&R
- A (이름): 환경설정·공통 레이아웃·머지 관리
- B (이름): 도서 목록
- C (이름): 도서 상세·삭제
- D (이름): 등록·수정 폼
- E (이름): AI 표지 생성

## 협업 규칙
- main에 직접 push 금지, 기능 브랜치에서 작업 후 PR
- 브랜치: feature/list, feature/detail, feature/form, feature/ai-cover
- db.json은 A만 수정 (테스트로 바뀌면 `git checkout db.json`)
- OpenAI API Key는 절대 커밋하지 않기
- 커밋 메시지: feat: / fix: / docs:
