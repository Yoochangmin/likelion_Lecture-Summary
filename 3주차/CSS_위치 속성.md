- # display 

  ------

  : 요소가보여지는 방식을 지정

  display: block;

  | 새로운 줄에서 시작-                   |
  | ------------------------------------- |
  | <div> , <h>, <p>, <header>, <section> |
  | width, height, margin, padding 가능   |

  

  display; inline

  | 새로운 줄에서 시작하지 않고 content 만큼의 너비만큼만 가짐 |
  | ---------------------------------------------------------- |
  | <a>, <span>, <img>                                         |
  | width, height, margin-top, padding-bottom 불가능           |



​		display:inline-block

- | content 만큼의 너비만큼만 가짐                 |
  | ---------------------------------------------- |
  | <a>, <span>, <img>                             |
  | width, height, margin-top, padding-bottom 가능 |



- # position

  ------

  1. static : 기본, 좌표 프로퍼티 사용 불가

  2. relative :  상대위치, 기본 위치를 기준으로 좌표이동

     | top  |      |
     | ---- | ---- |
     | left |      |

     

  3. absolute : 부모나 조상 증 relatice, absolute, fixed가 선언된 곳을 기준으로 좌표 프로퍼티 적용

     ------

     inline처럼 content가 width가 줄어듬.   너비만 inline처럼 바뀜 inline 블록이라 생각

  4. fixed : fixed는 보이는 화면을 기준으로 좌표 프로퍼티를 이용하여 위치를 고정

  5. z-index: 1~ : 층의 우선순위

     ```
     <!DOCTYPE html>
     <html>
     <head>
         <title>수노입니다.</title>
        
         <style>
           #parent{
               width: 200px;
               height: 200px; 
               background-color: blue;
               position: relative;
               top: 50px; 
               left: 50px;
           }
     
           #child{
               width: 100px;
               height: 100px;
               position: relative;
               background-color: red;
               top:20px;
               left:20px;
               
           }
           #child2{
             position:absolute;
             width: 200px;
               height: 200px;
               background-color:chartreuse;
               top:20px;
               left:20px;
           }
         </style>
     </head>
     <body>
         <div id ="parent">
             <div id = "child">
             child.
             </div>
             <div id = "child2">
             child2
              </div>
         </div>
     </body>
     </html>
     ```

     ```
     <!DOCTYPE html>
     <html>
     <head>
         <title>수노입니다.</title>
        
         <style>
         body{background-color: skyblue; margin : 0;}
         #main{height:1200px;}
         #fixed{
             background-color: pink;
             height: 60px;
             position: fixed;
             left: 0;
             top:0;
             width: 100%;
         }
         </style>
     
     </head>
         <body>
             <div id ="main">
                 <div id ="fixed">
                     저는 고정 되어 있습니다.
                 </div>
                 이 노래는 유명해지지 않았으면 해
                 이 노래는 유명해지지 않았으면 해
                 사람들이 가사를 못 외웠으면 해
                 에라라라라 에베베베 에베베베
     
                 일주일 전 욕조에서
                 나 혼자 흥얼거리던 노래
                 이제는 너 혼자 듣고 있고
                 곧 사람들도 듣게 되겠지
     
                 피아노 하나로는 심심해
                 베이스도 넣게 되었지
                 하루 종일 널 생각하다 쓴 노래
                 별 내용은 없지만
                 그냥 내 마음이다 생각하고 들어줬으면
     
                 이 노래는 유명해지지 않았으면 해
                 이 노래는 유명해지지 않았으면 해
                 사람들이 가사를 못 외웠으면 해
                 에라라라라 에베베베 에베베베
                 </div>
             
         </body>
     </html>
     
     ```

     

  