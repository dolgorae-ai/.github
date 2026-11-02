# Dolgorae AI

회전기계의 알람 확인부터 트렌드 분석, 근거 기반 진단, 정비 보고서 초안 생성까지 연결하는 AI Agent 프로젝트입니다.

## 전체 저장소 클론

아래 명령어를 한 번에 복사해 터미널에서 실행하면 `dolgorae-ai` 디렉터리를 만들고, 각 저장소를 그 안에 클론합니다. Git이 설치되어 있어야 합니다.

```bash
mkdir -p dolgorae-ai
cd dolgorae-ai

for repo in frontend backend ai-agent ml-service infra; do
    git clone "https://github.com/dolgorae-ai/${repo}.git"
done
```

비공개 저장소는 접근 권한이 있는 GitHub 계정으로 인증해야 합니다.

### 클론 후 디렉터리 구조

```text
dolgorae-ai/
├── frontend/       # React 기반 사용자 화면
├── backend/        # Spring Boot 기반 운영 데이터 API
├── ai-agent/       # LangGraph·RAG 기반 진단 및 보고서 생성
├── ml-service/     # 이상탐지·트렌드 분석 및 주기적 탐지
└── infra/          # 공통 개발 환경 및 팀 문서
```

각 폴더는 독립 Git 저장소입니다. 작업할 서비스 폴더에서 브랜치 생성, 커밋, 푸시를 진행합니다.

## 개발 시작하기

- [인프라 실행 안내](https://github.com/dolgorae-ai/infra#readme)
- [시스템 아키텍처](https://github.com/dolgorae-ai/infra/blob/main/docs/ARCHITECTURE.md)
- [팀 컨벤션](https://github.com/dolgorae-ai/infra/blob/main/docs/CONVENTION.md)

서비스별 실행 방법은 각 저장소의 README를 참고하세요.
