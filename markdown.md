마크업(makrup): 문서를 작정하는 언어
문서 작성을 구조와 서식을 태그로 지정하여 사용하는 언어
웹 문서 작성에 많이 사용(HTML)

마크업 예시: \<h1>제목\</h1>

마크다운(markdown): 타 마크업 언어보다 간단한 문법을 제공하는 경량 마크업 언어.

간결하고 직관적인 문법, HTML로 호환 가능, 개발자가 많이 사용함

단점
구조화된 문서를 작성하기 어려움, 표준이 없음

Header 헤더: 문서의 제목을 표시할 때 사용  
'#'으로 제목의 중요성을 표시함.  
'#'가장 중요한 제목,  '######' 가장 덜 중요한 제목  

# 가장 중요한 제목
## 두번쨰로 중요한 제목
###### 가장 덜 중요한 제목

h1 제목
===
h2 제목
---

# 가로 구분선
'-' 또는 '*' 또는 '_'를 3개 이상으로 작성
'---'은 h2제목으로 인식을 할 수 있기 때문에 바로 윗칸은 비워야 함
---

***

___
***

# 줄바꿈
기본적으로 마크다운은 문서에서 줄바꿈을 하더라도 인식하지 않음
공백 문자 두개 혹은 '<br>'이라는 태그로 줄바꿈 처리

첫번째 줄  
두번째 줄<br>
세번째 줄

# 문자열 강조
이텔릭체: '*' 혹은 '_'로 텍스트를 감싸줌.
보더체: '**' 혹은 '__'fh 텍스트를 감싸줌.
취소선: '~~'로 텍스트를 감싸줌

이 문장은 *이텔릭체*를 테스트  
이 문장은 **보더체**를 테스트  
이 문장은 ~~취소선~~을 테스트  
*이 문장은 **중첩** ~~테스트~~*

# 인용문
'>'로 텍스트를 시작함
'>' 3개까지 중첩하여 사용 가능

링컨이 이야기했습니다.
> 인민의, 인민에 의한, 인민을 위한 정부는  
> > 이 땅에서 사라지지 않는다.  

# 리스트 표현
## 순서가 없는 리스트
'*', '-', '+'를 텍스트 앞에 붙여서 사용 가능
들여쓰기를 농하여 깊이를 조정 가능

* 사과  
    * apple
    * 포도
* 바나나
- 딸기

## 순서가 존재하는 리스트
숫자. 을 텍스트 앞에 붙여서 지정가능  
들여쓰기를 사용하여 깊이 조정 가능

1. 첫번째
    1. 1-1

2. 두번째
    - 요소 1  
    - 요소 2  

# 특수 문자 표현
특수 문자를 표현하고자 한다면 \를 앞에 붙임

\* 별표 표현

# 코드 블럭
'```' 혹은 '~~~'로 코드를 감싸 표현
'```' 뒤에 해당 코드의 언어를 지정하여 하이라이트 가능

```java
public static void main(String[] args) {}
```

```bash
pip install matplotlib
```

# 테이블
헤더, 로우를 구분해서 작성할 수 있음  
각 필드의 구분은 '|'으로 구분  
헤더와 로우는 '---'로 구분

이름|나이|주소
---|---|---
홍길동|30|부산
김철수|20|서울

# 이미지
'\!\[설명](이미지경로)'로 이미지
표현 가능  

![고양이](https://i.namu.wiki/i/0o7fWfiVJ8wFx7tsI7rA7JkHQcZNYNrj3uM8f7At0paBR6nVEnc9vBjXPYv8PfzRmfwlcs2_8WHAyQlvnIhI_CKykgooBXXCujx35JyDAPizvGjTcJ1CGoyo9BWpLWT3k95Uf8EHi2oRTXY3mCo4mw.webp) 

<img src="https://i.namu.wiki/i/0o7fWfiVJ8wFx7tsI7rA7JkHQcZNYNrj3uM8f7At0paBR6nVEnc9vBjXPYv8PfzRmfwlcs2_8WHAyQlvnIhI_CKykgooBXXCujx35JyDAPizvGjTcJ1CGoyo9BWpLWT3k95Uf8EHi2oRTXY3mCo4mw.webp" height='200px' width='200px'>

# 링크
## 외부 링크
'\[링크이름](주소)'로 링크 지정 가능

[구글](https://google.com)  
https://google.com

## 내부 링크
'\[링크이름](헤더)'로 내부 링크 지정 가능

[1 - 줄바꿈](#줄바꿈)

## 이미지에 링크 적용
'\[이미지형태](주소)'로 이미지에 링크 적용 가능

[![고양이2](https://i.namu.wiki/i/8vscVp_fuPphr1eZ99zaOog5v2oMNHdUSTzglW8HavIEyjKuEr7wl6e3cESVq-ouvLpBZ516oG9KOIFPakL_fUuQagMyQ3oYTR4QqG0HiGomnucvMuF57RQIfceJbvL-buzi6c-Qcm9rckxHrDMkPA.webp)](#줄바꿈)

# HTML 혼용
마크다운에 HTML 사용 가능

# 제목을 입력했습니다.
<h1 style="background-color:black; color: white;"> 제목을 입력했습니다. </h1>
