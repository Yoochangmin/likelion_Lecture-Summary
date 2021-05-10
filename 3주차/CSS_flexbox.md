- # Flexbox

  ![](C:\Users\cdals\OneDrive\바탕 화면\멋쟁이사자처럼!!~~\강의 정리\picture\flexbox.PNG)

  ### -가로방향 or 세로방향으로  프로퍼티 적용

  1. ## 부모요소

     | -flex-direction:flex 컨테이너 안의 item들의 방향을 정함 기본 row |
     | ------------------------------------------------------------ |
     | flex-direction:row or row-reverse;  ; flex-direction:column or column-reverse; |
     | -**flex-wrap**: flex 아이템이 flex 컨테이너를 벗어 났을 댸 줄을 바꾸는 속성 |
     | ![](C:\Users\cdals\OneDrive\바탕 화면\멋쟁이사자처럼!!~~\강의 정리\picture\wrap.PNG) |
     | **justify-content**: flex-direction으로 정해진 방향을 기준으로 수평으로  item을 정렬하는 방법을 정함 |
     | ![](C:\Users\cdals\OneDrive\바탕 화면\멋쟁이사자처럼!!~~\강의 정리\picture\justify-content.PNG) |
     | ![](C:\Users\cdals\OneDrive\바탕 화면\멋쟁이사자처럼!!~~\강의 정리\picture\space.PNG) |
     |                                                              |
     |                                                              |

     -**justify-content**: flex-direction으로 정해진 방향을 기준으로 수평으로  item을 정렬하는 방법을 정함

     ![](C:\Users\cdals\OneDrive\바탕 화면\멋쟁이사자처럼!!~~\강의 정리\picture\justify-content.PNG)

     ![](C:\Users\cdals\OneDrive\바탕 화면\멋쟁이사자처럼!!~~\강의 정리\picture\space.PNG)

     space- around :좌우 균일 분배

     space- between : 양끝 배치 후 사이 간격 균인 분배

     **-align-item**: 뱡향을 기준으로 수직으로 item을 정렬

       :   flex-start,   center, flex-end

     -align-content:

     ![](C:\Users\cdals\OneDrive\바탕 화면\멋쟁이사자처럼!!~~\강의 정리\picture\content.PNG)

     ![](C:\Users\cdals\OneDrive\바탕 화면\멋쟁이사자처럼!!~~\강의 정리\picture\content space.PNG)

  2. ## 자식요소

     flew- grow : flex 아이템의 확장과 관련된 속성, 기본 0

     ex) 남은 부모요소의 width 부분 컨테이너를 비율에 따라 나누어짐

     ![](C:\Users\cdals\OneDrive\바탕 화면\멋쟁이사자처럼!!~~\강의 정리\picture\grow.PNG)

     ![](C:\Users\cdals\OneDrive\바탕 화면\멋쟁이사자처럼!!~~\강의 정리\picture\grow2.PNG)

     flex-shrink: 아이템의 축소와 관련된 속성,  기본 1

     ![](C:\Users\cdals\OneDrive\바탕 화면\멋쟁이사자처럼!!~~\강의 정리\picture\shrink.PNG)

     ![](C:\Users\cdals\OneDrive\바탕 화면\멋쟁이사자처럼!!~~\강의 정리\picture\shrink2.PNG)

     flex-basis:flex 아이템의 기본 크기를 결정함

     ex) flex-basis: 20px;

     ## flex 축약형 : 

     ## =>    flex : 1 1 20px 

     

```
<!DOCTYPE html>
<html>
<head>
    <title>수노입니다.</title>
    <style>
        body{margin: 0;}
          #container{ background-color:skyblue;
          display:flex;
          flex-direction: row;
          width: 300px;
          height: 150px;
    
          /* justify-content: space-between; */
          align-items: center;
          /* flex-wrap: wrap; */
            align-content:flex-start;
          }
          .item{
              border-radius: 4px;
              background-color: brown;
              height: 60px;
              width: 60px;

          }
          #one{
              /* flex-shrink: 0; */
              flex-grow: 1;
          }
          #two{
              /* flex-shrink: 1; */
              flex-grow:2;
          }
          #three{
              /* flex-shrink: 2; */
          }
    </style>
</head>
    <div id="container">
        <div id ="one" class="item">1</div>
        <div id ="two" class="item">2</div>
        <div id = "three" class="item">3</div>
        
        
    </div>
   

   
</html>
```

