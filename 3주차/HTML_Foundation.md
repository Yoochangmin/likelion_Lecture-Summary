- # HTML기초

  ------

  ```
  !DOCTYPE HTML!  //이 문서는 html로 작성됨을 의미
  <html lang = "ko">    // html의 문서가 한국말로 작성됨
  	<head>  // 문서를 설명해주는 태그  (내적)
  		<meta charset ="utf-8">  // 인코딩 방식이 uft-8	
  	</head>
  
  <body>   // 문서의 본문을 나타내는 영역 (외적)
  
  </body>
  
  </html>
  ```

  - ## 태그(tag)  : 의미를 가지고 있는 태그  기본요소

    ------

    ```
    1.제목 태그
    <h1~h6>  </h1~h6> // 제목을 나타내는 태그 //수가 커지면 제목의 크기작아짐
    --------------------------------------------------------------------
    2.본문태그
    <p></p> // 단락 구분 // </p> 부분에 줄바꿈 
    <br>  // 줄바꿈
    <pre></pre> // 입력한대로 문장을 출력
    <strong></strong>  // 글씨 굵어짐
    <em></em>  // 글씨가 기울어짐
    <ins></ins>  // 아래로 밑줄
    <del></del> //  가운데로 밑줄
    <sub></sub> // 글자가아래로
    <sup></sup>  // 글자 위로
    ```

    - ## 링크,이미지

      ------

      ```
      <a href ="주소">주소제목</a>  //주소제목 클릭시 저장해논 주소로 이동
      <img src = "이미지 주소(URL)">  // 저장한 URL주소의 이미지를 출력
      <img src = "이미지 주소(URL)" alt ="이미지가 출력안될때 사진설명"    height="?px" width="?px" //높이와 너비>
      ```

      - ##   웹페이지의 구성요소

       		<img src ="웹페이지 구성요소.png">
      
      

      - ## <table 태그>
      
        - table  // 표 전체를 나타냄
  - tr       // 행을 나타냄
        - th      //   행의 제목을 나타냄  // 1열
        - td      //   행의 열을 나타냄    // 2열부터
        - colspan, rowspan = "숫자" // 값만큼 행과 열을 점유
      
        ```
        <table>
          <tr>                  // 1행
              <th> 제목</th>    // 1행 1열
        <th> 제목</th>    // 1행 2열
              <th> 제목</th>    // 1행 3열
          </tr>
          <tr>                  // 2행
             <td> 내용 </td>    // 2행 1열 데이터
       <td> 내용 </td>    // 2행 2열 데이터
             <td> 내용 </td>    // 2행 3열 데이터
    </tr>
            <tr>                  // 3행
             <td> 내용 </td>    // 2행 1열 데이터
             <td colspan ="2"> 내용 </td>    // 2행 2부터 3열까지 행을 통합 
          </tr>
        ```

      - ## 목록 태그
      
        - ol  //순서가 있는 목록 태그
        - ul  //순서가 없는 목록 태그
        - li   //항목들을 나타냄
      
        ```    
        <ol  start="숫자">  // 리스트의 시작숫자 나타냄
        <ol type ="문자">   // 리스트의 순서를 시작하는 문자 // 로마자, 숫자
        <ol reversed>       // 순서를 반대로 시작
        
        <li value="숫자">    //해당 리스트의 아이템의 번호 지정
        ```
      
      - ## <form>태그
      
        ```
  action // 데이터를 보낼 URL 지정
        method // 보내는 방식 지정
   -get : 데이터를 URL끝에 붙여 눈에 띄게 보냄 // 데이터 조회 // 엽서
         	(header~URL) +데이터  //get
         	(Body      )
         -post : 데이터를 URL에 적지 않고 내부에 숨겨 보냄 // 서버 데이터 수정,작성,삭제에 이용 //편지
   	(header~URL)
         	(Body +데이터)
        input //사용자의 입력값을 만들어냄
         -input type = "text" // text 타입으로 입력
         -input type = "passwod"  // 정보가 공개되지 않는 타입으로 입력
         -label  //
         -textarea // 많은 글을 입력 받을 때 이용
         -botton  // 입력값으로 버튼 생성
   -placeholder // 입력받는 곳의 내용을 지정
        ```

        ```
        <form action ="URL" method = "get">
        	<input type ="text" name ="id" placeholder ="아이디를 입력하시오">
        	<input type ="text" name ="password" placeholder ="비밀번호를 입력하시오">
        	
         
        ```
      
        
      
        - ## select 태그
      
          ```
          <select name ="값"> // 값이라 불리는 이름 설정
          	<option value> 내용1 </option>  // 선택값으로 내용1 생성
          	<option value> 내용2 </option>  // 선택값으로 내용2 생성
          	<option value> 내용3 </option>  // 선택값으로 내용3 생성
    </select>
          ```
      
        - ## div태그 // 태그들을 구분짓고 나누기 위해 사용 // 아무것도 안나타냄
      
          
      

