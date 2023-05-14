<h4>유튜브 aside-container를 클론해봤다!</h4>

**느낀점**
1. 오타 하나 때문에 몇 백 줄 뒤져가면서 오류를 찾았다. 영문자 오타 하나 내면 너무 힘들어진다..
2. 괄호를 잘 닫아줘야한다. 제대로 닫아줘야 다음 요소에 영향을 미치지 않는다. 이것 때문에 "대체 왜 css가 적용이 안되는 거야?!" 많이 그랬다.
3. 확실히 직접 해봐야 외워지는 것 같다. flex-direction이니 뭐니.. 뭐든 실전을 겪어봐야 하는 듯!
4. 직접 어떻게 박스를 나눌 것인지 생각해보는 게 또 나름 재미있었다.
5. 미적 감각이 좀 필요한 작업인 것 같다.
6. 유튜브 썸네일 따오는 법을 알아냈다!
> https://img.youtube.com/ + id + /mqdefault.jpg
7. 시작했을 땐 너무 막막했는데, 한번 감을 잡으니까 금방 했다. 무엇보다 완성하나까 너무 뿌듯하다!

---

**직접 추가해 본 css**
.aside-container {
  display: flex;
  flex-direction: column;
}
>

.aside-container-thumbnail {
  width: 192px;
  height: 108px;
  margin: 3px;
  <mark>border-radius: 10px;
  cursor: pointer;</mark>
}

>border-radius 속성 : 둥근 모서리
>cursor 속성 : 해당 태그 위에 위치하는 마우스 커서의 모양을 바꿀 수 있다.
>- auto : 자동
>- default : 기본값(화살표)
>- pointer : 손가락 모양(클릭 가능한 버튼)
>- wait : 로딩

.aside-container-information {
  display: flex;
  flex-direction: column;
  <mark>align-items: flex-start;</mark>
  cursor: pointer;
}
>align-items: flex-start; 영상 제목을 썸네일과 맞춰서 위에서부터 시작하고 싶었음

.#aside-video {
  display: flex;
  flex-direction: row;
}

---
**CSS에서 #과 .의 차이점?**
클래스 선택자 : '.'
ID 선택자 : '#'

_**클래스 선택자와 ID 선택자는 어떨 때 써야 할까?**_
여러 번 반복될 필요가 있는 스타일은 클래스 선택자를 사용하는 것이 좋다. 하지만 한번만 적용될 스타일은 ID 선택자를 이용하는 것이 좋다.

>보통 폰트크기, 색상 등 추후 다른 곳에 적용될 수 있는 스타일 지정시 클래스 지정자를 사용하면 되고, ID선택자는 주로 HTML내에서 요소의 배치 방법 지정 등에 사용하게 된다.