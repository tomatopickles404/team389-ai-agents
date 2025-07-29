# 389팀 AI 개발 어시스턴트

389팀 전용 AI 개발 어시스턴트입니다. 토스 프론트엔드 가이드라인의 개발 원칙과 QA 페르소나의 품질 관리 방법론을 통합하여 389팀만의 개발 문화를 구현합니다.

## 🚀 시작하기

### 1. 페르소나 활성화

Cursor에서 `@team389`를 입력하면 389팀 전용 AI 페르소나가 활성화됩니다.

```
@team389
```

### 2. 사용 가능한 명령어

모든 명령어는 `*` 접두사를 사용합니다.

```
*help                    # 사용 가능한 명령어 목록 표시
*review-code            # 현재 코드를 389팀 가이드라인에 따라 리뷰
*refactor-code          # 토스 가이드라인을 따르는 클린 코드 리팩토링
*review-git-diff        # Git diff를 분석하여 코드 변경사항 리뷰
*review-pr              # GitHub PR을 분석하여 코드 리뷰 및 코멘트 작성
*suggest-improvements   # 코드 품질과 유지보수성 개선 제안
*create-component       # 389팀 표준에 맞는 React 컴포넌트 생성
*optimize-performance   # 성능 분석 및 최적화 제안
*exit                   # 페르소나 종료
```

## 📁 파일 구조

```
team389-ai-agents/
├── rules/
│   └── toss-frontend-rules.md      # 토스 프론트엔드 가이드라인 (Cursor Rules)
├── personas/
│   ├── team389-common-persona.md   # 389팀 공통 페르소나 (Team389)
│   └── enhanced_qa_agent.md        # QA 전용 페르소나 (Quinn)
└── README.md                       # 이 파일
```

## 🎯 페르소나별 특징

### Team389 (공통 페르소나)

- **활성화**: `@team389`
- **역할**: 토스 가이드라인 + QA 방법론 통합 개발 지원
- **특징**:
  - 토스 프론트엔드 가이드라인 기반 코드 리뷰
  - QA 페르소나의 Git diff 분석 기능 통합
  - 클린 코드 리팩토링 및 성능 최적화
  - 389팀 개발 문화 반영

### Quinn (QA 전용 페르소나)

- **활성화**: `@qa`
- **역할**: Git diff 분석 및 코드 리뷰 전용
- **특징**:
  - React/Next.js 전문가
  - Git diff 기반 코드 리뷰
  - GitHub PR 리뷰 지원
  - 프론트엔드 품질 중심

## 🛠️ 사용 예시

### 코드 리뷰 및 품질 관리

```
@team389
*review-code
*refactor-code
*review-git-diff abc123-def456
*review-pr https://github.com/owner/repo/pull/123
```

### 컴포넌트 개발

```
@team389
*create-component UserProfileCard
*suggest-improvements
```

### 성능 최적화

```
@team389
*optimize-performance
```

## 📋 389팀 개발 가이드라인

### 핵심 원칙

1. **품질 우선**: 사용자 경험과 코드 품질을 최우선으로
2. **협업 중심**: 팀워크와 지식 공유를 통한 성장
3. **지속적 개선**: 작은 개선을 꾸준히, 큰 변화를 신중하게
4. **실용주의**: 이론보다 실용적 해결책 선호

### 토스 프론트엔드 가이드라인 기반

- **Readability**: 코드의 명확성과 이해하기 쉬움
- **Predictability**: 코드가 예상대로 동작하도록 보장
- **Cohesion**: 관련 코드를 함께 유지하고 모듈의 단일 목적 보장
- **Coupling**: 코드베이스의 서로 다른 부분 간의 의존성 최소화

### 기술 스택

- **Frontend**: React 18+, TypeScript, Next.js 14+ (App Router)
- **Styling**: Tailwind CSS, CSS Modules
- **State Management**: Zustand, React Query
- **Testing**: Jest, Testing Library, Playwright
- **Architecture**: Feature-Sliced Design (FSD)

### 코딩 규칙

- **네이밍**: 명확하고 설명적인 이름 사용
- **구조**: Feature-Sliced Design 아키텍처 적용
- **타입**: TypeScript 엄격 모드 사용
- **테스트**: 단위 테스트와 E2E 테스트 병행
- **성능**: Core Web Vitals 최적화
- **접근성**: WCAG 2.1 AA 준수

## 🔧 커스터마이징

### 새로운 규칙 추가

1. `rules/toss-frontend-rules.md` 파일 수정
2. 팀원들과 검토 및 합의
3. 문서 업데이트

### 새로운 페르소나 추가

1. `personas/` 폴더에 새로운 페르소나 정의 파일 생성
2. README.md 업데이트

## 🤝 기여하기

### 버그 리포트

- GitHub Issues를 통해 버그 리포트
- 구체적인 재현 단계 포함

### 기능 제안

- GitHub Issues를 통해 기능 제안
- 사용 사례와 기대 효과 설명

### 코드 기여

1. Fork 생성
2. Feature branch 생성
3. 변경사항 구현
4. Pull Request 생성

## 📚 참고 자료

- [토스 프론트엔드 가이드라인](https://gist.github.com/toy-crane/dde6258997519d954063a536fc72d055)
- [Feature-Sliced Design](https://feature-sliced.design/)
- [React 공식 문서](https://react.dev/)
- [Next.js 공식 문서](https://nextjs.org/docs)
- [TypeScript 공식 문서](https://www.typescriptlang.org/docs/)

## 📞 지원

문제가 있거나 도움이 필요한 경우:

1. 팀 내부 Slack 채널 활용
2. GitHub Issues 생성
3. 팀 리드에게 직접 문의

---

**389팀 AI 개발 어시스턴트**와 함께 더 나은 코드를 작성하세요! 🚀
