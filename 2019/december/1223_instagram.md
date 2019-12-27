# Django로 Instagram 기능 구현하기



## 1. 경로 및 가상환경 설정하기

1. ~/projects/wps12/instagram/
2. env : was-instagram-env (Interpreter 설정해주기)
3. $ pip install 'django<3.0'
4. $ git init & git ignore
   - .gitignore      #gitignore.io. (Git, Linux, macOS, Python, Django, Windows, PyCharm+all, jupyternotebook)
5. $ pip install django-extensions notebook (필수사항 아님, settings의 INSTALLED_APPS에 추가해줘야 작동함)
6. pip freeze > requirements.txt (필요한 프로그램들을 list-up하여 파일로 만들어줌)



## 2. project 시작하기

1. $ django-admin startproject config (프로젝트 생성)

2. $ mv config app (config폴더의 이름을 app으로 변경)

3. app폴더를 sources root 설정하기

   <img src="/Users/moonpeter/Library/Application Support/typora-user-images/image-20191224101855003.png" alt="image-20191224101855003" style="zoom: 33%;" />



## 3. app 추가하기

1. members앱 추가
   - $ django-admin startapp members
2. posts앱 추가
   - $ django-admin startapp posts





## 24일 수업한 내용



HTTP Scheme + HOST + MEDIA_URL + FileField의 실제 값

http//: + localhost:8000 + /meida/ + popsts/images/파일명.jpg

![image-20191224143043684](/Users/moonpeter/Library/Application Support/typora-user-images/image-20191224143043684.png)

![image-20191224143124546](/Users/moonpeter/Library/Application Support/typora-user-images/image-20191224143124546.png)

=> prefix=settings.MEDIA_URL, 로 변경





쿠키기반 사용자 세션

![image-20191224185700341](/Users/moonpeter/Library/Application Support/typora-user-images/image-20191224185700341.png)