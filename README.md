#웹의 흐름

웹의 흐름을 알기전에

-웹브라우저란?

  웹 서버에서 이동하며 쌍방향으로 통신하고 HTML 문서나 파일을 출력하는 소프트웨어

-URL이란?

  네트워크 상에서 자원이 어디 있는지를 알려주기 위한 규약으로 흔히 웹 주소 또는 인터넷 주소라고도 불리며 URI의 한 유형으로 리소스의 위치와 엑세스에 사용되는 프로토콜을 나타낸다. 

통신 프로토콜(communication protocol)

  -네트워크 상의 서버로 부터 웹 문서 정보(html)와 이미지 등의 리소스를 받아올 통신 방식을 미리 정해 놓은 것으로 HTTP, HTTPS, FTP, FILE, MAILTO 등이 있다.

호스트 (Host Name)

  -네트워크에 연결된 장치 또는 서버들에 부여되는 고유한 이름으로 호스트 명은 IP 주소나 MAC 주소와 같은 기계적인 이름을 대신하여 일반인이 쉽게 읽고 이해할 수 있는 이름으로 만들어진다.

3차 도메인 (third-level domain)

  -리소스가 네트워크(인터넷)상에 위치하는 물리적 위치로 Namespace 계층 상에서 최종 호스트 명을 포함하는 도메인 명을 뜻하는 FQDN(Fully Qualified Domain Name)이라고도 하며, 2차 도    메인에 WWW와 같이 호스트 명를 부가한 3차 도메인 또는 서브 도메인 이라고도 한다.

2차 도메인 (second-level domain) 

  -일반적으로 도메인 둥록/구매처에서 등록하여 사용하는 도메인을 가리키며 서브 도메인에 대응하여 메인 도메인(또는 zone apex/root domain/naked domain/bare domain)으로 불리기도 하    며,3차 도메인과 혼용하여 부르기도 한다.

최상위 도메인 (top-level domain)

  -인터넷에서 도메인 네임의 가장 마지막 부분으로 특정한 조직 계열에 따라 사용되는 도메인이다. com, net, org, edu, gov, mil등의 일반 최상위 도메인(gTLD)와 co.kr, kr과 같은 국가      코드 최상위 도메인(ccTLD)이 있다.

포트 번호 (port number)

  -포트 번호는 네트워크 또는 인터넷을 사용하여 통신하는 각 응용 프로그램 또는 프로세스의 논리 주소로 0에서 65,535번 까지 포트 번호를 사용한다. HTTP가 기본 포트인 80번으로 설정된      경우, 80번은 생략될 수 있다.

디렉터리 (directory)

  -해당 파일(또는 자원)이 서버의 어디에 있는지를 나타내는 경로로서 초기의 웹에서는 웹 서버상에서 물리적 파일 위치를 의미하였으나, 최근에는, 실제 물리적 경로를 나타내지 않고, 웹 서    버에서 추상화하여 보여줍니다.

파일 (file)

  -월드 와이드 웹 상에서 연결 할 실제 파일의 이름으로 HTML(또는 XHTML), CSS 문서, 자바스크립트, 이미지, 문서,동영상 등의 파일을 가리킵니다,

파일 형식 (file format)

  -일반적으로 사용하는 웹 프로그래밍 언어에 따라 달라지며
   HTML, CGI, PHP, JSP, ASP 등이 사용됩니다.

쿼리 스트링 (Query String)

  -웹 서버에 제공하는 추가 파라미터로 이 파라미터들은 & 기호로 구분된 키/값으로 짝을 이룬 일련의 쿼리 리스트들로 이루어져 있습니다.

#웹의 흐름 순서

1.사용자가 웹브라우저를 통해 찾고 싶은 웹 페이지의 URL 주소를 입력

2.사용자가 입력한 URL 주소 중에서 도메인 네임(DOMAIN NAME) 부분을 DNS 서버에서 검색

3.DNS 서버에서 해당 도메인 네임에 해당하는 IP 주소를 찾아 사용자가 입력한 URL 정보와 함께 전달

4.웹 페이지 URL 정보와 전달받은 IP 주소는 HTTP 프로토콜을 사용하여 요청 메시지 생성

  -이렇게 생성된 HTTP 요청 메시지는 TCP 프로토콜을 사용하여 인터넷을 거쳐 해당 IP 주소의 컴퓨터로 전송된다

5.도착한 HTTP 요청 메시지는 HTTP 프로토콜을 사용하여 웹 페이지 URL 정보로 변환된다.

6.이렇게 도착한 HTTP 요청 메시지는 HTTP 프로토콜을 사용하여 웹 페이지 URL 정보로 변환된다.

7.웹 서버는 도착한 웹 페이지 URL 정보에 해당하는 데이터를 검색

8.검색된 웹 페이지 데이터는 또 다시 HTTP 프로토콜을 사용하여 HTTP 응답 메시지를 생성
  
  -이렇게 생성된 HTTP 응답 메시지는 TCP 프로토콜을 사용하여 인터넷을 거쳐 원래 컴퓨터로 전송함

9.도착한 HTTP 응답 메시지는 HTTP 프로토콜을 사용하여 웹 페이지 데이터로 변환

10.변환된 웹 페이지 데이터는 웹 브라우저에 의해 출력되어 사용자가 볼 수 있게 된다.

