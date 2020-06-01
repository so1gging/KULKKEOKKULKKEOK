## 💡기능구현 및 설명
#### 프로젝트 설명 KULKKEOK KULKKEOK
개발기간 : 2020.04.30 ~ 2020.05.18
투입인원 : 4명
프로젝트 소개 : 전세계 맥주 정보를 제공하는 사이트


#### 📌담당 업무
자유·공지게시판 / 게시판 댓글·대댓글 / 마이페이지 / 관리자 페이지 / 맥주 이상형 월드컵 페이지 / 파일 업로드 / 카카도 지도 API 구현
기존 JDBC를 myBatis framework로 변경
코드 병합

#### 사용 언어 및 IDE
Java 8
JavaScript, jQuery, JSP/Servlet
HTML5, CSS
Eclipse

### Framework
bootstrap , myBatis

### Server
Apache Tomcat v9.0

### DBMS
Oracle - SQL developer(11g)

### OS
Chrome

---

#### 📌코드 설명
#### 1. Post (free · notice) & Commenct (FreeController, NoticeController, PostService, PostDao, Paging, PostDto, CommentDto)

+ __freeboard.jsp(자유게시판)__ :
 답글형 게시판, 자유게시판 목록 , 인기게시글 상단에 표시(일정 조회수 이상) ,페이징
 
+ __freeboard_view.jsp(글 상세폼 + 댓글)__ :
 게시글 상세 폼 , 게시글 답변달기 및 CRUD, 댓글 리스트(AJAX) , 대댓글 CRUD(AJAX)
 
+ __freeboard_write.jsp(글 작성)__ :
 글 작성폼

+ __freeboard_edit.jsp(글 수정)__ :
글 수정폼

+ __freeboard_answer.jsp(답글 작성)__ :
답글 작성폼

+ __notice.jsp(공지게시판)__ :
답글형 게시판, 공지게시판 목록 , 인기게시글 상단에 표시(일정 조회수 이상) ,페이징

+ __notice_view.jsp(공지 상세폼 + 댓글)__ :
공지 게시글 상세 폼 , 공지 게시글 답변달기 및 CRUD, 댓글 리스트(AJAX) , 대댓글 CRUD(AJAX) * 관리자만 CRUD 가능 *

+ __notice_write.jsp(공지 작성)__ :
공지 작성폼 (관리자만 가능)

+ __notice_edit.jsp(공지 수정)__ :
공지 수정폼 (관리자만 가능)

+ __notice_answer.jsp(공지 작성)__ :
공지 작성폼 (관리자만 가능)


#### 2. Mypage (MypageController , MypageService , MypageDao)
+ __wmypage_my.jsp (내 정보 수정)__ :
사용자 정보 수정 폼

+ __mypage_mybeer.jsp (북마크한 맥주)__ :
사용자가 북마크 한 맥주 리스트

+ __mypage_mymoim.jsp (내가 연 모임)__ :
사용자가 연 모임 리스트

+ __mypage_myreview.jsp (작성한 리뷰)__ :
사용자가 작성한 리뷰 리스트

+ __mypage_unsubscribe.jsp (회원 탈퇴)__ :
회원탈퇴


#### 3. Admin (AdminController , AdminService, AdminDao)
+ __admin_activity.jsp (회원 리스트)__ :
사이트를 가입한 모든 회원 리스트 출력

+ __admin_userMng.jsp ( 회원 활동 관리)__ :
회원 활동(작성한 게시글 , 작성한 댓글 , 개최한 모임, 작성한 모임 댓글) 삭제 및 열람 가능

+ __beerinfo_write.jsp (맥주 추가하기)__:
맥주 정보 업로드

#### 4. world cup(WorldCupController, WorldCupService, WorldCupDao, WorldCup)
+ worldcup_start.jsp (맥주 월드컵 시작 페이지)
맥주 이상형 월드컵 시작 페이지

+ worldcup_play.jsp (맥주 월드컵 playing 페이지)
맥주 이상형 월드컵 플레이 페이지

+ worldcup_win.jsp (맥주 월드컵 end페이지
맥주 이상형 월드컵 결과 및 순위

#### 5. 기타 :
카카오 지도 API, 파일 업로드
