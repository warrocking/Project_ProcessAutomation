# 원본 및 정리 범위

복사 기준 커밋: `3194623a51019d419ba0b6a0af3133bc933d4df6`. 기존 파일은 수정·이동·삭제하지 않았습니다. 새 코드 복사본은 원본과 SHA-256이 동일합니다. [복사 검증 목록](copy-manifest.json).

| 원본 경로 | 새 경로 |
|---|---|
| `RobotStudio/project.mod` | `project.mod` |
| `RobotStudio/DI_DO_Signals.csv` | `DI_DO_Signals.csv` |
| `RobotStudio/PLC_ServerConnect/`의 Python 3개·JSON·requirements | `pc_client/` |

## 원본에 그대로 둔 자료

- [수업 실습](../../RobotStudio/practice/)과 [RAPID·서버 학습 자료](../../RobotStudio/RAPID_Server_Study/): 타이어 핵심 코드와 구분하기 위해 새 폴더에는 복사하지 않았습니다.
- [RAPID 입문 발표자료](../../RobotStudio/ABB_RAPID_입문.pptx): 별도 학습 자료입니다.
- [개발 환경 설정 기록](../../RobotStudio/SETUP_LOG.md), 원본 `.vscode`: 개발 환경 자료이며 새 폴더의 설정으로 복제하지 않았습니다.
- [client_test.ps1](../../RobotStudio/client_test.ps1), [robot_connector.ps1](../../RobotStudio/robot_connector.ps1): 주석과 명령을 확인한 결과 `ex_p224.mod`의 `11/22/33/qq` 소켓 실습 도구입니다. 타이어 `start/end` 클라이언트와 다릅니다.
- [New Module.mod](../../RobotStudio/PLC_ServerConnect/New%20Module.mod): 메인 코드와 다른 모듈이며 정확한 버전 관계가 확인되지 않아 원본에 보관합니다.
- [기존 AI 작업 메모](../../RobotStudio/CLAUDE.md), [Python 개발 프롬프트](../../RobotStudio/PLC_ServerConnect/plc_python_prompt.md): 원본은 유지하고 기술 설명은 새 문서로 작성했습니다.

두 폴더는 자동 동기화되지 않습니다. 이후 코드 변경은 어느 버전을 수정하는지 명시해야 합니다. 원본 `RobotStudio`를 가리키는 기존 지원서·QR 링크는 계속 유지됩니다. 정리된 설명을 공유할 때는 `Tire_Process_Automation` 주소를 사용합니다.
