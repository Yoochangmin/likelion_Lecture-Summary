- # Flexbox

 ![flexbox](https://user-images.githubusercontent.com/81625956/117682535-1fdf6900-b1ee-11eb-924b-359cc8873d99.PNG)


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

     ![justify-content](https://user-images.githubusercontent.com/81625956/117682737-56b57f00-b1ee-11eb-8f3f-00654a1c3a1a.PNG)


     ![space](https://user-images.githubusercontent.com/81625956/117682790-66cd5e80-b1ee-11eb-8283-6d96c8c0a91e.PNG)

     space- around :좌우 균일 분배

     space- between : 양끝 배치 후 사이 간격 균인 분배

     **-align-item**: 뱡향을 기준으로 수직으로 item을 정렬

       :   flex-start,   center, flex-end

     -align-content:


     ![content](https://user-images.githubusercontent.com/81625956/117682840-7351b700-b1ee-11eb-9d0d-37adbf72d4c4.PNG)
     
     ![content space](https://user-images.githubusercontent.com/81625956/117682878-7c428880-b1ee-11eb-9e59-e42e89316c81.PNG)

  2. ## 자식요소

     flew- grow : flex 아이템의 확장과 관련된 속성, 기본 0

     ex) 남은 부모요소의 width 부분 컨테이너를 비율에 따라 나누어짐
     
     ![grow](https://user-images.githubusercontent.com/81625956/117682921-85cbf080-b1ee-11eb-9b6c-896049ab0fa3.PNG)

     ![grow2](https://user-images.githubusercontent.com/81625956/117682947-8c5a6800-b1ee-11eb-9e4e-1735b893af0f.PNG)

     flex-shrink: 아이템의 축소와 관련된 속성,  기본 1

     ![shrink](https://user-images.githubusercontent.com/81625956/117682991-954b3980-b1ee-11eb-9b55-ccfba5706b3b.PNG)
   
     ![shrink2](https://user-images.githubusercontent.com/81625956/117682997-9714fd00-b1ee-11eb-9144-768923a3c0a3.PNG)

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

