# HTML

# HTML

**Hyper Text Markup Language**

- 웹 페이지를 만드는 언어
- Hyper Text(링크)
- Markup Language
- 확장자가 html

# HTML 문법

## 태그

`<태그이름>내용</태그이름>`  → 전체를 ‘요소’ 라고 부른다. 태그와 요소는 으레 동일한 의미로 표현하기도 한다. 

## 속성

`<h1 id="title">Hello, HTML</h1>`

- 속성이름: id
- 속성 값: title
- 속성: 태그 이름 뒤에 `속성이름=”속성 값”` 사용. `=` 은 붙여서 사용
- 하나의 태그에도 여러 속성을 사용할 수 있다. 속성의 선언 순서는 상관없다.
    
    `<h1 id=”title” class=”test”>Hello, HTML</h1>`
    

## 태그의 중첩

**올바른 예**

`<h1>Hello, <i>HTML</i></h1>`

**잘못된 예**

`<h1>Hello, <i>HTML</h1></i>`

## 빈 태그

태그 중에 쌍으로 이뤄지지 않는 태그들. 종료 태그가 존재하지 않아 내용을 그 사이에 쓸 수 없음.

속성을 통해서 화면에 나타나게 할 수 있거나 다른 기능을 수행.

- `<br>`
- `<img src="">` : 이미지를 삽입하는 태그. 이미지의 경로를 src 속성을 활용해서 전달.
- `<input type="">`

## 공백

HTML은 기본적으로 두 칸 이상의 공백을 모두 무시한다.

```html
<h1>Hello, HTML</h1>
<h1>Hello,     HTML</h1>
<h1>
    Hello,
    HTML
</h1>
```

모두 같은 결과.

## 주석

화면에 노출되지 않고 메모의 목적

```html
<!-- 주석처리 되는 내용 -->
<!-- 여러줄로
작성할 수도 있다.
-->
```

## 문서의 기본구조

```html
<!DOCTYPE html>
<html lang="ko">
    <head>
        <meta charset="UTF-8">
        <title>HTML 문서의 기본구조</title>
    </head>
    <body>
        <h1>Hello HTML</h1>
    </body>
</html>
```

- `<!DOCTYPE>`
    - 이 문서가 어떤 버전으로 작성되었는지 브라우저에 알려주는 것
    - 문서의 최상단에 위치해야 한다.
- `<html>`
    - 문서 타입 선언 후에는 `<html>` 태그가 나와야 하고, 자식으로는 <head> 태그와 <body> 태그가 있다.
    - lang 속성은 문서가 어느 언어로 작성돼 있는지 의미
- `<head>`
    - `<title> </title>` : 문서의 제목을 표현하는 태그. 탭 바에 나타난다.
    - `<meta>` : charset 속성은 문자의 인코딩 방식을 지정
- `<body>`
    
    실제 브라우저 화면에 나타나는 내용이 들어가며, 앞으로 다루는 태그들 대부분이 모두 여기에 해당