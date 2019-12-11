# 12월 11일 TIL

## 장고걸스 튜토리얼 2일차

모델-뷰-컨트롤러 :  소프트웨어 공학에서 사용되는 소프트웨어 디자인 패턴이다. 이 패턴을 성공적으로 사용하면, 사용자 인터페이스로부터 비즈니스 로직을 분리하여 애플리케이션의 시각적 요소나 그 이면에서 실행되는 비즈니스 로직을 서로 영향 없이 쉽게 고칠 수 있는 애플리케이션을 만들 수 있다. MVC에서 모델은 애플리케이션의 정보(데이터)를 나타내며, 뷰는 텍스트, 체크박스 항목 등과 같은 사용자 인터페이스 요소를 나타내고, 컨트롤러는 데이터와 비즈니스 로직 사이의 상호동작을 관리한다.



MVC(모델-뷰-컨트롤러)

MTV



**Model**

​	DB

**View (Django: Template)**

​	사용자가 보는 화면

**Controller (Django : View)**

​	DB의 데이터를 사용자가 보는 화면으로 전달(View code를 사용하여 response(HTML형태)를 생성하여 전달) or

​	사용자의 데이터를 적절히 가공해서 DB에 변경사항을 전달



urls.py -> URLResolver

요청의 URL을 판단해서 특정 Controller(View 함수)로 연결



Request -> runserver -> urls.py -> view function ->Response(HTTP 규격)



pip install django-extentions notebook

./manage.py shell_plus --notebook