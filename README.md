# Edutech AI Chatbot

2026-05-15에 제작한 `AI 시대, 인간다움은 무엇일까?` 교육과정 전용 상담 챗봇입니다.

## 산출물

- 상담 챗봇 화면: `ai/ai-education-chatbot.html`
- 관리자 페이지: `ai/admin.html`
- OpenAI API 서버리스 함수: `ai/api/chat.js`
- Vercel 배포 설정: `ai/vercel.json`
- 실행 및 배포 스크립트: `ai/package.json`
- 화면 참고 이미지: `image/`

## 배포 URL

- 챗봇: https://ai-virid-mu.vercel.app
- 관리자: https://ai-virid-mu.vercel.app/admin.html

## 주요 기능

- 문서 기반 10차시 교육과정 상담
- 상담 대상, 상담 주제, 상담 모드별 답변 구성
- 빠른 질문 제공
- 관리자 페이지에서 시스템 프롬프트, 교육 지식, 빠른 질문 수정
- OpenAI Responses API 연동
- API 키 미설정 또는 오류 시 fallback 답변 제공

## 교육과정 반영 내용

- 생성형 AI 기본 개념과 활용 윤리
- 인간 고유 역할과 오감/심리 조향 실습
- `먼저 온 미래` 기반 독서 토론
- ThinkGym 기반 질문 도출과 논리적 주장 구조화
- AI 할루시네이션 검증과 정보 교차 확인
- 미래 직업 예측, 마인드맵, 미래 선언서
- 진로 포트폴리오와 꿈it(잇)다 2.0 연계
- 포트폴리오 50%, 참여도 30%, 성찰일지 20% 평가 구조

## 로컬 실행

```bash
cd ai
npm install
cp .env.example .env.local
npm run local
```

## 배포

```bash
cd ai
npm run deploy
```

OpenAI API 키는 소스에 저장하지 않고 Vercel 환경변수 `OPENAI_API_KEY`로 설정합니다.
