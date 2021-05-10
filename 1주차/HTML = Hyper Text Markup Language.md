# HTML = Hyper Text Markup Language

------

- HTML 코드
  1. 글
  2. 태그
  3. 속성

```html
<h1> 오늘의 활동 <h1>
    <p>나는 오늘 일어나서 슬프지만 과제를 했다... 과제를 진행한지 언 10시간 후 그 뒤에도 끝나지 않은 과제로 인        해 나는 지금 죽기 일보 직전이다.. 교수님... 과제좀 그만 주세요 ㅠㅠㅠㅠㅠㅠ 오늘의 활동 끝...</p>
```

```
<!DOCTYPE html> // 이 문서는 html로 작성된 문서라는 것을 표현 
<html> </html> // 이 문서는 html로 작성된 문서라는 것을 표현 
<head> </head> // 문서의 타입, 인코딩 방식(utf-8)을 나타냄 
<body> </body> // <h1> <li> <a> <img> 등 문서를 직접적으로 표현하는 html태그를 이용하여 나타내는 곳
```



- ## 태그

```form : 사용자로부터 입력값을 받는 태그
<form action ="전송받을 대상"> </form>
<input type = "txet" name=" id "> // 입력타입은 텍스트, 입력값의 이름은 id 로 인식
<input type = "password name = "pw"> // 입력타입은 패스워드, 입력값의 이름은 pw로 인식
<textarea cols ="30" rows ="20"></textarea>  //텍스트 공간 너비는 20 높이는 30으로 구성
<input type ="submit"> // 위의 정보들을 전송받을 대상에게로 전송


<select> // 선택 가능 항목 
<option value= "옵션">이름</option> 이름이라는 선택항복의 값의 옵션을 생성 => 전송받을 대상은 옵션이라고 인식
</select> 

ul>li*4
사용자   ------>HTML ------->입력값 처리 프로그램
```

```
<img = "파일 이름">   //이미지 파일 생성
<ol> //번호가 있는 목록을 만드는 태그
<ul> //번호가 없는 목록을 만드는 태그
<li> // 목록을 만드는 태그
<br> // 한 줄 띄우는 태그
<p> //  문단을 설정해서 문단이 끝나면 띄우는 태그
<a href></a> // 링크(하이퍼텍스트)를 연결해주는 태그

```

```공부하면서 만든 코드
<!DOCTYPE html>
<html lang="ko">
    <script
    src="https://code.jquery.com/jquery-3.6.0.js"
    integrity="sha256-H+K7U5CnXl1h5ywQfKtSj8PCmoN9aaq30gDh27Xc0jk="
    crossorigin="anonymous"></script>
    <head>
     /*   <!-- 합쳐지고 최소화된 최신 CSS -->
        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap.min.css">

        <!-- 부가적인 테마 -->
        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap-theme.min.css">

        <!-- 합쳐지고 최소화된 최신 자바스크립트 -->
        <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/js/bootstrap.min.js"></script>
        */ 부트 스트렙을 이용하기 위해 필요한 코드
       
       <meta charset="uft-8">
        <title>나를 소개해요</title>
    </head>
    <body>
        <div class="container">
        <h1>유창민</h1><br>
        <ul class="nav nav-tabs">
            <li role="presentation" class="active"><a href="1.html">유년기</a></li>
            <li role="presentation"><a href="#">Profile</a></li>
            <li role="presentation"><a href="#">Messages</a></li>
          </ul>
            <form action="전송받을 대상">

                아아디 : <input type="text" name="id">
                비밀번호 : <input type ="password" name="pw">
                <div class="form-group">
                  <label for="exampleInputEmail1">이메일 주소</label>
                  <input type="email" class="form-control" id="exampleInputEmail1" placeholder="이메일을 입력하세요">
                </div>
                <div class="form-group">
                  <label for="exampleInputPassword1">암호</label>
                  <input type="password" class="form-control" id="exampleInputPassword1" placeholder="암호">
                </div>
                <div class="form-group">
                  <label for="exampleInputFile">파일 업로드</label>
                  <input type="file" id="exampleInputFile">
                  <p class="help-block">여기에 블록레벨 도움말 예제</p>
                </div>
                <div class="checkbox">
                  <label>
                    <input type="checkbox"> 입력을 기억합니다
                  </label>
                </div>
                <input type="submit" class="btn btn-primary">
              </form></br>
        
         
        <img src="강아지.jpg" width="300px" height="300px"><br>

        <form action="전송받을 대상">
            <h2>나의 일기장</h2>

            제목 : <input type="text" name="diarytitle"><br>
            <select>
                <option value="goodday">좋은날</option>
                <option value="sadday">슬픈날</option>
                <option value="gloomydday">우울한날</option>
            </select><br>

            내용 : <br>
            <textarea cols="30" rows="20"></textarea><br>
             <input type="submit">
        </form><br>

        
        <h2>나의 일대기</h2>
        <ol>
            <li><a href="1.html">유년기 </a>  </li>
            <li><a href="2.html">청소년기</a></li>
            <li>청년기</li>
        </ol>
        <ul>
            <li></li>
            <li></li>
            <li></li>
        </ul>
    </div>

    <div class="progress">
        <div class="progress-bar progress-bar-success" role="progressbar" aria-valuenow="40" aria-valuemin="0" aria-valuemax="100" style="width: 40%">
          <span class="sr-only">40% Complete (success)</span>
        </div>
      </div>
      <div class="progress">
        <div class="progress-bar progress-bar-info" role="progressbar" aria-valuenow="20" aria-valuemin="0" aria-valuemax="100" style="width: 20%">
          <span class="sr-only">20% Complete</span>
        </div>
      </div>
      <div class="progress">
        <div class="progress-bar progress-bar-warning" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" style="width: 60%">
          <span class="sr-only">60% Complete (warning)</span>
        </div>
      </div>
      <div class="progress">
        <div class="progress-bar progress-bar-danger" role="progressbar" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100" style="width: 80%">
          <span class="sr-only">80% Complete (danger)</span>
        </div>
      </div>
    </body>
</html>
```

부트스트렙 : css 자바스크립터를 기반으로 만들어진 웹 프레임워크 

이용 방법 부트스트랩 CDN코드 와 j-Quary 코드 헤더파일에 적용



github

1.code저장 가능

2 unbo 기능