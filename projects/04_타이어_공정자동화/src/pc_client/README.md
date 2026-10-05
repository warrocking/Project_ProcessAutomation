# PC–ABB 로봇 TCP 통신 도구

원본 `RobotStudio/PLC_ServerConnect`의 Python 코드와 데이터 파일을 그대로 복사했습니다. 파일명·import·데이터 참조 관계는 유지했습니다.

| 파일 | 역할 |
|---|---|
| `main.py` | 연결 수·형식·주소 입력, 순차 세션 실행 |
| `tcp_connection.py` | TCP 연결, 송수신, 종료 |
| `data_format.py` | Plain Text·JSON·MC Protocol 처리 |
| `database.json` | JSON 필드 확인에 사용하는 데이터 |
| `requirements.txt` | MC Protocol 관련 의존성 |

## 실행 흐름

해당 폴더에서 `python main.py`를 실행합니다. MC Protocol 기능을 사용할 때는 `python -m pip install -r requirements.txt`로 의존성을 준비합니다. Plain Text 모드에서는 MC Protocol 라이브러리를 불러오지 않습니다.

타이어 RAPID 코드와 통신할 경우 연결 수 1, 형식 1(Plain Text), 실제 설정에 맞는 IP·포트를 입력합니다. 원본 RAPID 바인딩 값은 `192.168.3.3`, 포트 `5000`입니다. 장비 연결과 동작 조건을 확인한 환경에서 `start` 명령을 사용합니다. `end`는 로봇 측 종료 요청이고 `exit`는 PC 입력 루프 종료이므로 서로 다릅니다.

## 동작상 주의점

원본 클라이언트는 송신 뒤 응답을 기다리는 동기식 구조이고, 수신 기본 제한 시간은 5초입니다. 생산 중 `end`를 검사하는 RAPID 루틴에는 응답 송신이 없어 해당 경로에서 수신 대기 시간 초과가 발생할 수 있습니다. 따라서 이 복사본을 검증된 전용 운영 클라이언트로 설명하지 않습니다.

이번 정리는 파일 복사와 문서 작성 작업입니다. 실제 로봇 접속·생산 동작 시험은 수행하지 않았습니다. 코드 수정 없이 원본의 동작과 제한을 설명했습니다.
