# ABB 로봇 기반 타이어 공정 자동화

ABB 로봇과 PLC I/O 신호를 연계해 타이어 이송, 프레스, 냉각, 색상 판별, 코팅, 창고 적재 공정을 구성한 팀 프로젝트입니다.

## 구조

- `src/project.mod`: ABB RAPID 공정 시퀀스와 TCP 서버
- `src/pc_client/`: Python TCP 통신 코드
- `resources/DI_DO_Signals.csv`: 공정 신호표
- `docs/`: 공정 흐름과 통신 설명

## 담당 역할

팀 회의와 공정 순서 정리, ABB RAPID 코드 작성, 실제 로봇 좌표·동작 티칭, Python 통신 프로그램을 담당했습니다. PLC 래더 전체를 담당한 프로젝트는 아닙니다.

시연 영상: https://www.youtube.com/watch?v=O2JILGMgIAs
