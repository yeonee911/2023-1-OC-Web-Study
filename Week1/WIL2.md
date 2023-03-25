##HTML/CSS/JS

**HTML ((Hyper Text Markup Language))**
- 웹 문서를 만들기 위하여 사용하는 기본적인 웹 언어의 한 종류
- 웹 페이지에서 제목, 이미지, 동영상, 문단, 표, 등을 정의하고 그 구조와 의미를 부여하는 정적 언어
- 웹의 구조를 담당
- 사람 신체의 뼈, 신체 구조(키, 몸무게, 근육 등)

**CSS (Cascading Style Sheets)**
- 마크업 언어(HTML, XML, XHML 등)가 실제 표시되는 방법(색상, 레이아웃, 크기, 폰트 등)을 지정하여 콘텐츠 구조를 꾸며주는 정적 언어
- 웹의 시각적인 표현을 담당
- 사람의 겉모습(외모와 의상, 액세서리 등)

**JS : 제어(JavaScript)**
- 콘텐츠를 바꾸고 움직이는 등 페이지를 동적으로 꾸며주는 역할을 하는 프로그래밍 언어
- 웹의 동적 처리를 담당한다.
- 사람이 행동하는 알고리즘(어떤 외부 자극에 대한 반응, 행동의 범위 등)

***

##git 영역
1. Working Directory : 개인 코드 작성
2. Staging Area : git add를 통해서 수정된 코드를 올리는 영역
3. Repository : git commit을 통해서 최종 수정본을 제출

**git add** : git이 추적하고 있는 수정된 파일이 working directory에서 staging area에 저장
**git commit** : Local Repository에 변화한 부분을 저장
**git push** : Local Repository의 커밋(git commit)된 내용을 원격 저장소(Remote Repository)로 내보냄
<br>
####_ **git fetch vs git push**
**git fetch** : 원격 저장소에 변경사항이 있는지 확인만 하고, 변경된 데이터를 로컬 git에 실제로 가져오지는 않음

**git pull** : 원격 저장소에서 변경사항을 확인할 뿐만 아니라 최신 데이터를 복사하여 로컬 git에 가져옴(병합)

_참고 : fetch 후 pull을 사용하는 게 좋다!_