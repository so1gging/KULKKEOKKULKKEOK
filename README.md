## 💡기능구현 및 설명
#### 프로젝트 설명 KULKKEOK KULKKEOK
개발기간 : 2020.04.30 ~ 2020.05.18
투입인원 : 4명
프로젝트 소개 : 전세계 맥주 정보를 제공하는 사이트


#### 📌담당 업무
자유게시판 / 공지게시판 / 게시판 댓글·대댓글 / 마이페이지 / 관리자 페이지 / 맥주 이상형 월드컵 페이지 / 파일 업로드 / 카카도 지도 API 구현
기존 JDBC를 myBatis framework로 변경

#### 사용 언어 및 IDE
Java 8 / jre 1.8.0_202
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
##### Post (free / notice) & Commenct
view
freeboard.jsp(자유게시판) / freeboard_view.jsp(글 상세폼 + 댓글) / freeboard_write.jsp(글 작성)
freeboard_edit.jsp(글 수정) /freeboard_answer.jsp(답글 작성)

notice.jsp(공지게시판) / notice_view.jsp(공지 상세폼 + 댓글) / notice_write.jsp(공지 작성)
notice_edit.jsp(공지 수정) / notice_answer.jsp(공지 작성)

mvc
FreeController.java  NoticeController.java PostService.java PostDao.java
CommentController.java CommentService.java CommenctDao.java


##### Mypage
view
mypage_my.jsp (내 정보 수정) / mypage_mybeer.jsp (북마크한 맥주) / mypage_mymoim.jsp (내가 연 모임)
mypage_myreview.jsp (작성한 리뷰) / mypage_unsubscribe.jsp (회원 탈퇴)

##### Admin
view
admin_activity.jsp (사이트 내 가입 회원 리스트)
admin_userMng.jsp (사이트 내 가입 회원 활동 관리)
beerinfo_write.jsp (맥주 추가하기)

### world cup
worldcup_start.jsp (맥주 월드컵 시작 페이지)
worldcup_play.jsp (맥주 월드컵 playing 페이지)
worldcup_win.jsp (맥주 월드컵 end페이지)

### 지도 API
moim_wirte.jsp (모임 작성하기)
