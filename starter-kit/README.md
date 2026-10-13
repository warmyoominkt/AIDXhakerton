# [서비스명]

> 팀: team[번호] · 주제: TOPIC [번호]
> 제출 소스 SHA: `[커밋 SHA]` · 마지막 전체 시험 SHA: `[커밋 SHA]` · 최종 갱신: [YYYY-MM-DD]

[한 줄 소개: 누구의 어떤 문제를 어떻게 해결하는지]

## 1. 실행 환경 (정확한 버전)

| 항목 | 버전 | 확인 명령 |
|---|---|---|
| OS | [예: Ubuntu 22.04 / macOS 14] | |
| Node.js | [예: 20.x.x] | `node -v` |
| 패키지 매니저 | [예: npm 10.x.x] | `npm -v` |
| DB | [종류·버전] | |
| 브라우저 (E2E) | [예: Chromium, Playwright 버전] | |

- 의존성 버전은 lock 파일(`[package-lock.json 등]`)로 고정한다.
- 주요 의존성: [프레임워크, UI 라이브러리(KDS 사용 시 KDS 패키지), DB 드라이버 등]
- (KDS 사용 시) KDS 패키지 설치에 필요한 사내 권한: [필요 권한 설명, 토큰 값은 쓰지 않음]. 안 쓰면 이 줄 삭제

## 2. 설정 (비밀값 없음)

```bash
cp .env.example .env
```

| 변수 | 설명 | 예시 값 | 필수 |
|---|---|---|---|
| `[변수명]` | | `[더미 값]` | 예 |

실제 비밀값은 저장소와 문서에 포함하지 않는다. 받는 방법: [담당자 / 절차]

## 3. 실행 순서

새 환경에서 아래 순서 그대로 실행하면 재현된다.

```bash
# 1) 설치
[예: npm ci]

# 2) 빌드
[예: npm run build]

# 3) DB 준비 (마이그레이션·시드)
[명령]

# 4) 기동
[예: npm run start]   # 접속: http://localhost:[포트]

# 5) 시험
[단위 시험 명령]
[E2E 시험 명령]

# 6) 종료·정리
[예: Ctrl+C / docker compose down -v / 시험 데이터 삭제 명령]
```

| 단계 | 정상 확인 기준 |
|---|---|
| 설치 | 오류 없이 완료 |
| 빌드 | |
| 기동 | [예: 메인 화면 표시] |
| 시험 | 아래 결과 요약과 같은 PASS 수 |
| 종료·정리 | [예: 포트 해제, 시험 데이터 제거] |

**새 환경 재현 확인 기록**

| 확인일 | 확인자 | 환경 | 소스 SHA | 결과 | 비고 |
|---|---|---|---|---|---|
| | | [예: 새로 클론한 다른 PC] | | 성공 / 실패 | |

## 4. 구현 현황

| 구분 | 개수 | 검증완료 | 미검증 | 미구현 |
|---|---|---|---|---|
| 필수 요구 (REQ) | | | | |
| 추가 요구 (REQ-X) | | | | |

상세: [docs/prd.md](docs/prd.md)

## 5. 문서

| 문서 | 내용 |
|---|---|
| [project-brief](docs/project-brief.md) | 문제·사용자·범위, 팀원 역할 |
| [prd](docs/prd.md) | 요구사항(REQ)과 인수조건(AC) |
| [arch](docs/arch.md) | 구성·데이터 흐름·권한 경계 |
| [experience](docs/experience.md) | 사용자 흐름(FLOW)과 화면 |
| [development](docs/development.md) | AI 활용 개발 기록 |
| [security-compliance](docs/security-compliance.md) | 보안 기준 적용·검증 결과 |
| [e2e-test](docs/e2e-test.md) | 시험 시나리오와 실제 결과 |
| security-policy (주최 측) | [docs/security-policy.md](docs/security-policy.md) |

## 6. 시험 결과 요약

| 시험 | 실행 시각 | 소스 SHA | PASS | FAIL | SKIP | 결과 위치 |
|---|---|---|---|---|---|---|
| 단위 시험 | | | | | | [리포트 경로 / CI 링크] |
| E2E 시험 | | | | | | [리포트 경로 / CI 링크] |
| 보안 점검 | | | | | | [docs/security-compliance.md](docs/security-compliance.md) |

## 7. 미검증 항목과 제약

| 항목 | 상태 | 이유 | 관련 문서 |
|---|---|---|---|
| | 미검증 / 미구현 / 제약 | | |
