# HTML TABLE

`table` 태그는 데이터를 포함하는 셀들의 행과 열로 구성된 2차원테이블을 정의 할 때 사용한다. 

이러한 테이블은 `table`요소와 자식요소인 하나의 `td` ,`tr` ,`th` 요소들로 구성된다. + `caption `

* tr (table row) : 가로줄을 만드는 역할, 기본값으로 굵은 글씨체, 중앙정렬
* th (table head) : 표의 제목을 쓰는 역할, 보통 글씨체, 왼쪽 정렬
* td (table data) : cell 을 만드는 역할 , 보통 글씨체, 왼쪽 정렬
* caption : 테이블의 제목이나 설명을 작성하는태그, 태이블의 가로폭의 가운데로 오는것이 기본값이다.

## Atributes

### table tag attributes

#### border 

* 테이블이 갖고 있는 테이블과 셀 모두에 선처리를 한다.

#### bordercolor 

* 테부리의 색상을 지정한다.

#### width

* 테이블의 너비를 설정한다.

#### height

* 테이블의 높이를 설정한다.

#### cellpadding

* 셀과 컨텐츠 간의 간격 조절(셀의 안쪽 여백)

#### cellspacing

* 셀과 셀간의 간격 조절 (셀의 바깥쪽 여백)

#### bgcolor 

* 테이블의 배경색을 명시한다.

------

### 셀 병합 속성

#### colspan : column span 

같은 행의 칸들을 병합 할 때 사용한다. `<td colspan = "칸수">`

#### rowspan : row span

다른 행의 칸들을 병합 할 때 사용한다.`<td rowspan = "칸수">`



> 병합..? td를 병합한 갯수만큼지워주지 않으면 밀려나게 된다?

-----

### 셀 태그 속성

#### width

* 셀의 너비(가로폭)를 설정한다.

#### height

* 셀의 높이(세로폭)를 설정한다.

#### allign

* 셀의 컨텐츠를 가로 정렬 시켜주는 속성 : `left`, `right`, `center`

#### valign

* 셀의 컨텐츠를 세로 정렬 시켜주는 속성 : `top` , `middle`, `bottom`

-----

### HTML 5 테이블 행그룹 태그

#### thead 

테이블의 제목들을 묶는 태그

#### tbody 

테이블의 일반적 데이터들을 묶는 그룹태그

#### tfoot 

테이블의 마지막 아래부분을 묶는 그룹태그

위의 태그들을 묶는 이유는 css에서 사용하기 편리하게 되기 때문이다.

![](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbxguwK%2FbtqEbQkXPiW%2FXI7UnWe1gsEfp8XbK8gk2k%2Fimg.jpg)

-----

#### HTML5에서 변경된 사항

HTML5에서는 `<table>` 태그의 align, bgcolor, border, cellpadding, cellspacing, frame, rules, summary, width 속성을 더 이상 지원하지 않습니다.

-----

references

> https://ossam5.tistory.com/69
>
> 