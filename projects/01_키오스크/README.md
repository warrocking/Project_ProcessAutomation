# 콘솔 키오스크 구현

관리자와 고객의 주문 흐름을 분리한 C++ 콘솔 키오스크입니다. 메뉴 변경, 주문·할인·결제, 영수증 저장, 매출 조회를 JSON 데이터 구조로 연결했습니다.

## 구조

- `src/`: C++ 소스와 CMake 설정
- `resources/`: 메뉴·권한·결제 결과 JSON
- `docs/`: 프로젝트 설명 자료

## 실행

```text
cmake -S src -B build
cmake --build build
```

실행 환경은 C++17 이상이며, `resources/`의 JSON 파일이 실행 위치에서 읽혀야 합니다.
