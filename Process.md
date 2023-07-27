# 프로세스(Process)

`프로세스` 

- 실행중인 프로그램
- 운영체제 입장 : 작업의 단위
- 작업 완료를 위해서 특정 자원이 필요
  - CPU time
  - memory
  - files
  - I/O devices



## 프로세스의 메모리 영역

<img src = "./img/img49.png" width = "60%">

- `코드 영역(Text section)`
  - 실행가능한 코드
  - 읽기 전용(read-only)
- `데이터 영역(Data section)`
  - 프로그램이 실행되는 동안 유지할 데이터가 저장되는 공간
  - 전역 변수(global variable)
- `힙 영역(Heap section)`
  - 직접 할당할 수 있는 저장 공간
  - 공간을 할당했다면 언젠가는 해당 공간을 반환해야함
  - `메모리 누수(memory lack)` : 반환하지 않는다면 할당한 공간은 메모리 내에 남아서 메모리 낭비를 초래
- `스택 영역(Stack section)`
  - 데이터를 일시적으로 저장하는 공간
  - 매개변서, 지역 변수
- 정적 할당 영역 :arrow_right: 코드 영역, 데이터 영역
- 동적 할당 영역 :arrow_right: 힙 영역, 스택 영역



