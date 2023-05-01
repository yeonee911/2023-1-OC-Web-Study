<h1>HTML5</h1>

<b>정의</b>
- 웹페이지를 기술하기 위한 마크업 언어
- 웹페이지의 내용(content)과 구조(structure)을 담당하는 언어
- HTML 태그를 통해 정보를 구조화

<b>HTML 기본구조</b>
HTML5 문서는 반드시 <!DOCTYPE html>으로 시작
-> 문서 형식(document type)을 HTML5로 지정

실제적인 HTML document은 2행부터 시작, <html>과 </html> 사이에 기술한다.

<head>와 </head> 사이 : document title, 외부 파일의 참조, 메타데이터의 설정 등이 위치, 브라우저에 표시X

<body>와 </body> 사이 : 웹브라우저에 출력되는 모든 요소

<br><b>HTML5의 기본 문법</b>

1.요소
:시작태그 - 콘텐츠 - 종료태그 

1.1 요소의 중첩
- 요소는 다른 요소를 포함할 수 있다.
- 시각적으로 파악하기 쉽게 들여쓰기 활용

1.2 빈 요소
:content를 가질 수 없는 요소
br
hr
img
input
link
meta

<b>어트리뷰트</b>
:요소의 성질, 특징을 정의하는 명세
- 요소에 추가적 정보(예: 이미지 파일의 경로, 크기 등)를 제공
- 어트리뷰트는 시작 태그에 위치해야 하며 이름과 값의 쌍을 이룬다. (e.g. name=”value”)

<b>주석</b>
:개발자에게 코드를 설명하기 위해 사용, 브라우저는 주석을 화면에 표시X

<hr>

<b>시맨틱 요소와 검색 엔진</b>
<b>크롤링</b> : 검색엔진이 로봇(Robot)이라는 프로그램을 이용해 전세계의 웹사이트 정보를 수집
<b>인덱싱</b> : 검색 사이트 이용자가 검색할 만한 키워드를 예상하여 검색 키워드에 대응하는 인덱스를 만들어 두는 것
<b>시맨틱 태그</b> : 브라우저, 검색엔진, 개발자 모두에게 콘텐츠의 의미를 명확히 설명
<b>non-semantic 요소</b> : 이들 태그는 content에 대하여 어떤 설명도 X
<b>sementic 요소</b> : 이들 태그는 content의 의미를 명확히 설명

=> 크롤링 - 시맨틱 요소를 해석 - 인덱싱
<br>

<b>텍스트 관련 태그</b>
- <i>b vs strong</i>
b : bold체를 지정, 의미론적(Semantic) 중요성의 의미X
strong : bold체를 지정, 의미론적(Semantic) 중요성의 의미O
<br>
- <i>i vs em</i>
i : Italic체를 지정, 의미론적(Semantic) 중요성의 의미X
em : emphasized(강조, 중요한) text를 지정, Italic체로 표현, 의미론적(Semantic) 중요성의 의미O

<hr>

<h1>CSS</h1>
<b>정의</b>
<br>: HTML의 각 요소(Element)의 style(design, layout etc)을 정의하여 화면(Screen) 등에 어떻게 렌더링하면 되는지 브라우저에게 설명하기 위한 언어

<br><b>셀렉터(Selector, 선택자)</b>
:스타일을 적용하고자 하는 HTML 요소를 선택하기 위해   CSS에서 제공하는 수단

<b>스타일시트(Style Sheet)</b> 
:Rule Set의 집합

<b>프로퍼티(Property / 속성)</b>
- 셀렉터로 HTML 요소를 선택하고 {} 내에 프로퍼티(속성)와 값을 지정하는 것으로 다양한 style을 정의
- 프로퍼티는 표준 스펙으로 이미 지정되어 있는 것을 사용하여야하며 사용자가 임의로 정의할 수 없다. 
- 여러 개의 프로퍼티를 연속해서 지정할 수 있으며 세미콜론(;)으로 구분

<b>값(Value / 속성값)</b>
:프로퍼티의 값은 해당 프로퍼티에 사용할 수 있는 값을 “키워드”나 “크기 단위” 또는 “색상 표현 단위” 등의 특정 단위로 지정
크기 단위 : px(절댓값), em(상대값), %(상대값)
색상 표현 단위 : 사용이 간편하나 ㅎ=표현할 수 있는 색상의 수 제한

<hr>

Box
: 콘텐트(Content) < 패팅(Padding) < 테두리(Border) < 마진(Margin)

Content 
: 요소의 텍스트나 이미지 등의 실제 내용이 위치하는 영역. 
- width, height 프로퍼티를 갖는다.

Padding 
: 테두리(Border) 안쪽에 위치하는 요소의 내부 여백 영역
- padding 프로퍼티 값 : 패딩 영역의 두께
- 기본색은 투명(transparent)
- 요소에 적용된 배경의 컬러, 이미지는 패딩 영역까지 적용

Border 
: 테두리 영역. 
-border 프로퍼티 값 : 테두리의 두께

Margin 
: 테두리(Border) 바깥에 위치하는 요소의 외부 여백 영역
- margin 프로퍼티 값 : 마진 영역의 두께
- 기본적으로 투명(transparent), 배경색을 지정할 수 없다.

<b>폰트와 텍스트</b>
font-size 프로퍼티 : 텍스트 크기 정의
font-family 프로퍼티 : 폰트 지정
font-style 프로퍼티 : 이탤릭체의 지정
font-weight 프로퍼티 : 폰트 굵기 지정
line-height 프로퍼티 : 텍스트의 높이 지정
letter-spacing 프로퍼티 : 글자 사이의 간격 지정
text-align 프로퍼티 : 텍스트의 수평 정렬 정의

<b>요소의 위치 정의</b>
position 프로퍼티 : 요소의 위치 정의
static (기본위치) : position 프로퍼티의 기본값. 좌표 프로퍼티와 같이 사용할 수 없다.
relative (상대위치) : 기본 위치를 기준으로 좌표 프로퍼티를 사용하여 위치를 이동시킨다.
absolute (절대 위치) : 부모 요소 또는 가장 가까이 있는 조상 요소(static 제외)를 기준으로 좌표 프로퍼티(top, bottom, left, right)만큼 이동한다. 즉, relative, absolute, fixed 프로퍼티가 선언되어 있는 부모 또는 조상 요소를 기준으로 위치가 결정된다.
만일 부모 또는 조상 요소가 static인 경우, document body를 기준으로 하여 좌표 프로퍼티대로 위치하게 된다.

<br>

<b><i>relative 프로퍼티 vs absolute 프로퍼티</i></b>

relative 프로퍼티 
: 기본 위치(static으로 지정되었을 때의 위치)를 기준으로 좌표 프로퍼티(top, bottom, left, right)을 사용하여 위치를 이동
-> 따라서 무조건 부모를 기준으로 위치하게 된다.

absolute 프로퍼티
: 부모에 static 이외의 position 프로퍼티가 지정되어 있을 경우에만 부모를 기준으로 위치. 만일 부모, 조상이 모두 static 프로퍼티인 경우, document body를 기준으로 위치
-> 따라서 absolute 프로퍼티 요소는 부모 요소의 영역을 벗어나 자유롭게 어디든지 위치할 수 있다.

<br>
fixed (고정위치) : 부모 요소와 관계없이 브라우저의 viewport를 기준으로 좌표프로퍼티(top, bottom, left, right)을 사용하여 위치를 이동시킨다. 스크롤이 되더라도 화면에서 사라지지 않고 항상 같은 곳에 위치한다.