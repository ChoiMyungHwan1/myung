# Git hub

# git 명령어
## 전역 설정 정보 조회

git config - -global - -list

## 전역 설정 정보 삭제시키기

git config --global --unset-all user.email

git config --global --unset-all user.name

## 새로운 저장소 초기화하기

git init

## 저장소 복제하기

git clone <저장소 url>

## 새로운 원격 저장소 추가하기

git remote add <원격 저장소> <저장소 url>

## 새로운 파일 git에 등록시키기(staging)

git add <파일>

## 현재까지 작업한 내용 저장하기

git commit -m “<메시지>”

## 원격 저장소에서 합치지 않고 지역 브랜치로 변경 사항 가져오기

git fetch <원격 저장소>

## 원격 저장소에서 변경 사항을 가져와 현재 브랜치에 합치기

git pull <원격 저장소>

## 새로운 로컬 브랜치를 원격 저장소에 푸싱하기

git push <원격 저장소> <지역 브랜치>

-------------------------------------------------------------------------------------------------------------
### 제목 Headers #으로 시작하는 텍스트다. #은 하나부터 여섯새까지 쓸 수있고, #이늘어날때마다 제목의 수준은 내려간다.
# 아아
## 아아아
### 아아아아
#### 아정말?
---------------------
>으로 시작하는 텍스트
마크다운 >인용문  실행결과 : 인용문

코드 블럭 ```` 혹은 ~~~  코드 첫 줄과 마지막 줄에 Back quote ( ` ) 또는 물결( ~ ) 3개 삽입

실행을 시켜보면
```
코드블럭
입니다
```
~~~
코드블럭
이다.
~~~

```c
void f()
  printf(%s,"이것은 c코드 입니다");
  }
  ```
  
  인라인 코드! 
  마크다운: `인라인 코드 블럭` 실행결과: 인라인 코드 블럭
  
  강조 Emphasis
  기울여쓰기 : *또는 _로 감싼 텍스트
  굵게 쓰기 : **또는 __로 감싼 텍스트
  
  수평선 -또는 *또는 _을 3개 이상 작성
  (단, -을 사용할 경우 header로 인식할 수 있으니 이 전 라인은 비워두어야한다.)
  
 # 링크 Links
  외부링크
   [링크](http://example.com "링크 제목") 인라인 링크
   
   [링크1][1] [1]: http://example1.com/ "링크제목1" 참조 링크
   
   <example.com/> <example@example.com> url 링크
   
  ## 마크다운	/ 실행결과
   
인라인 링크

[Google](http://www.google.co.kr “구글” / Google

참조 링크 
[Google][1]                           /  Google

[Naver][2]                            / Naver

[1]: http://google.com/ “구글”

[2]: http://naver.com/ “네이버”


URl 링크
<http://google.com/>         / http://google.com
<example@gmail.com/>         / example@gmail.com

내부 링크 Internal (Anchored) Links
[링크](#id) 내부 링크

마크다운 / 실행결과

[목차](#index) / 목차

# 리스트 Lists

순서 있는 리스트 Ordered Lists

No. 숫자 다음 .을 찍는다. (적힌 숫자랑 상관없이 순서대로 번호가 매겨진다.)

## 마크다운 / 실행결과

1. list item 1 / 1.list item 1

1. list item 2 / 2.list itme 2

2. list item 3 / 3.list item 3

0. list item 4 / 4.list item 4

3. list item 5 / 5.list item 5

# 순서 없는 리스트 Unordered Lists

*,+,- 으로 시작

## 마크다운 / 실행결과

*list item 1  / ● list item1

  *list item 1-1 / ○ list item 1-1

  *list item 1-2 / ○ list item 1-2

--------------------------------------

+list item1 / ● list item 1

  +list item 1-1 / ○ list item 1-1
  
  +list item 1-2 / ○ list item 1-2
  
--------------------------------------

-list item 1 / ● list item 1
  
  -list item 1-1 / ○ list item 1-1
 
  -list item 1-2 / ○ list item 1-2

--------------------------------------

# 테이블 Tables

## 마크다운  /  실행결과

### 테이블 생성

Header 1 | Header 2          /       Header1  Header2

---------|----------          /     

Content1 | Content 3           /     Content1  Content3

Content2 | Content4                 Content2 Content4

### 테이블정렬

| Header 1 | Header 2 | Header 3 |          /// Header1  Header2  Header3

| :-------- | :--------: | --------: |      /// Left Center Right

| Left | Center | Right |

----------------------------------------

# 이미지 Adding Images!!

## 마크다운    //  실행결과

---------------------------------------

인라인 이미지
![alt text](/test.png )

링크 이미지
![alt text](image_URL)

참조 이미지
![alt text][1]
[1]: /test.png

----------------------------------------

# 각주 Footnotes

각주입니다[^!d]

[^id]: 각주에 대한 설명

GitHub에서는 footnote를 지원해주지 않는다.

## #Blog #Markdown

< 이전 포스트 [Markdown] title 대괄호[] 사용하기
 
