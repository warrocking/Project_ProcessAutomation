# TurtleBot Fleet Server

ROS2 기반 TurtleBot의 명령과 상태를 TCP로 관리하는 중앙 관제 서버입니다. Control UI, Fleet Server, Robot Command Client가 분리된 구조이며, 서버는 명령·상태·헬스 체크를 관리합니다.

## 구조

- `src/code/`: 서버와 실행 코드
- `src/scripts/`: 실행·점검 스크립트
- `resources/json/`: 서버·클라이언트 설정과 메시지 정보
- `docs/`: 프로토콜과 운영 설명

## 실행

```bash
python3 src/code/server_manager.py
```

실제 로봇 네트워크와 ROS2 환경이 필요합니다. IP와 포트는 `resources/json/`에서 환경에 맞게 설정합니다.
