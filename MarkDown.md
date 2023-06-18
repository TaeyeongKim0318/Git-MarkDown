# 마크다운 문법 정리(MarkDown Syntax)
[![참고 링크](./Img/MarkDownImg.png)](https://goddaehee.tistory.com/307)<br>
>##### 참고 출처 : 갓대희의 작은공간(이미지 클릭시 해당 링크로 이동)
<br>
<br>

## 1. 제목 (Header) `<h1>` ~ `<h6>`
 - `#` 뒤에 띄어쓰기를 넣어주는게 권장하는 방법 이다.
 - `<h1>` ~ `<h6>` 까지 표현 가능하다.
```
# 제목1
## 제목 2
### 제목 3
#### 제목 4
##### 제목 5
###### 제목 6
```
# 제목1
## 제목 2
### 제목 3
#### 제목 4
##### 제목 5
###### 제목 6
<br>
<br>

## 2. 줄바꿈 (Line Breaks) `<br>`
- 띄어쓰기 2번 또는 `<br>`로 표현 가능 하다.
```
# 줄바꿈(Line Breaks) 
띄어쓰기 2번  
또는 <br/>
```
![2. 줄바꿈](Img/2.%20%EC%A4%84%EB%B0%94%EA%BF%88.png)
<br>
<br>

## 3. 수평선 (Horizontal Rule) `<hr>`
 - 가시적으로 페이지를 나누는 용도로 많이 사용된다.
```
---
***
___
******
```
![3. 수평선](Img/3.%20%EC%88%98%ED%8F%89%EC%84%A0.png)
<br>
<br>

## 4. 글자 강조 (Emphasis)
```
**굵은 글씨**  
*이텔릭*  
_이탤릭_  
~~취소선~~  
<u>밑줄</u>  
ex)  
This is the **bold** text and this is the *italic* text and <u>let's</u> do ~~strikethrough~~
```
![4. 글자 강조](Img/4.%20%EA%B8%80%EC%9E%90%20%EA%B0%95%EC%A1%B0.png)
<br>
<br>

## 5. 인용문 (BlockQuote) `>`
- ">" 블럭 인용 문자를 사용하면 인용문 표현이 가능하다.
```
> 인용문장
>> 중첩된 인용문
>>> 중첩된 인용문 2
```
![5. 인용문](Img/5.%20%EC%9D%B8%EC%9A%A9%EB%AC%B8.png)
<br>
<br>

## 6. 목록 (List)
### 1) 순서가 없는 목록 (*, +, -)
```
- 순서가 필요하지 않은 목록
    - 순서가 필요하지 않은 목록
        - 순서가 필요하지 않은 목록
* 순서가 필요하지 않은 목록
    * 순서가 필요하지 않은 목록
        * 순서가 필요하지 않은 목록
+ 순서가 필요하지 않은 목록
    + 순서가 필요하지 않은 목록
        + 순서가 필요하지 않은 목록

- 순서가 필요하지 않은 목록
    * 순서가 필요하지 않은 목록
    + 순서가 필요하지 않은 목록
```
![6-1. 순서가 없는 목록](Img/6.%20%EB%AA%A9%EB%A1%9D(%EC%88%9C%EC%84%9C%EC%97%86%EB%8A%94).png)
<br>

### 2) 순서가 있는 목록
```
1. 순서가 필요한 목록
    1. 순서가 필요한 목록
    1. 순서가 필요한 목록
1. 순서가 필요한 목록


1. 순서가 필요한 목록
    9. 순서가 필요한 목록
    3. 순서가 필요한 목록
8. 순서가 필요한 목록
```
![6-2. 순서가 있는 목록](Img/6.%20%EB%AA%A9%EB%A1%9D(%EC%88%9C%EC%84%9C%EC%9E%88%EB%8A%94).png)
<br>

### 3) 혼합 사용하는 예시
```
- 순서가 필요하지 않은 목록
    1. 순서가 필요한 목록
    1. 순서가 필요한 목록
- 순서가 필요하지 않은 목록2
    1. 순서가 필요한 목록
    3. 순서가 필요한 목록
    8. 순서가 필요한 목록
```
![6-3. 혼합 사용하는 예시](Img/6.%20%EB%AA%A9%EB%A1%9D(%EC%88%9C%EC%84%9C%ED%98%BC%ED%95%A9).png)
<br>
<br>

## 7. 링크 (Links)
### 1) 기본방법
`[<Title>](<link>)`

```
Click [here](http://goddaehee.tistory.com/)  
[갓대희의 작은 공간](https://goddaehee.tistory.com)
```
![7-1. 기본방법](Img/7.%20%EB%A7%81%ED%81%AC(%EA%B8%B0%EB%B3%B8).png)
<br>

### 2) 참조 링크 사용 방법
`[<Link Keyword>][<id>]`<br>
`[<id>]: <URL> <Optional Title> `
#### (1) title 옵션 없이 사용
```
[갓대희의 작은 공간][gdh]
[gdh]: https://goddaehee.tistory.com
```
![7-1-1. 참조 링크 사용 방법](Img/7.%20%EB%A7%81%ED%81%AC(%EC%B0%B8%EC%A1%B0%EB%A7%81%ED%81%AC1).png)
<br>

#### (2) title 옵션 사용시 커서를 링크 위로 위치하면, title이 노출 된다.
```
[갓대희의 작은 공간][gdh]
[gdh]: https://goddaehee.tistory.com "Click here"
```
![7-1-2. title 옵션 사용시 커서를 링크 위로 위치하면, title이 노출 된다.](Img/7.%20%EB%A7%81%ED%81%AC(%EC%B0%B8%EC%A1%B0%EB%A7%81%ED%81%AC2).png)
<br>

### 3) 자동 링크 사용 방법
  - 인터넷 URL 혹은 이메일 주소를 적합한 형식으로 링크를 생성해준다.
```
https://goddaehee.tistory.com
goddaehee@kakao.com
```
https://goddaehee.tistory.com<br>
goddaehee@kakao.com
<br>
<br>

## 8. 이미지 (Images)
  - Link와 문법이 유사하다. 앞에 `!`만 추가하면 된다.
### 1) 기본 문법
`![<대체 텍스트>](<이미지 주소>)`
```
![Image Description](https://tistory1.daumcdn.net/tistory/1994430/74cb0667c02241939c5c13ec5dd1afb1)
```
![8-1. 기본 문법](Img/8.%20%EC%9D%B4%EB%AF%B8%EC%A7%80(%EA%B8%B0%EB%B3%B8).png)
<br>

### 2) 참조 링크 사용 방법
`:[<대체 텍스트>][<id>]`<br>
`[<id>]: <이미지 주소> <Optional Title>`
```
![Image Description](gdh)
[gdh]:https://tistory1.daumcdn.net/tistory/1994430/74cb0667c02241939c5c13ec5dd1afb1
```
![8-2. 참조 링크 사용 방법](Img/8.%20%EC%9D%B4%EB%AF%B8%EC%A7%80(%EC%B0%B8%EC%A1%B0).png)
<br>

### 3) 이미지 노출과 동시에 링크 처리
`[![<대체 텍스트>](<이미지 주소>)](<링크 주소>)`
```
[![Image Description](https://tistory1.daumcdn.net/tistory/1994430/74cb0667c02241939c5c13ec5dd1afb1)](http://goddaehee.tistory.com)
```
![8-3. 이미지 노출과 동시에 링크 처리](Img/8.%20%EC%9D%B4%EB%AF%B8%EC%A7%80(%EC%9D%B4%EB%AF%B8%EC%A7%80%26%EB%A7%81%ED%81%AC).png)
<br>
<br>

## 9. 표 (Table)
 - `|` (vertical bar) 기호를 통해 테이블을 표현 가능. (가장 좌측, 우측 생략 가능)
 - 헤더와 셀을 구분할 때 3개 이상의 `-` (하이픈, 대시)가 필요 하다.
 - `:` (콜론) 기호를 통해 정렬할 수 있다.
```
| Header | value | Description |
| --: | :-- | :--: |
| 정렬 | --: | 우측정렬 |
| 정렬 | :-- | 좌측정렬 |
| 정렬 | :--: | 가운데정렬 |
```
![9. 표](Img/9.%20%ED%91%9C.png)
<br>
<br>

## 10. 코드 (Code)
### 1) 인라인 코드 (Inline Code)
- `` (백틱) 기호로 강조할 내용을 감싸면 된다.
```
`해당 코드`는 강조할 부분 이다.
```
![10. 코드](Img/10.%20%EC%BD%94%EB%93%9C1.png )
<br>

### 2) 블럭 코드 (Block Code)
- html, css, javascript, bash, plaintext 등등
#### (1) 코드의 종류를 명시 하지 않은 경우
![2-1) 코드의 종류를 명시 하지 않은 경우](Img/10.%20%EC%BD%94%EB%93%9C2.png )
#### (2) HTML
![2-2) HTML](Img/10.%20%EC%BD%94%EB%93%9C3.png)
#### (3) CSS
![2-3) CSS](Img/10.%20%EC%BD%94%EB%93%9C4.png )
#### (4) JavaScript
![2-4) JavaScript](Img/10.%20%EC%BD%94%EB%93%9C5.png )
#### (5) Bash
![2-5) Bash](Img/10.%20%EC%BD%94%EB%93%9C6.png)
#### (6) 이 외 텍스트
![2-6) 이 외 텍스트](Img/10.%20%EC%BD%94%EB%93%9C7.png )
#### (7) 정리
| 언어 | Markdown | 언어 | Markdown |
| :--: | :--: | :--: | :--: |
| **Bash** | bash | **JSON** | json |
| **C#** | cs | **Java** | java |
| **C++** | cpp | **JavaScript** | javascript |
| **CSS** | css | **PHP** | php |
| **Diff** | diff | **Perl** | perl |
| **HTML, XML** | html | **Python** | python |
| **HTTP** | http | **Ruby** | ruby |
| **Ini** | ini | **SQL** | sql |
<br>
<br>

## 11. 원시 HTML (Raw HTML)
 - MarkDown 환경에서는 결국 표현의 한계가 있고, 이런 경우 순수 html문법을 사용할 수 있다.
### 1) image를 표현할 때 MarkDown으로는 width 지정이 불가능 하다.
```<img width="70" src="" alt="gods" />```
### 2) 링크를 표현할 때 target="_blank" 지정이 불가능 하다.
### 3) 밑줄을 표현할 수 없어 <u></u>를 사용하거나 다음과 같이 style을 직접 지정 해줘야 한다.
```<span style="text-decoration: underline;">갓대희</span> 티스토리 입니다.```
