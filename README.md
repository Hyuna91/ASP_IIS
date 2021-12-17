# IIS 설치 및 설정

### 1.IIS 설치
   제어판 → 프로그램 제거 또는 변경 → Windows 기능 켜기/끄기  
   <br>
   <!-- ![IIS_setting](/images/1_제어판.PNG){: width="100" height="100"} -->
   <img src="images/1_제어판.PNG" alt="img1" width="45%" height="auto">
   <img src="images/2_프로그램 제_거_또는_변경.PNG.jpg" alt="img2" width="45%" height="auto">

<br>
<img src="images/3_Windows_기능_켜기_끄기.jpg" alt="img3" width="27%" height="auto">
<img src="images/3_Windows_기능_켜기_끄기_2.jpg" alt="img4" width="27%" height="auto">

인터넷 정보 서비스 → World Wide Web 서비스 → 응용 프로그램 개발 기능  
인터넷 정보 서비스 → 웹 관리 도구  
다음과 같이 설정한다.

---

### 2. IIS 관리자 설정

<img src="images/4_IIS_관리자.jpg" alt="img5" width="50%" height="auto">

    2-1. 웹사이트 추가

<img src="images/5_IIS_관리자_바인딩.jpg" alt="img6" width="60%" height="auto">
<img src="images/6_웹사이트_추가.jpg" alt="img7" width="26%" height="auto">

사이트 이름 : wrestling
실제 경로 : C:\Users\5N\Desktop\wrestling

    2-2. 사이트 바인딩 편집
    기존 포트인 80에서 변경하는 이유 : 포트 충돌 우려가 있어서 변경하는 것을 추천

<img src="images/7_웹사이트_바인딩.jpg" alt="img8" width="60%" height="auto">

<img src="images/8_80포트_변경.jpg" alt="img9" width="35%" height="auto">
<img src="images/9_포트변경_8077.jpg" alt="img10" width="26%" height="auto">

    2-3. 고급 설정
    실제 경로로 지정한 곳이 해당 웹 루트 디렉토리가 된다.

<img src="images/10_고급설정.jpg" alt="img11" width="60%" height="auto">
<img src="images/11_고급설정_실제경로.jpg" alt="img12" width="30%" height="auto">

실제 경로 : C:\Users\5N\Desktop\wrestling

     2-4. 기본 설정
    고급 설정에서 수정하면 자동 반영된다.

<img src="images/12_기본_설정.jpg" alt="img13" width="60%" height="auto">
<img src="images/13_기본_설정_변경.jpg" alt="img14" width="35%" height="auto">

애플리케이션 풀 : Classic .NET AppPool  
실제 경로 : C:\Users\5N\Desktop\wrestling

    2-5. 가상 디렉터리

<img src="images/14_가상_디렉토리_보기.jpg" alt="img15" width="60%" height="auto">

<img src="images/15_가상_디렉토리_보기.jpg" alt="img16" width="60%" height="auto">
<img src="images/16_가상_디렉토리_추가.jpg" alt="img17" width="35%" height="auto">

별칭 : wrestling  
실제 경로 : C:\Users\5N\Desktop\wrestling

    2-6. ASP 설정

<img src="images/18_ASP_설정.jpg" alt="img18" width="51%" height="auto">
<img src="images/19_ASP_설정.jpg" alt="img19" width="41%" height="auto">

---

### 기타 설정
<img src="images/19_ASP_설정.jpg" alt="img19" width="41%" height="auto">
C:\Users\5N\Desktop\wrestling\default.asp
