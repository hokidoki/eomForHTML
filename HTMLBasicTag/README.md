# HTML tag basic

## h1~h6 tag

h1 ~ h6 요소는 6단계의 구획 제목을 나타낸다. 구획단계는 h1이 가장 높고 h6이 가장 낮다.

## b tag

b태그는 글자를 굵게표시하는 태그로, bold의 약자이다. 독자의 주의를 요소의 콘텐츠로 끌기 위한용도

`<strong></strong>`태그도 같은 기능을 하며 최신 표준은 `<b>` 태그 보다는 `<strong>` 태그를 권고하고있다.

CSS에서 [`font-weight`](https://ofcourse.kr/css-course/font-속성#font-weight)을 `bold`으로 설정하는 것과 같은 효과를 나타낸다.

* `b` vs `strong`
  * `b`태그는 단순히 텍스트를 진하게 표시하는 역할만 존재하나,`strong`태그는 실제로 페이지 내의 중요한 부분으로 브라우저에게 알려주는 역할을 한다. 이는 브라우저에서 지원되는 웹 접근성에 큰 기여를 한다.

## i tag

글자를 기울여서 표시하는 태그로, italic의 약자이다. CSS에서 `font-style`을 `italic`으로 설정하는 것과 같은효과를 나타닙니다.

```html
<i>기울여서 표시 할 내용</i>
```

**출력 결과**

*italic content* normal content

* `i` vs `em`
  * b와 strong 차이만큼 `em` 태그를 사용하면 실질적 강조를 하는 효과가 있다.

## a tag

(앵커요소) 다른 콘텐트와 연결되는 하이퍼링크를 정의한다. 

* 속성

  * **href**: 클릭시 이동 할 링크

  ```html
  <a href="http://www.naver.com">Go NAVER</a>
  ```

  * **target**  : 링크를 클릭 할 대 창을 어떻게 열지 설정한다.

    - `_self`: 현재 페이지 (기본값)
    - `_blank`: 새 탭
    - `_parent`: 부모 창에서 연다. (부모 창이 없으면 _self 속성으로 처리)
    - `_top`: 전체 브라우저 창에서 가장 상위의 창에서 연다. (부모 창이 없으면 _self 속성으로 처리)
    - *`프레임이름`*: 직접 프레임이름을 명시해서 사용할 수도 있다.

  * **title**: 해당 링크에 마우스 커서를 올릴때 도움말 설명을 설정한다. 

    

## p tag

`paragraph` 로 하나의 문단을 나타낸다.

```html
<p>문단1</p>
```

## span tag

구문 컨텐트를 위한 통용 인라인 컨테이너, 아무것도 나타내지 않으나 스타일을 적용하기 위해서, 어떤 특성값을 서로 공유하는 요소를 묶을때 사용한다.

div 태그와의 차이점은 `display` 속성이 `block`이 아닌 `inline` 이라는 점이다. 즉 `<div>` 태그는 줄 바꿈이 되지만, `<span>` 태그는 줄 바꿈이 되지 않는다.

```html
<span>내용</span>
```

## label tag

폼의 양식에 이름 붙이는 태그이다. = `input` 태그의 의미를 정의하기 위한 태그이다.

속성으로는 `for`를 가지고 있다. 이곳에 설명하고싶은 input 태그의 id값을 지정해 주어야 한다. 즉 input 태그에 id값이 있어야 하며 해당 id값을label태그의 for 속성에 넣어주면 된다.

```html
<label for="description">설명 : </label>
<input type="text" id="description" name="description">
```

- `<label>` 태그사이에 위치한 `text`, `checkbox`, `radio` 등은 클릭 가능 영역이 텍스트로 확장된다.

#### for 쓰지 않고 label 사용법

`<label>` 태그를 `<input>` 태그 바깥에 사용하면, `for` 속성을 사용하지 않을 수 있다.

```html
<label>
  <input type="checkbox" name="eom">
</label>
```

------------

reference

* https://developer.mozilla.org/ko/docs/Web/HTML/Element
* https://ofcourse.kr/html-course
* https://electronic-moongchi.tistory.com/87 : a tag
* https://dasima.xyz/html-label/ : label tag