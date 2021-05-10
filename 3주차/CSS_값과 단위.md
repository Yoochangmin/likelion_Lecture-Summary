- # 단위

  ```
  px : 1px = 1/96(in)  -> 절대 길이
  em : 현재 스타일이 지정된 요소의 font-size 기준 -> 상대적인 길이
  rem : 최상위 요소의 font-size기준 -> 상대적인 길이
  %(퍼센트) : 상대길이, 이미지나 레이아웃의 너비나 높이를 지정할 떄 씀.
  ```

  ```
  <!DOCTYPE html>
  <html>
  <head>
      <title>수노입니다.</title>
      <style>
      html{
          background-color: tomato;
          font-size = 30px;
      }
      #main{
          background-color: violet;
          height:150px;
      }
      #px{ 
          background-color:yellow;
          height:10px;
          width: 10px;
      }
      #em{                           // 1em =25px;
          background-color: blue;
          width: 1em;
          height: 1em;
          font-size: 25px;
      }
      #rem{                          // 1rem = 30px;  html 태그(최상위 요소)
          background-color: brown; 
          width: 1rem;
          height: 1rem;
     
      }
      </style>
  </head>
  <body>
      <div id ="main">
          단위
          <div id = "px">px</div>
          <div id ="em">em</div>
          <div id ="rem">rem</div>
      </div>
  </body>
  </html>
  ```

  - ## 색상

    영어  , hex - code  , rgb(  ,  , )

