# Django 를 이용한 웹개발 

## 개발 환경 
* ubuntu: 16.04LTS
* python-version: 3.6.6
* Django: 2.1.1 

## ch3
* 파이썬 웹프로그래밍(개정판) 실습  

### HTML 기초 : element, attribute 소개 
* HTML 은 "<" 로 시작해서 ">"로 끝나는 태그를 통해 작성 
    - '열리는 태그', '닫히는 태그'로 이루어진 태그  ex> <tag\>ABC </tag\>
    - '스스로 닫는 태그'  ex> <br /\>, <img /\>
<br/>
    
    
* 기본적인 HTML 태그 구조는 html, head, title, body 의 구조를 가진다. 
    - html : 눈에 보이는 한 페이지를 가르키는 영역 
    - head: 각종 설정을 포함하는 정보
    - title: 인터넷 익스플로러 탭에 나타나는 제목 
    - body: 실제 홈페이지의 내용을 작성하는 영역 
<br/>
    
    
* <img src="http://www.naver.com/sample.png" alt="샘플 이미지" /\>
    - img: "태그" 이자, "element(요소)"
    - src, alt: attribute(속성)
    - 태그의 구성
        - <요소 속성="속성값" /\> 
        - <요소 속성="속성값"\> 내용 </요소\>
<br/>


* html: id, class, name 속성의 차이 

| id  | class | name |
|:---:|:---:|:---:|
| 하나의 요소만 가능(페이지 유일) | 여러 요소 적용 가능 | 여러 요소 적용 가능 |
| CSS에서 식별자로 사용 가능 | CSS에서 식별자로 사용 가능 | CSS에서 사용 불가(같은 이름이 여러개 존재 가능)|
| jQuery: \$("#아이디") | jQuery: \$(".클래스명") | jQuery: \$("input[name=이름]")|



* id, class 간 차이 
    - CSS 측면에서 상단, 컨텐츠, 하단 으로 나눌 경우 페이지 내에서 하나씩 존재 > id 
    - 게시물 추출 내용에 CSS 부여하고 싶을 경우 > class 
<br/>
   
   
* CSS(Cascading Style Sheets)란? 
    - HTML, XHTML, XML 같은 문서의 스타일을 꾸밀 때 사용하는 스타일 시트 언어 
    - HTML 로 문서의 뼈대를 만들면 CSS는 이를 꾸미는 역할을 한다 
        ex) 글꼴, 배경색, 너비, 높이, 위치 등을 지정하거나, 웹 브라우저, 스크린 크기, 장치에 따라 화면이 다르게 표현하는 등 
    - CSS 장점 
        - HTML을 통해 문서의 뼈대도 만들고 꾸밈을 만들 경우, 모든 문서를 하나씩 수정해야 함 
        - CSS는 문서의 내용(contents)와 표현(presentation)을 분리하여, CSS 파일 하나만 수정하면 스타일에 해당하는 HTML 문서가 한번에 수정되는 장점 
        
| HTML 작성 | CSS 작성 |
|:---:|:---:|
|<태그 속성="속성값"\> 내용 </태그\> <br/> ex) <p align="center"\> 내용 </p\> | 선택자 {속성:속성값; 속성:속성값;} <br/> ex) p{text-align:center; color:red;} |
<br/>


* span, div 
    - <span\>: 문자열 중 원하는 부분만 선택(inline)해서 시각적 효과 부여 <br/>
        ex) <span id="이름"\> 내용 </span\> 
    - <div\>: 하나 이상의 요소(태그)를 묶어서(block) 스타일 부여  <br/> 
        참고: http://aboooks.tistory.com/63 
<br/>


* inline element, block element 
    - inline element: 줄 속에 끼워 넣는 요소 <br/> 
        활용: <span\>, <a\>, <b\>, <img\> 등 
    - block element: 묶음요소 <br/> 
        활용: <div\>, <p\>, <ol\>, <ul\>, <table\> 등 
            



## myproject  
* Djangogirls 실습 