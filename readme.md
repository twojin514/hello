## 백엔드 장고 첫번째 세션에 대한 질문 보충답변 (●'◡'●)





### 📌 가상환경을 독립적으로 관리한다는 것이 무엇이고 왜 그렇게 해야되는가??
- 가상환경이란?
> 독립적인 파이썬의 실행 환경을 의미


- 가상환경이 필요한 이유
> 하나의 pc에 서로 다른 버전의 파이썬과 라이브러리를 쉽게 설치해 사용할 수 있게 하는 것 

> 프로젝트를 진행하다보면 여러 라이브러리, 패키지를 다운로드하여서 사용하게 된다. 그러다 보면 각 라이브러리들끼리 충돌을 일으키는 문제를 발생시키는 경우가 있고 특정 버전과 호환하는 경우가 생겨서 최신 버전과 이전 버전 중 선택해야 하는 상황이 발생하여 잘못하면 전부 삭제해야하는 경우가 발생한다.

> example) 예를 들어 파이썬 개발자 A가 2개의 장고 프로젝트를 개발하고 관리한다고 가정 

>파이썬 장고 프로젝트를 각각 프로젝트1, 프로젝트2 라고 할때, 이때 1과 2에 필요한 라이브러리 버전이 다를 수 있음
예를들어 1에는 a라이브러리 3.1 버전이, 2에는 a라이브러리 4.0 버전이 필요하다고 하면 하나의 PC에 서로 다른 버전의 라이브러리를 설치해야 하는 문제가 생김
이러한 개발 환경은 구축하기도 어렵고 사용하기도 힘든데 파이썬 가상 환경을 이용하면 하나의 PC 안에 독립된 가상 환경을 여러 개 만들 수 있음
즉, 프로젝트 1을 위해 가상 환경 V1을 만들고, 프로젝트 2를 위해 가상 환경 V2를 만들어 서로다른 라이브러리 버전을 설치해 사용할 수 있는 것




### 📌 정적인 대상에는 어떤 파일들이 있을 수 있을까??
-  변하지 않는 파일, 즉 개발자가 서버를 개발할 때 미리 넣어 준비해 놓은 파일로, 서비스 중에 추가되거나 수정되지 않고 고정되어 있음




### 📌 MTV에서 View의 동작을 정의하는 함수는??
- 어떠한 요청이 들어왔을때 "index.html"을 띄어보냄
> ![화면 캡처 2022-05-20 113909](https://user-images.githubusercontent.com/97498094/169438847-c924077a-c2c3-40c3-90c7-7af6cd96da74.png)


- urls.py에 언제 View의 동작을 할지 정해줌
> ![화면 캡처 2022-05-20 114721](https://user-images.githubusercontent.com/97498094/169438802-dd54c7b9-e127-4106-8537-fdbf89e05b2f.png)
> 등록해준 함수를 잘 찾아내기 위해서 import




### 📌 장고에서 자신이 만든 앱을 지정해주는 방식??

- 앱 생성
> ![화면 캡처 2022-05-20 111853](https://user-images.githubusercontent.com/97498094/169435597-995e9a3c-b74d-43fc-967c-3f8d51f79ca8.png)


- 앱 등록
> ![화면 캡처 2022-05-20 112457](https://user-images.githubusercontent.com/97498094/169436240-020b7b18-e248-4bd1-8788-beea2cf8b42d.png)





### 📌 Http에서 Get과 Post 방식의 기능 말고 다른 기능은 무엇이 있는가??
- GET : 서버에게 조회할 리소를 요청한다. (READ, 조회)
- POST : 서버에게 본문(body)에 생성할 데이터를 삽입하여 전송한다. (CREATE, 생성)
- PUT : 서버에게 본문에 수정할 데이터를 삽입하여 전송한다. (UPDATE, 생성)
- DELETE : 서버에게 삭제할 리소스를 요청한다. (DELETE, 삭제)
- PATCH : PUT과 비슷하지만 일부만 수정한다는 점에서 다르다.
