# html

## 월드 와이드 웹

web :  인터넷에 연결되어 있는 컴퓨터들이 정보를 주고받는 공간

get(주세요) <->ok

post(처리해주세요)<->ok



user >>>>>> program

​	request

​	<<<<<<<

​	response



우리는 서버컴퓨터에서 요청과 응답을 처리할 프로그램을 개발한다.





서버컴퓨터 : 서버 역할을 위해 필요한 프로그램만 깔려 있다.

클라이언트 사용량에 맞는 성능을 가진다.

보안에 있어 공격대상이 되기 쉽다.

절대 꺼지지도, 인터넷 연결이 끊겨서도 안된다.



## html : 

하이퍼 링크를 통해서 텍스트 간 이동이 가능함

htper text 전송 프로토콜 : http

웹페이지를 작성하기 위한 역할 표시 언어 : html

html파일 : html로 작성된 문서파일



### static web 정적인 웹

아무것도 없는 컴퓨터에 하나만 설치해야 한다면? : 브라우저(크롬)

직접 주소창에 지정하여서 가져오는 도서관같은 웹

단, https://ahndogeon.github.io/ 뒤에 아무것도 안붙이면 정확히 'index.html' 이라고 디폴트값 주어져서 그 파일에 접근하게 한다. ---- 인덱스 페이지



### Dynamic web : web application program(web app)









모든 컴퓨터에서 서버에 달라고 하는 법 : URI(i)

URL(Uniform Resource Locator)은 네트워크 상에서 자원이 어디 있는지를 알려주기 위한 고유 규약이다.

흔히 웹사이트 주소로 알고 있지만 url은 웹사이트 주소뿐만 아니라 컴퓨터 네트워크 상의 자원을 모두 나타낼 수 있다.





## html

https://validator.w3.org/ 여기서 다이렉트 인풋에서 복붙 -> 파이썬 튜터같이 html 파일 검사해주는 곳



```html
<!DOCTYPE html> # 선언해주는 것, 지금부터 시작한다!
<html lang="en"> # html은 트리구조 en 대신 ko넣으면 시각장애인분들을 위한 읽어주는 트리거
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>AhnDogeon's github page</title>
</head>
<body> # 이 안의 내용들이 사람들한테 보여지는 내용
    <h1>Comming Soon..</h1>
</body>
</html>
```

`<h1>내용</h1> 여는 태그 닫는 태그 -----> 태그 + 내용 : 요소 (element)`

혼자 열리고 혼자 닫히는게 있음

`<img src="./animals/animal.jpg" alt="daram"/>`

속성(attribute) :  ~~ = ~~ : attribute 는 이것 속성명은 따옴표 없고 속성값은 따옴표 있다!

`<li>HTML</li>` 엘러먼트의 태그는 li이고 컨텐트는 html이고 attribute는 없습니다

h1, img, ul은 형제 자매관계이고 body와 부모자식 관계

div 들 : 요즘은 이름에 명시해줌

header : 헤더

nav : 네비게이션 바

aside : 좌측우측 사이드

footer: 하단에 있는 것

등등 div가 아니라 태그 이름만 봐도 이 문서에서 무슨 역할하는지 알 수 있게 됨 html5에서



크롬에서 web developer 

informatino에서 view document outline



html 글자 두껍게 하기

`<b></b>` 그냥 두껍게만 하는 것

`<strong></strong>` 이게 요즘 강조하는 것

`<i></i>` :

`<em></em>` 기울이기

`<blockquote></blockquote>`: 인용구 블럭

<ol> 순서가 있는 리스트
## 190114 요약정리



```html
<!DOCTYPE html>
<html lang="ko">
    <head>
        <meta charset="UTF-8">
        <title>Learn HTML</title>
        <style>
            table, tr, td {
                border: 1px solid darkgray;  # 한 줄 한 줄 스타일 입혀주지말고 맨 위에 style 로 전역으로 해줌
            }
        
        </style>
    </head>

    <body>
        <h1>프로그래밍 교육</h1>
        <a href="https://ko.wikipedia.org/wiki/%ED%8C%8C%EC%9D%B4%EC%8D%AC" target="_blank"> # 클릭하면 특정 url로 이동 또는 target="_blank"로 다른 창 띄우기
            <img src="./images/python.png" alt="python" width="50px" height="50px"> # src 다음 이미지가 있는 폴더주소나 이미지 자체 url로 이미지 삽입 가능, alt 다음은 이름인데 웬만하면 넣는게 좋음
        </a>
        <a href="https://ko.wikipedia.org/wiki/HTML5" target="_blank">
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/220px-HTML5_logo_and_wordmark.svg.png" alt="html5" width="50px" height="50px">
            <hr /> # 한 줄 긋는거
        </a>
        <section> # 파트나누는거
            <h2>
                <a href="https://docs.python.org" target="_blank">
                    Python
                </a>
            </h2>
            <h3>Number Type</h3>
            <p>파이썬에서 숫자형은 아래와 같다</p>  # 문자열 삽입
            <ol> # 순서가 있는 것.
                <li>int</li> # li*4 탭 이렇게 연속 네 개 만들 수 있다. 리스트!
                <li>float</li>
                <li>complex</li>
                <li>str</li>
            </ol>

            <h3>Sequence</h3>
            <p>파이썬에서 시퀀스는 아래와 같다</p>
            <strong>시퀀스는 for문을 돌릴 수 있다!</strong> # 강조
            <ol>
                <li>str</li>
                <li>lits</li>
                <li>tuple</li>
                <li>range</li>
            </ol>
        </section>
        <section>
            <h2>
                <a href="https://developer.mozilla.org" target="_blank">
                    Web
                </a>
            </h2>
            
            <h3>Basic</h3>
            <ul> # 순서 없는거 un order list
                <li>HTML</li>
                <li>CSS</li>
            </ul>
        </section>
        <iframe width="800" height="760" src="https://www.youtube.com/embed/_hsrsmwHv0A" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> # iframe으로 동영상 삽입 가능
        <table> # 테이블로 표 만들기
            <thead>
                <td>점심메뉴</td> # 표 제목
            </thead>
            <tr> tr : row
                <th></th> : 표 제일 첫 째줄에 있는 정보들
                <th>월</th>
                <th>화</th>
                <th>수</th>

            </tr>
            <tr>
                <td>특식</td> #  table data
                <td>초밥</td>
                <td>바베큐</td>
                <td>삼겹살</td>
            </tr>
            <tr>
                <td>한식</td>
                <td>육개장</td>
                <td>미역국</td>
                <td>삼계탕</td>
            </tr>
        </table>

        <hr>8887ㅠ8
        <h3>TimeTable</h3>
        <table>
            <tr>
                <th>TIME</th>
                <th>INDOOR</th>
                <th colspan="2">OUTDOOR</th> #colspan : col 행 빈칸 2칸 늘려줌
            </tr>
            <tr>
                <td></td>
                <td>소극장</td>
                <td>잔디마당</td>
                <td>대공연장</td>
            </tr>
            <tr>
                <td>10:00</td>
                <td rowspan="2">안녕하신가영</td> row 열 빈칸 2칸 늘려줌
                <td></td>
                <td>10cm</td>
            </tr>
            <tr>
                <td>13:00</td>
                <td rowspan="2">선우정아</td>
                <td rowspan="2">참깨와 솜사탕</td>
            </tr>
            <tr>
                <td>15:00</td>
                <td></td>
            </tr>
            <tr>
                <td>17:00</td>
                <td rowspan="2">크러쉬</td>
                <td></td>
                <td rowspan="2">폴킴</td>
            </tr>
        </table>
    
    </body>
</html>
```








