# 12월 10일 TIL

## 장고걸스 튜토리얼 1일차

#### 환경설정

- ~projects/wps12/djangogirls/

- env : wps-djangogirls-env

- - pyenv virtualenv 3.7.4 <환경명>

  - pyenv local <환경명>

- - gitinit
  - .gitignore      #gitignore.io. (Git, Linux, macOS, Python, Django, Windows, PyCharm+all)
- pip install 'django<3.0'



#### 장고란 무엇인가요?

무료 오픈소스 웹 애플리케이션 프레임 워크 => 웹 애플리케이션을 만들때 반복적인 작업을 피하기 위해서

urlresolver : url해석기



#### 첫번째 프로젝트

django-admin startproject config .

python manage.py migrate

./manage.py runserver.   => local:8000번에 접속해서 확인(개발서버를 작동시킴)



#### 장고 모델

- 객체 => 모델을 만들어 그 모델이 어떤 역할을 가지고 어떻게 행동해야 하는지 정의하여 서로 알아서 상호작용할 수 있도록 만드는 것

- 장고모델 : 장고안의 모델은 객체의 특별한 종류, 이 모델을 저장하면 내용이 데이터베이스에 저장되는 것이 특별한 점

- 어플리케이션 만들기 : 의미단위로 구분하는 패키지는 만듬, 데이터베이스에 기록이 되면 애플리케이션이다.

  - python manage.py startapp blog. => 블로그 애플리케이션 생성
  - 애플리케이션 생성 후 장고에 사용해야 한다고 알려줘야함 => config/settings.py 를 열어 INSTALLED_APPS 에 'blog' 를 추가

  

블로그 글 모델 만들기

