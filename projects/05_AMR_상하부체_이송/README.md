# AMR을 활용한 자동차 상·하부체 생산·이송

ABB 로봇 3대, Omron LD-90 AMR, Arduino 브릿지, Python 중앙 서버와 PLC를 TCP 통신으로 연동한 자동차 조립 자동화 프로젝트입니다.

## 구조

- `src/Rapid/`: ABB 로봇 프로그램
- `src/Server/`: 중앙·중계 서버 코드
- `src/Arduino/`: AMR I/O 브릿지 코드
- `resources/`: 설정과 신호 자료
- `docs/`: 공정·통신 설명

## 담당 역할

ABB RAPID 코드, 실제 로봇 좌표 티칭, 중앙·중계 서버의 명령·상태 연계를 담당했습니다. 로봇 완료 상태와 AMR 도착 상태가 모두 확인될 때만 출고하도록 조건을 구성했고, 여러 명령이 한 번에 수신될 때 버퍼에 남는 문제를 줄 단위 메시지 분리로 수정했습니다.

시연 영상: https://www.youtube.com/watch?v=jK3QsIFbCSc&t=5s
