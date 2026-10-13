# AIDXhakerton

AIDx 해커톤 Pro-Code 부문 준비용 참고 레포입니다. 실제 제출은 주최 측 팀 저장소(team01~16)에서 합니다.

## 구성

| 경로 | 내용 |
|---|---|
| [resources/리소스_정리.md](resources/리소스_정리.md) | 라이브러리·스킬·프롬프트 목록, 일정 체크리스트 |
| [starter-kit/](starter-kit/) | 팀 저장소에 복사해 쓸 기본 세트 |
| [starter-kit/CLAUDE.md](starter-kit/CLAUDE.md) | Claude 작업 규칙 (ID 체계, 상태값, 커밋 규칙) |
| [starter-kit/README.md](starter-kit/README.md) | 제출용 README 양식 |
| [starter-kit/docs/](starter-kit/docs/) | 제출 문서 7종 양식 |

## 제출 문서 8종

| 문서 | 질문 | ID |
|---|---|---|
| README.md | 어떻게 실행하고, 결과는 어디서 보나 | — |
| docs/project-brief.md | 무엇을, 누구를 위해 만드나 | — |
| docs/prd.md | 무엇이 되면 완성인가 | REQ, AC |
| docs/arch.md | 어떻게 구성했나 | — |
| docs/experience.md | 사용자는 어떻게 경험하나 | FLOW |
| docs/development.md | AI와 어떻게 개발했나 | Issue |
| docs/security-compliance.md | 보안 기준을 어떻게 지켰나 | SEC |
| docs/e2e-test.md | 어떻게 시험했고 무엇이 확인됐나 | TC |

연결 원칙: **REQ → AC → Issue → 코드 → TC → 실제 결과**

## 스타터킷 사용법

1. 주최 측 팀 저장소를 클론한다.
2. 주최 측이 이미 넣어둔 docs 양식이 있으면 그걸 우선하고, 이 레포의 양식에서 빠진 표만 옮긴다.
3. 없으면 `starter-kit/` 내용을 팀 저장소 루트에 복사한다.
   ```bash
   cp -r starter-kit/. <팀저장소 경로>/
   ```
4. 주최 측 `docs/security-policy.md`는 덮어쓰지 않는다.
5. 주제 공개(10/14) 후 `resources/리소스_정리.md`의 프롬프트 P2부터 순서대로 사용한다.
