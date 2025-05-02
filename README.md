노마드코더 코코아클론 학습을 위한 프로젝트입니다.

집-회사-노트북 프로젝트 공유를 위해 사용

=배운 내용 요약 정리=

1. 태그 a 는 양커를 뜻한다
2. 태그에 부가적인 정보를 주는걸 속성이라 한다
3. \_blank 는 새창에서 연다-->
4. 이미지 태그는 닫아주는 태그가 없다
5. src 태그는 hi에서 동작안함
6. body는 콘텐츠를 보여주는곳이고 head는 페이지에 대한 환경설정을 하는곳이다
7. 브라우져안에 보여질 내용은 전부 body 태그 안에 있어야한다.
8. meta 태그는 부가적인 정보를 표현할때 사용한다.
9. 태그 검색할때 Mdn을 붙여서 검색하면 좋다
10. w3School을 사용하면 안되는 이유 : MDN are the ones that create the standards, MDN is non profit, W3C has commercial interests + the source of W3C is MDN :)
11. 옆에 다른요소가 올수있으면 inline, 없으면 block
12. 인라인은 높이와 넓이를 가질수 없다
13. margine은 box 경계로부터 바깥에 있는 공간이다
14.      margin: 20px 15px 12px 9px; 이러면 시계방향 순으로 적용(위 오 아래 왼)
15.      margin: 20px 15px ; 이러면 상하, 좌우 순으로 적용
16. collapsing margins 현상 : 위아래 경계가 일치하면 두 요소의 마진은 1개로 취급한다(ex. div, body 경계가 같은경우)





=vsc 간편 단축키=
VSC 간편 단축키

7. 반복되는 단어 한방에 수정
   ⌘ + D or Ctrl + D(한번씩 일일이 눌러줘야함 / 귀찮으면 Ctrl + F2)

8. 클릭하는 곳마다 커서 생성
   ⌥ + Click or Alt + Click

9. 코드 위/아래로 움직이기
   ⌥ + ↑ / ↓ or Alt + ↑ / ↓

10. 코드 복사해서 위/아래로 움직이기
    ⌥ + ⇧ + ↑ / ↓ or Alt + ⇧ + ↑ / ↓

11. 코드 블록 한방에 코멘트 처리하기
    ⌘ + / or Ctrl + /

12. 선택된 영역에 커서 만들기
    ⌥ + ⇧ + i or Alt + ⇧ + i

13. 마우스가 가는 곳 마다 커서 만들기
    ⌥ + ⇧ + Mouse Drag or Alt + ⇧ + Mouse Drag

Bonus:
파일 맨 위-아래로 한번에 이동하기
Top / Bottom of File: ⌘ + ↑ / ↓ or Ctrl + Home / End

사이드바 숨기기
Hide / Show Sidebar: ⌘ + B or Ctrl + B
-->노마드 코더 코코아클론 강의 2.7 댓글 참고

6.12 ~ 13 배운내용 정리
6.12: 200짜리 박스에 padding-left 50px등 값을주면 css는 알아서 padding 한 공간만큼 값을 늘린다 (200px가 250px 가 됨)
      이걸 방지하고싶으면     box-sizing: border-box; 사용한다. 이러면 padding이 생겨도 그만큼 박스 사이즈를 늘리지 않는다

6.13: 네이게이션바의 채팅 아이콘 위에 채팅이 몇개 왔는지 구현
      span에 클래스 nav__notification 주고 css를 통해 구현했다
      backgroud color : tomato를주고 
      원형으로 만들기위해 border-radius 50% (혹은 width 값에 절반)을준다
      이떄, span은 높이 와 넓이를 가질수 없으니 display flex를 해준다. 

      이후 숫자 1을 가운데 정렬하기위해 
         justify-content: center;
        align-items: center; 사용 한다.

        폰트 두께는 font-weight, 색깔은 color로 조정할수 있다. 

        마지막으로 위치를 조정하기 위해 
        position: absolute;
        left: 13px;
        bottom: 15px
        사용해준다. 단, 부모 class(span을 감싸고 있는 부모 클래스)에     position: relative;를 줘야한다! 
        그렇지 않으면 body 기준으로 값이 이동함

        추가로 강의 마지막 부분 챌린지 내용
        nav__ellipsis{
            background-color: tomato;
            width: 5px;
            height: 5px;
            border-radius: 50%;
            display: block;
            font-weight: 600;
            position: absolute;
            left: 30px;
            bottom: 25px
        }