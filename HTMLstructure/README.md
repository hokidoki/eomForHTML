# HTML Structure

### HTML Header Information 

HTML파일의 헤더에는 브라우저에서 랜더링 되지 않는 여러 개의 HTML요소들을 포함 할 수 있다. 이러한 요소는 페이지에 대한 정보르 설명하는 메타데이터 이거나 `CSS` 스타일시트 또는 `Javascript` 파일과 같은 외부 리소스에서 정보를 가져오는데 사용되는섹션을 포함한다.  페이지의 헤더는 `head`태그로 표현된다.

* 메타데이터는 <title>, <style>, <meta>, <link>, <script>, <base>태그 등을 이용하여 표현할 수 있습니다.

페이지 제목을 설정하려면, title 태그로 표현 할 수 있다. 

* HTML 문서의 제목(title)을 정의하며, 다음과 같은 용도로 사용된다.

  - 웹 브라우저의 툴바(toolbar)에 표시된다.

  - 웹 브라우저의 즐겨찾기(favorites)에 추가할 때 즐겨찾기의 제목.

  - 검색 엔진의 결과 페이지에 제목으로 표시된다.

### HTML Body Information 

Body는 브라우저에 의해 렌더링 되는 파일의 모든 내용을 포함하는 파일의 기본 섹션 이다. html `body` 는 여러모양의 태그로 이루어진 블럭을 참조하는 마크업이 포함묄 수 있다.여기에는 텍스트, 이미지, 색상, 그래픽 등과 같은 여러 유형의 정보가 포함될 수 있고, 오디오 및 비디오 요소는 브라우저에서 렌더링하기 위해 html 본문에 포함될 수도 있다. 시각적 표현을 위한 최신 스타일 시트 응용 프로그램이 있는 경우(CSS) 배경색, 링크 색상, 텍스트 색상 등과 같은 BODY의 표시 속성은 사용하지 않는다.

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN"
   "http://www.w3.org/TR/html4/strict.dtd">
<HTML>
<HEAD>
 <TITLE>Inline Style Sheets referencing</TITLE>
 <STYLE type#"text/css">
 </STYLE>
</HEAD>
<BODY>
  ... document body...
</BODY>
</HTML>
```

--------

### 참고한 곳

##### https://docs.fileformat.com/web/html/





