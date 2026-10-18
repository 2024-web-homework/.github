# .github
# Web Programming CRUD Project — HW 02 to HW 03

2024년 웹 프로그래밍 과제에서 하나의 데이터 관리 프로젝트를 단계별로 발전시킨 기록입니다. 정적인 도서 목록 화면에서 시작해 DB 기반 CRUD, 이미지 첨부와 검색 기능, 그리고 Spring MVC의 계층 분리까지 학습했습니다.

네 저장소는 각각 별개의 결과물이 아니라 이 프로젝트의 네 단계입니다. 코드 변화와 과제별 실행 환경을 보존할 수 있도록 통합 저장소에서는 단계마다 폴더를 나눕니다.

## 진행 과정


| HW 02-1 | `list.jsp`에 예시 도서 목록이 고정되어 있습니다. 등록·수정 폼 결과 페이지는 전달된 값을 표시합니다.

| HW 02-2 | `BoardDAO`, `BoardVO`, `JDBCUtil`을 사용해 MariaDB의 `BOARD` 테이블에 도서 데이터를 등록·조회·수정·삭제합니다. `searchBoardList`에서 도서명 검색도 처리합니다. | JDBC CRUD와 DAO/VO 역할 분리 |

| HW 02-3 | `BoardDAO`가 제목·작성자·내용·이미지 경로를 DB에 저장하고, 업로드된 이미지는 웹앱의 `upload` 폴더에 둡니다. 게시글 CRUD, 제목 검색, 날짜 범위 필터, 정렬 기능이 있습니다. | 파일 업로드와 DB에 파일 경로 저장, 검색 조건 구성 |

| HW 03 | Spring MVC의 `BoardController` → `BoardService` → `BoardDAO` 구조로 목록·등록·수정·삭제·상세 조회와 검색을 구성합니다. `JdbcTemplate`을 사용하며 `BOARD2` 테이블과 `BoardVO`를 다룹니다. | Controller/Service/DAO 계층 분리와 Spring JDBC |


## 기술

- Java, Maven
- JSP, Servlet, HTML/CSS
- JDBC, MariaDB
- Spring MVC, Spring JdbcTemplate


JSP 폼에서 받은 데이터를 화면에 표시하는 것부터 시작해, JDBC 기반 CRUD와 검색, 이미지 업로드, Spring MVC의 계층 구조까지 순서대로 다뤘습니다. 같은 데이터 관리 주제를 여러 구현 방식으로 확장하며 웹 애플리케이션의 구조를 익힌 프로젝트입니다
