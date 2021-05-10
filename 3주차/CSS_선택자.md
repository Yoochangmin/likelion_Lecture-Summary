- # 선택자

  ------

  h1,p,span,div

  h1,p //선택자{

  ​    color : red;

  }\

  ## 단순 선택자

  타입(Type) , 클래스 (Class), 아이디(ID), 전체(Universal), 속성(Attribute)

  #### 타입 선택자: 해당 태그를 가지는 모든 요소에 스타일을 적용

  ```
  <!DOCTYPE html>
  <html>
  <head>
      <title>수노입니다.</title>
      <style>   
          p{color: red;}    //타입 선택자
           h2 {color: royalblue;} // 타입 선택자
      </style>
  </head>
  <body>
      <h1>수업입니다.</h1>
      <p>이것은 첫번째 단락입니다.</p>
      <h2>작은 수업입니다.</h2>
      <p>이것은 두번째 단락입니다.</p>
      <h2>작은 수업입니오잉</h2>
  </body>
  </html>
  ```

  ### 아이디 선택자(Id Selector) : Id로 스타일을 적용 해당 Id하나에 적용(Id는 하나만)​

  ```
  #name_head{ background-color:sandybrown}   //아이디 선택자 꾸미기시 #아이디
  <h2 id ="name_head">작은 수업입니다.</h2>
  ```

  ### 클래스(Class) : 비슷한 특징을 갖는 요소를 지정하여 묶을 수 있음                                               여러번 사용이 가능

  ```
    .comtent {font-size: 24px;}   //클래스 꾸미기 시 .클래스
    <p class ="content">이것은 두번째 단락입니다.</p>
      <h2>작은 수업입니오잉</h2>
      <p class ="content"> 이것은 세번째 단락입니다.</p>
  ```

  ### 전체 선택자( Universal Selector): 모든 요소에  스타일을 적용 //안쓰길 권장

  ```
  *{background-color:red;}  // *사용
  ```

  ### 속성 선택자(Attribute Selector):특정 속성을 소유하는 모든 요소에 스타일을 적용

  ```
  선택자[속성명="속성값"]{color:red;}
  a[target ="_blank"]{color: red;}
  #newlink[target ="_blank"]{color: red;}
  
  <a href="링크 주소" target = "_self">라이크라이오느</a>
  <a href="링크 주소" target = "_blank">라이크라이오느</a>
  <a href="링크 주소" target = "_self">라이크라이오느</a>
  ```

  ### 복합 선택자:

  |            |      |             |      |
  | :--------: | :--: | :---------: | ---- |
  |            |      | article(나) |      |
  | 후손(자식) | div  |     div     | a    |
  |    후손    |  p   |      p      |      |

  ##### 자식 선택자(Child Selector):선택자 A의 모든 자식 중 선택자 B와 일치하는 요소 선택    

  ```
  // article > p {color:red;} /* article안에있는 자식p에게 속성적용*/
  
      <style>
      article > p {color:red;} /* article안에있는 p태그에 속성적용*/
      </style>
  
  <body>
      <article>
          <div>자식1
              <p>후손</p>
          </div>
          <div>자식2
              <p>후손2</p>
          </div>
          <p>자식3</p>
      </article>
  </body>
  ```

  ##### 후손 선택자(Descendant Selector): 선택자A의 모든 후손 중 선택자B와 일치하는 요소 선택

  ```
  선택자A 선택자B {color: blue;}
  article p {color: blue;}
  ```

  ### preudo -class(가상의 클래스):요소의 특별한 상태를 지정할 때 씀

  ```
  선택자:pseudo-class{
  	속성: 속성 값;
  }
  :link :방문하지 않은 링크일 경우
  :visited : 방문한 링크일 경우
  :hover : 요소에 마우스가 올라와 있을 경우
  
     a:link {color: yellow;}
     a:visited {color:violet;}
     a:hover {background-color: teal; }
  ```

  



