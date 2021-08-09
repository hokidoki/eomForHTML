# input tag

HTML `input` 태그는 웹 기반양식에서 사용자의 데이터를 받을 수 있는 태그 이다. `form` 태그안에서 가장 중요한(most important) 역할을 하는 요소입니다. 타입 속성에 따라서 다양한 방식으로 제공된다. 

## input type attributes

#### text 

기본값, 한 줄의  텍스트 입력 칸을 만든다. (기본 너비 문자는 20이다.)

#### button

누를 수 있는 기본 버튼을 만든다. `value ` 속성을 이용해 value 값을 보여 줄 수 있다. 기본 값은 비어있다.

#### checkbox

단일 값을 선택, 선택 해제 할수 있는 체크박스를 만든다.

활성화 되면  체크 표시(✔)가 나타나는 사각형 모양의 박스 모양 이다.

체크박스는 사용자가 여러 선택사항 중에서 하나 이상의 값을 선택 할 수 있게 해준다.

#### radio 

라디오 버튼을 만든다. 동일한 이름값을 가진 여러 항목들 중에 단일값을 선택 할 수 있다.

서로 연관된 옵션들의 집합을 보통 하나의 라디오 버튼 그룹으로 나타내며, 그룹 내의 라디오 버튼은 오직하나만 선택이 가능하다. 

#### color ![html5](http://tcpschool.com/lectures/html5_logo_s.png)

색상을 선택한다. 색상 선택기(color picker)를 연다.

입력의 기본값은 #000000으로 검정색을 나타내며 반드시 문자 # 로 시작하는 총 7자리 16진수 값이 와야 한다.

> 인터넷 익스플로어 미지원

#### date![html5](http://tcpschool.com/lectures/html5_logo_s.png)

날짜 입력을 위한 입력 상자를 만든다. 년 월 일에 대한 날짜 선택기(date picker) 혹은 숫자 휠을 연다.

입력 결과에는 년도, 월, 일이 포함되나 시간은 포함되지 않는다.

>  사파리 ,인터넷 익스플로어 미지원

#### datetime-local![html5](http://tcpschool.com/lectures/html5_logo_s.png)

날짜 및 시간을 입력합니다. 결과값으로 연도 월일 및 시간이 포함된다.

> 파이어 폭스, 사파리, 인터넷 익스플로어 미지원

#### email ![html5](http://tcpschool.com/lectures/html5_logo_s.png)

이메일 주소를 입력하기 위한 입력창을 만든다. `text` 타입과 비슷하게 생겼지만 입력값이 올바른 이메일 주소인지 자동으로 확인한다.  

multiple 속성을 명시해 여러개의 이메일 주소를 입력받을 수 있다.

#### month![html5](http://tcpschool.com/lectures/html5_logo_s.png)

시간대 없이 월과 연도를 입력하기위한 필드를 생성. "YYYY -MM" 포멧을 사용힙니다. 

> 파이어 폭스, 사파리, 인터넷 익스플로어 미지원

#### number

숫자를 입력하는 창을 만든다. 허용되는 숫자에 대한 제한을 설정 할 수도 있다.

*  아래의 속성을 이용하여 숫자제한을 설정 할 수있다.
  * `max` : 최댓값을 지정한다.
  * `min` : 촤솟값을 지정한다.
  * `step` :  입력 할 수 있는 숫자들 사이의 간격을 명시한다.(기본값 1)
  * `value` : 입력창의 기본값을 설정한다

#### password

비밀번호 입력 창을 만든다. (문자는 마스킹되어 구분이 불가능하다.)

#### range![html5](http://tcpschool.com/lectures/html5_logo_s.png)

정확하지 않는 숫자의 입력을 위한 입력창을 만든다. (슬라이드 컨트롤)

기본값으로 범위는 0에서 100 사이의 값을 가지고 있다. 다만 아래의 속성들을 이용하여 입력값의 범위를 지정 할 수 있다.

* `max` : 입력창에 허용되는 값의 최댓값을 지정한다.
* `min` : 입력창에 허용되는 값의 촤솟값을 지정한다. 
* `step` :  입력 할 수 있는 숫자들 사이의 간격을 명시한다.(기본값 1)
* `value` : 입력창의 기본값을 설정한다

 #### search![html5](http://tcpschool.com/lectures/html5_logo_s.png)

검색어를 입력 할 수있는 입력창을 만든다. `text`타입과 기능적으로는 완전히 똑같지만 브라우저에 의해 다르게 표현 될 수 있다. `serch` 타입엔 `name` 속성을 설정 해야하며 `name` 속성의 설정 되어있지 않으면 서버로 제출 되지 않는다. 

가장 흔한 `search` `name` 값은 `q`이다. (`name = p`)

#### submit

제출 버튼을 만든다.  서버의 폼 핸들러로 폼 데이터를 전송하는 제출 버튼을 만든다. 

#### reset

`form`요소에 입력되어있는 값들을 초기값으로 되돌리는 초기화 버튼을 생성한다. 

#### file

파일 입력을 위한 필드와, 파일 선택을 할수 있는 "찾아보기" 버튼을 생성한다. 여러 파일을 선택 할 수 있는 파일 선택 필드를 정의하려면 다중 속성을 추가해야한다. 

#### hidden

숨겨진 입력 필드를 생성합니다. `hidden` 필드를 사용하면 웹 개발자가 양식을 제출할 대 사용자가 보거나 수정할 수 없는 데이터를 포함 할 수 있다. 

양식을 제출할 때 업데이트 해야하는 데이터베이스 레코드를 저장하는 경우가 많다.

브라우저의 소스보기로 확인할 수 있으므로 입력 보안의 한 형태로 사용하면 안된다.

#### image

이미지 제출 버튼을 생성하는 버튼을 생성합니다. 이미지의 경로는 `src` 속성에 지정된다.

#### time![html5](http://tcpschool.com/lectures/html5_logo_s.png)

시간을 입력하는 입력창을 생성한다. (타임존 없음)

자동으로 입력 내용을 검증하는 텍스트 필드를 통해 시간을 직접 입력하거나, 시간을 선택할 수 있는 time picker를 사용하여 시간을 입력할 수 있다. time 과 minute 이 포함되며 오전/오후를 반드시 선택해야만 입력 유효성을 통과 할 수 있다.

* `time`을 24시간으로 변환하기 위해 `jquery` `timepicker `  library 등을 이용해야 한다. 

> 사파리 미 지원, 인터넷 익스플로어 11 에서 지원이 된다.

#### URL(Uniform Resource Locator) ![html5](http://tcpschool.com/lectures/html5_logo_s.png)

인터넷 주소를 입력하는 입력창을 생성한다.  입력창은 데이터를 제출하기 전 입력된 값이 유요한 URL 주소인지 여부를 자동으로 검출한다. 

#### tel![html5](http://tcpschool.com/lectures/html5_logo_s.png)

전화번호를 입력하는 입력창을 만든다. `tel` 을 지원하지않는 브라우저는 `text` 입력으로 대체된다.

> 현재 크롬, 엣지 10.0 up to 10 version, fire fox, safari , opera  up to11.0 version 브라우저에서는 지원이 된다

#### week![html5](http://tcpschool.com/lectures/html5_logo_s.png)

주차와 년도를 입력받는 입력창을 만든다. (타임존없음)

> 파이어 폭스, 사파리 미지원

------

## input other attributes

#### accept 

서버로 업로드할 수 있는 파일의 타입을 명시한다. `accept`속성에 하나이상의 속성값을 명시할 경우에는 콤마(.)를 사용하여 구분한다. 

문법 = `file 확장자 (ex: .jpg,.doc...)` , `audio/*`,`vedio/*`,`image/*`,`media type: 파라미터를 가지지 않는 유요한 미디어 타입`

type : `file`

#### alt

이미지를 위한 대체 텍스트를 명시한다. 사용자의 느린 네트워크 환경이나 `src` 속성값의 오류, 시각장애인용 스크린 리더 사용등 어떤 이유로든 사용자가 이미 지를 볼 수 없을때 대시 제공할 대체 정보를 제공한다. 

문법 =  "텍스트"

type : `image`

#### autocomplete

사용자에게 input 요소에서 자동완성 기능을 사용할지 여부를 명시한다. 속성값을 `on` 으로 명시하면 , 브라우저는 사용자가 이전에 입력했던 값을들 기반으로 사용자가 입력한 값과 비슷한 값들을 드롭다운 옵션으로 보여준다.

문법 = `on` , `off`

type : `color` `datepickers` `email` `password` `search` `tel` `text` `hidden` `number` `range`

#### autofocus

페이지가 로드 될 때 자동으로 포커스가 input 요소로 이동됨을 명시한다. 문서 내 `autofocus` 속성을 가질 수 있는 요소는 하나만 있을 수 있다. 2개 이상 존재할 시 가장 첫 번째 선언된 속성만 적용된다. 

페이지가 스크롤이 된체 로딩이 된다거나 터치 디바이스에선 키보드 액션이 나올 수 있습니다.

속성은 불리언속성이다. 불리언 속성은 해당 속성을 명시하지 않으면 자동으로 false값을 가지며 명시하면 true값을 가지게 된다.

문법 `autofocus`

#### checked

페이지가 로드될 때 미리 선택될 요소를 명시한다. 페이지가 로드된 후에도 자바스크립트를 사용하여 설정 할 수 있다. 

속성은 불리언속성이다. 불리언 속성은 해당 속성을 명시하지 않으면 자동으로 false값을 가지며 명시하면 true값을 가지게 된다.

`radio` 버튼에서 `checked` 활성시 속해있는 그룹중 하나의 버튼이 선택되어 있음을 뜻합니다.

`check box` 버튼에서 `checked` 활성시 기본적으로 선택되어 있음을 나타낸다. 

`check box` 버튼이 선택되어 있는지 여부를 나타내지 않기 때문에 `checked` 속성의 `check box`가 값이 변하더라도 변경사항을 반영하지 않는다.

문법 `checked`

type : `radio` `checkbox`

#### disabled

존재하는경우 사용자가 입력과 상호작용흘 할수 없어야함을 나타내는 속성이다.

명시된 input 요소는 사용할 수 없으며, 사용자가 클릭 할 수도 없다. 또한 폼 데이터가 제출될 때도 disabled 속성이 명시된 input 데이터는 제출되지 않는다.

속성은 불리언속성이다. 불리언 속성은 해당 속성을 명시하지 않으면 자동으로 false값을 가지며 명시하면 true값을 가지게 된다.

문법 `disabled`

type : `every type of input tag`

#### maxlength

input 요소에 입력할 수 있는 최대 문자 수를 명시한다. 반드시 0보다 큰 수를 입력해야 한다. 

문법 ="숫자"

type : `text` `search` `url` `tel` `email` `password`

#### multiple

input요소에 둘 이상의 값을 입력할 수 있음을 명시한다. 콤마(,)를 추가하여 이메일 주소를 동시에 입력하거나, file의 경우 CTRL , SHIFT 키를 사용하여 여러개의 파일을 동시에 선택할 수 있다.

속성은 불리언속성이다. 불리언 속성은 해당 속성을 명시하지 않으면 자동으로 false값을 가지며 명시하면 true값을 가지게 된다.

문법 `mulitple`

type : `file`,`email`

#### name

input 이름을 명시한다. name 속성은 폼이제출된 후 서버에서 폼 데이터를 참조하기 위해 사용되거나 자바스트립트에서 요소를 참조하기 위해 사용된다.

input에 name이 지정되지 않았거나 name이 비어있으면 input값이 폼과 함께 제출되지 않는다.

* 역사적인 이유로 `isindex` 로 name을 지을 수 없습니다.

문법 ="텍스트"

type : `every type of input tag`

#### pattern

폼 제출 시 입력값을 검사할 때 사용될 정규 표현식을 명시한다. 이때 title 속성을 이요하여 정규 표현식에 간단한 설명을추가함으로써 사용자가 정확한 값을 입력할 수 있도록 도움을 줄 수 있다.

문법 = "정규 표현식"

* https://neomania.tistory.com/3 : input pattern 정규 표현식 모음

```html
1. 숫자만
<input type="text" name="patternValue" pattern="\d*"> 
<input type="text" name="patternValue" pattern="^[0-9]+$">
2. 영문 대소문자만
<input type="text" name="patternValue" pattern="^[a-zA-Z]+$">
3. 영문 대소문자만, 띄어쓰기 및 공백 가능
<input type="text" name="patternValue" pattern="^[a-zA-Z\s]+$">
4. 숫자, 영문 대소문자만
<input type="text" name="patternValue" pattern="^[a-zA-Z0-9]+$">
5. 최소 8자리에서 최대 16자리까지 숫자, 영문, 특수문자 각 1개이상 포함(암호 유효성 검사 유용)
<input type="text" name="patternValue" pattern="^(?=.*[A-Za-z])(?=.*\d)(?=.*[$@$!%*#?&])[A-Za-z\d$@$!%*#?&]{8,16}$">

```

type : `date` `email` `password` `search` `tel` `text` `url`

#### placeholder

입력 필드에 사용자가 적절한 값을 입력할 수 있도록 도와주는 짧은 도움말을 명시한다. 이러한 도움말은 사용자가 입력하기 전까지 입력 필드에 표시되다가 사용자가 입력을 시작하면 사라진다.

문법 = "텍스트"

type : `email` `password` `search` `tel` `text` `URL`

#### readonly

입력 태그가 읽기전용 속성임을 명시한다. 사용자가 수정할수 없지만 해당 내용을 하이라이트 하거나 복사할 수는 있다. 따라서 이속성을 사용하면 특정 조건이 충족될 때 까지 사용자가 입력필드의 내용을 수정할 수 없도록 설정하고, 특정 조건이 충족되면 자바 스크립트 등으로 readonly 속성을 삭제하여 사용자가 입력 필드를 수정할 수 있도록 조절할 수 있다.

* disabled 와 readonly  : disabled 속성의 입력값은 서버로 제출되지 않지만, readonly 속성의 입력값은 서버로 제출된다. 

속성은 불리언속성이다. 불리언 속성은 해당 속성을 명시하지 않으면 자동으로 false값을 가지며 명시하면 true값을 가지게 된다.

문법 `readonly`

type : `text` `search` `url` `tel` `email` `date` `month` `week` `time` `datetime-local` `number`

#### required

폼 데이터가 서버로 제출되지 전 반드시 체워져 있어야 하는 입력 필드를 명시한다. 

속성은 불리언속성이다. 불리언 속성은 해당 속성을 명시하지 않으면 자동으로 false값을 가지며 명시하면 true값을 가지게 된다.

문법 `required`

type : `text` `search` `url` `tel` `email` `date` `month` `week` `time` `datetime-local` `number` `password` `checkbox` `radio` `file`

#### size

input 요소의 너비를 문자수 단위로 명시한다.  기본값은 20

문법 = "숫자"

type : `text` `tel` `email` `password` `url` `search`

#### src

이미지 제출 버튼을 나타내기 위해 표시할 이미지 파일의 URL을 지정하는 문자열이다. 반드시 명시해야하는 속성이다.

문법 ="URL"

type : `image` 

#### value

input 의  초기값을 정의한다. 자바스크립트를 사용하여 언제든지 변경하거나 검색하여 해당 개채의 value 프로퍼티에 엑세스 할 수 있다. 

 value 속성은 <input> 요소의 type 속성값에 따라 다른 용도로 사용된다.

* “button”, “reset”, “submit” : 버튼 내의 텍스트를 정의함.

* “hidden”, “password”, “text” : 입력 필드의 초깃값을 정의함.

* “checkbox”, “image”, “radio” : 해당 입력 필드를 선택 시 서버로 제출되는 값을 정의함.

문법 = "텍스트"

type : `button` `reset` `submit` `hidden` `password` `text` `checkbox` `image` `radio`

------

#### 문제의 인터넷 익스플로어 11 호환 :mask:

2013년도에 마지막버전인 11 버전이 나온 뒤 부터 인터넷 익스플로어는 발전하지 못하고 있기 때문에 13년도 이후에 나온 태그를 사용 할 수 없다. -> 자바스크립트 라이브러리를 이용하여 구현 해야한다.

* URL
* color
* time
* date, datetime-local, week, month 

인터넷 익스플로어에서 지원되지 않는 타입을 사용하면 업/다운 화살표나 캘린더,컬러 피커등이 지원되지 않으며 일반 텍스트 필드로 출력된다.

-------------

references

* https://developer.mozilla.org/ko/docs/Web/HTML/Element/input
* https://www.w3schools.com/tags/tag_input.asp
* http://tcpschool.com/html-tag-attrs/input-type
* https://blogpack.tistory.com/86 : 태그 고급속성, 잘 사용되지 않는것들.. :x:

* https://jin-na.tistory.com/entry/%ED%95%B4%EC%99%B8%EB%B2%88%EC%97%AD-%EB%9D%BC%EB%94%94%EC%98%A4-%EB%B2%84%ED%8A%BC%EA%B3%BC-%EC%B2%B4%ED%81%AC%EB%B0%95%EC%8A%A4%EA%B0%80-%EA%B3%B5%EC%A1%B4%ED%95%A0-%EC%88%98-%EC%97%86%EB%8A%94-%EC%9D%B4%EC%9C%A0 : 라디오 버튼과 체크박스가 공존할 수 없는 이유.