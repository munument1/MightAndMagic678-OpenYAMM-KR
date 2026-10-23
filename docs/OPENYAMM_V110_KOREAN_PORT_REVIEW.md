# OpenYAMM v1.10 한국어 대응 검토 (2026-10-23)

공식 릴리스: https://github.com/pjasicek/openyamm/releases/tag/v1.10 (2026-10-22 UTC)

## 실제 원본 차이

- 공식 `1.5...v1.10` Git 비교: `ahead`, 신규 커밋 17개.
- Android 업데이트 UI 신규 소스: `android/app/src/main/java/org/openyamm/android/OpenYammUpdateActivity.java`.
- Android 업데이터 신규 소스: `android/app/src/main/java/org/openyamm/android/OpenYammUpdater.java`.
- 공식 v1.10 릴리스 노트: 업데이트 노트 스크롤 영역, 긴 대화문 잘림 수정, Linux Wayland 원거리 안개 수정.

## 한국어 이식 게이트

1. 위 Android 신규 UI와 업데이터의 **실제 사용자 노출 문자열**을 추출하고 기존 한국어 번역과 대조한다. 기술 식별자와 URL은 번역하지 않는다.
2. 긴 대화문 잘림 수정과 기존 한국어 HUD/폰트 패치가 충돌하는지 비교한다.
3. `korean-localization` 브랜치의 기존 PO·오버레이를 보존한 채 별도 통합 브랜치에서 이식한다.
4. Windows 및 Android 빌드, 대화창·업데이트 화면의 한글 표시를 확인한 후에만 배포를 재개한다.

**상태:** 공식 v1.10 소스 차이 확인. 이 문서는 코드 동기화·신규 UI 번역·인게임 검증 완료를 의미하지 않는다. `KOREAN_RELEASE_HOLD=true` 유지.
