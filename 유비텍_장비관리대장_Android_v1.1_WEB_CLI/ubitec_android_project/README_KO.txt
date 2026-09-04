유비텍 장비관리대장 Android 프로젝트

현재 Windows EXE에서 확인한 24개 장비 항목을 모바일 화면으로 옮긴 버전입니다.

기능
- 통합 검색
- 고객사 / 구분 / Model 필터
- 조회 장비 / 고객사 / 구분 / Model / IP 미입력 현황
- 장비 등록 / 상세 수정 / 삭제
- WEB 주소 외부 브라우저 열기
- SSH / Telnet 주소를 설치된 Android 접속 앱으로 전달
- XLSX 가져오기 / XLSX 내보내기
- JSON 백업 / 백업 복원
- 고객사별 / 구분별 / Model별 장비 현황
- 계정 숨기기
- 동일 장비 식별은 기존 PC 로직과 동일하게 S/N -> MAC -> 고객사+Hostname -> 고객사+No 순서 사용

모바일 데이터는 앱 내부 저장소(IndexedDB)에 저장됩니다.
PC 자료를 옮길 때는 Windows 프로그램에서 XLSX 내보내기 후 Android 앱의 '엑셀 가져오기'를 사용하면 됩니다.

주의
- Android에서는 Windows CMD를 사용할 수 없으므로 SSH/Telnet은 별도 Android SSH/Telnet 앱이 설치되어 있어야 합니다.
- Android판 엑셀 가져오기는 XLSX를 대상으로 구현했습니다. 구형 XLS는 지원하지 않습니다.
