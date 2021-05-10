- # 박스모델

  ------

  - ### 구성 

 ![boxmodel](https://user-images.githubusercontent.com/81625956/117682382-f4f51500-b1ed-11eb-8226-9ec801278a34.PNG)

- ### 마진(Margin): Border 밖의 여백 

- ### 패딩 (Padding): content와 margin 사이의 여백

```
    <style>
      #innner{
          width: 200px;
          height: 100px;
          margin:20px;
          padding:20px;
          background-color: blue;
          color :red;      
         
          border: 4px solid black;

      }
    </style>
    
    <body>
    <div id ="main">
        <div id = "innner">
        이것은 박스 모델 개념입니다.
        </div>
    </div>
</body>
```

- ### border 속성

![border](https://user-images.githubusercontent.com/81625956/117682440-03dbc780-b1ee-11eb-82b8-41ac00ba486a.PNG)

```
  // 다음 값들을 적용할 때
  border-style:dashed double dotted solid ;
  border-width : 6px 8px 10px 12px;
  border-color: red black yellow green;
  
  border-radius:  //모서리 타원
```

   -위아래 마진을 적용시 큰 쪽 마진을 따라 작은 쪽 마진은 상쇄댐

- ### box-sizing

  ------

  box-sizing: content-box;  ///width(height)=content size

  box-sizing:border-box;   //width(height)= content size+padding +border

