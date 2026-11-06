# EasyDoRecord

인터넷 권한 없는 안드로이드 음성 녹음 · 편집 앱. 바로 녹음(앱 바로가기 · 빠른 설정 타일), 파형 보며 자르기 · 구간 삭제 · 분할, m4a 내보내기를 한 앱에서 하고, 녹음은 기기 밖으로 나가지 않음. EasyDo 시리즈.

## 다운로드

최신 버전 0.2.1 — [Releases](https://github.com/parkrye/AppProject_EasyDoRecord/releases)에서 `EasyDoRecord-<버전>.apk`를 받아 설치. Android 8.0 이상.

- 처음 설치 시 "출처를 알 수 없는 앱" 설치 허용 필요. Play 프로텍트가 검사 화면을 띄울 수 있음
- 처음 녹음할 때 마이크 · 알림 권한 요청. 알림은 녹음 중 표시와 일시정지 · 정지 버튼용
- 빠른 설정 타일은 알림창을 내려 편집(연필) 버튼에서 "바로 녹음"을 끌어다 추가
- 업데이트는 새 APK를 같은 방식으로 덮어 설치. 녹음 · 설정 유지
- 앱 안 업데이트 알림 없음. `설정 → 앱 정보 → 새 버전 받기`로 Releases 페이지를 열어 확인
- 서명 인증서 SHA-256: `9c442d01b7f04ff1d8f85eac42c2fe2d3c68143dddc87054b3b7132e75265694`
  (`apksigner verify --print-certs EasyDoRecord-<버전>.apk`로 확인)
- 버그 · 제안은 [Issues](https://github.com/parkrye/AppProject_EasyDoRecord/issues)에

## 기능

| 영역 | 내용 |
|---|---|
| 녹음 | 일시정지 · 재개, 실시간 레벨 표시, 화면을 꺼도 계속 녹음(알림에서 일시정지 · 계속 · 정지), 품질 16 · 32 · 44.1 · 48kHz |
| 단축 실행 | 홈 화면 앱 바로가기 "바로 녹음"(앱 아이콘을 길게 눌러 홈에 고정), 빠른 설정 타일 "바로 녹음"으로 즉시 시작 · 정지 |
| 목록 | 날짜 · 길이 · 크기, 이름 변경 · 삭제 · 공유 · 내보내기 |
| 재생 | 파형(누르거나 끌어서 탐색), 탐색바, 5초 이동, 배속 0.5 ~ 2배, 선택 구간 재생 |
| 편집 | 자르기(선택 구간만 남김) · 구간 삭제(앞뒤 잇기) — 새 녹음 저장 또는 원본 덮어쓰기, 재생 위치에서 두 녹음으로 분할(원본 유지) |
| 내보내기 | m4a(AAC 128kbps) · wav(원본), 원하는 위치에 저장 또는 다른 앱으로 공유 |
| 설정 | `녹음`(녹음 품질) / `화면`(배경화면 색 사용, 기본 꺼짐) / `데이터`(백업 만들기 · 백업에서 복원, 설정만 포함) / `앱 정보`(앱 정보 · 새 버전 받기 · 오픈소스 라이선스) |
| 기타 | 녹음 중 앱이 종료돼 남은 파일 자동 복구 |

녹음은 무손실 WAV로 저장해 편집해도 음질이 떨어지지 않음. 내보낼 때 m4a로 변환.

## 개인정보

인터넷 권한 없음 · 광고 없음 · 수집 · 전송 없음.

- 계정 · 광고 · 사용 통계 · 오류 보고 없음
- 녹음은 앱 전용 저장소에만 저장. 앱 삭제 시 함께 삭제 (Android 클라우드 백업도 끔). 보관할 녹음은 내보내기로 저장
- 내보낸 파일은 사용자가 고른 위치 · 공유한 앱에만 전달
- 권한: 마이크, 녹음 중 알림

## EasyDo 시리즈

| 앱 | 용도 | 플랫폼 |
|---|---|---|
| [EasyDoDraw](https://github.com/parkrye/MultiProject_EasyDoDraw) | 그림 · 애니메이션 | Android · Windows |
| [EasyDoWrite](https://github.com/parkrye/AppProject_EasyDoWrite) | 소설 · 글쓰기 | Android |
| [EasyDoRead](https://github.com/parkrye/AppProject_EasyDoRead) | 책 · 문서 읽기 | Android |
| [EasyDoShelve](https://github.com/parkrye/AppProject_EasyDoShelve) | 웹 소설 서재 | Android |
| [EasyDoPhoto](https://github.com/parkrye/AppProject_EasyDoPhoto) | 카메라 · 사진 편집 | Android |
| [EasyDoDiet](https://github.com/parkrye/AppProject_EasyDoDiet) | 식단 · 운동 기록 | Android |
| [EasyDoZip](https://github.com/parkrye/AppProject_EasyDoZip) | 파일 · 압축 관리 | Android |
| [EasyDoGame](https://github.com/parkrye/AppProject_EasyDoGame) | 미니 게임 모음 | Android |
| [EasyDoMix](https://github.com/parkrye/AppProject_EasyDoMix) | 영상 · 오디오 편집 | Android |
| [EasyDoRecord](https://github.com/parkrye/AppProject_EasyDoRecord) | 녹음 | Android |
| [EasyDoStudio](https://github.com/parkrye/DesktopProject_EasyDoStudio) | 화면 녹화 · 영상 편집 | Windows |

## 라이선스

MIT License · © parkrye. 포함된 서드파티 라이브러리 라이선스는 앱 안 `설정 → 앱 정보 → 오픈소스 라이선스`에서 확인.
