# 작업 규칙 (AIDx 해커톤 Pro-Code)

이 레포는 AI 기술평가(문서·코드·실행/테스트 결과·GitHub 이력·AI 활용 기록)를 받는다.
모든 작업은 **REQ → AC → Issue → 코드 → TC → 실제 결과**가 ID로 연결되도록 한다.

## ID 체계
- `REQ-01` 주최 측 요구 / `REQ-X01` 팀 추가 아이디어 (docs/prd.md)
- `AC-01` 인수조건 (docs/prd.md)
- `FLOW-01` 사용자 흐름 (docs/experience.md)
- `TC-01` 시험 케이스 (docs/e2e-test.md, 테스트 이름에도 포함)
- `SEC-01` 보안 항목 (주최 측 docs/security-policy.md 번호를 그대로 사용)

## 상태값 (모든 문서 공통)
`미구현` / `구현` / `검증완료` / `미검증` / `제외`
- 테스트를 실제로 실행해 통과한 것만 `검증완료`로 쓴다.
- 예시·계획·mock은 완료로 쓰지 않는다.

## 작업 순서
1. 모든 작업은 GitHub Issue 번호로 시작한다.
2. 관련 AC를 검증하는 테스트를 먼저 작성하고 실패를 확인한다.
3. 구현해서 테스트를 통과시키고, 실행 명령과 결과를 남긴다.
4. 커밋 메시지: `[REQ-01/AC-01] 요약 (#이슈번호)`
5. docs/development.md 작업 기록 표에 한 줄 추가한다.
6. 보안 관련 변경은 docs/security-compliance.md 해당 SEC 행을 갱신한다.

## 금지
- 주최 측 docs/security-policy.md 수정 금지
- 토큰·키·비밀번호를 코드나 문서에 쓰지 않는다 (.env 사용, .env는 커밋 금지)
- 실행하지 않은 결과를 추정해서 쓰지 않는다

## 기술 기준
- 프런트엔드: React 계열 필수 (React / Next.js)
- UI: KDS(KT UX Design System) 컴포넌트 우선. 직접 만든 컴포넌트는 이유를 docs/arch.md에 기록
- 예시·mock 데이터는 코드와 화면에서 실제 데이터와 구분 표시
