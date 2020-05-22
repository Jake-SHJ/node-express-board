# node-express-board

Board Back-End Logic Design based Node.js &amp; Express.js

## 요구사항

> DB 없이 배열에 담는다고 생각하고 시작

1. Post

- Post는 작성자, 작성일, 수정일, 타이틀, 콘텐츠, 조회수의 상태값을 가진다.
- Post는 상태값의 유효성을 검사해야 한다.

2. Posts

- Post를 작성할 수 있다.
- Post의 목록을 조회할 수 있다.
- Post를 수정할 수 있다.
- Post를 삭제할 수 있다.
- Posts는 게시판 제목을 상태값으로 가진다.

3. Comment

- Comment는 작성자, 작성일, 콘텐츠의 상태값을 가진다.
- Comment는 상태값의 유효성을 검사해야 한다.

4. Comments

- Comment를 작성할 수 있다.
- Comment의 목록을 조회할 수 있다.
- Comment는 수정할 수 없다.
- Comment를 삭제할 수 있다.
- Comments는 특정 Post에 속해야 한다.
