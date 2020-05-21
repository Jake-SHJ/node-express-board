# node-express-board

Board Back-End Logic Design based Node.js &amp; Express.js

## 요구사항

> DB 없이 배열에 담는다고 생각하고 시작

1. Post

- 상태값
  - 작성자
  - 작성시간
  - 작성내용
- 책임
  - 필요한 상태값이 전부 존재하는지에 대한 유효성 검사를 진행할 책임

2. Editor

- 상태값
  - 수정된 Post의 상태값
    - Idx
    - 작성자
    - 작성시간
    - 수정시간
    - 작성내용
- 책임
  - 수정시간을 추가할 책임
  - 수정된 Post의 유효성 검사할 책임

3. Cleaner

- 상태값
  - 삭제될 Post의 상태값
    - Idx
    - 작성자
    - 작성시간
    - 수정시간 (필수값은 아님)
    - 작성내용
- 책임
  - 삭제될 Post의 존재 유무에 대한 유효성을 검사할 책임

4. Posts

- 상태값
  - 등록된 Post 배열
- 책임
  - Post에서 유효성 검사를 통과한 Post를 등록하고 Idx를 부여할 책임
  - Editor에서 유효성 검사를 통과한 수정된 Post로 해당 Post를 변경할 책임
  - Cleaner에서 유효성 검사를 통과한 Post를 제거할 책임
