# Brandme
.html -> .php 전체 변경


# 추가적인 기능
- 타 사용자의 포트폴리오를 확인할 수 있는 기능
- 포트폴리오에 관한 정보, 팁등을 공유할 수 있는 게시판을 포함한 페이지


# login, signup
- 로그인, 회원가입 기능
- 폼 태그, 스크립트 수정해서 DB연동 후 작동하도록 변경

# main 
- 메인페이지
- main_setting에서 입력 받은 값 적용

# main_setting
- DB input form
- 입력 폼 작성
- 폼에서 입력받은 데이터를 DB에 insert 혹은 update 가능하도록 개발


# DB 테이블 명세

    # userinfo 
        - 유저 테이블
        - (user_id(pk), user_pw, user_name)
        - 유저 아이디, 패스워드, 이름
        - 로그인 및 회원가입 시 사용

    # home 
        - home 테이블

        - (user_id(pk, fk), user_name, occupation, home_introduction, user_img, git, blog ...)
        - 유저 아이디, 이름, 직종, 소개, 이미지, 깃 주소, 블로그 주소

    # about 
        - about 테이블

        - (user_id(pk, fk), about_img, about_introduction, experience, project, worked)
        - 유저 아이디, 이미지, 소개, 경력년도, 완료 프로젝트 수, 완료 외주 수

    # skills_frontend
        - skill_프론트앤드 테이블

        - (user_id(pk, fk), career, skill1, skill2, skill3, skill4, skill1_per, skill2_per, skill3_per, skill4_per)
        - 유저 아이디, 경력, 스킬, 이해도

    # skills_backend
        - skill_백앤드 테이블

        - (user_id(pk, fk), career, skill1, skill2, skill3, skill4, skill1_per, skill2_per, skill3_per, skill4_per)
        - 유저 아이디, 경력, 스킬, 이해도

    # qualification 
        - qualification 테이블

        - (user_id(pk, fk), edu(boolean), work(boolean))
        - 학력, 경력(제거할까 생각중)

    # qualification_edu 
        - (user_id(pk, fk), edu1, edu1_location, edu1_period ...)

    # qualification_work 
        - (user_id(pk, fk), work1, work1_location, work1_period ...)

    # services 


    # Board
        - 






