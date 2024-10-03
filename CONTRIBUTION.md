## Branch Protection Rule for `main` Branch

### 🔒 Branch name pattern
- `main`

### 🛡️ Required Rules:
1. **Require pull request reviews before merging**:
   - 최소 **1명** 이상의 리뷰어가 PR을 승인해야 병합이 가능합니다.
   - 리뷰어의 승인이 완료되지 않으면 병합할 수 없습니다.

2. **Require status checks to pass before merging**:
   - 지정된 테스트나 빌드 상태 검사(예: CI/CD)가 통과해야 병합이 가능합니다.
   - 모든 상태 검사가 통과되지 않으면 병합할 수 없습니다.

3. **Include administrators**:
   - 관리자는 이 규칙을 무시할 수 없습니다.
   - 관리자 또한 리뷰 및 상태 체크를 통과해야 병합 가능합니다.

### ✅ Benefits:
- 코드 품질 향상: 최소한의 코드 리뷰를 요구해 오류 발생 가능성 감소.
- 테스트 자동화: 상태 검사(예: 테스트 통과)를 강제하여 안정적인 코드 병합 보장.
- 일관성 유지: 관리자도 규칙을 따르게 해 모든 병합이 동일한 워크플로우를 따름.
