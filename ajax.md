# ajax 다른 파일 전체 "글" 가져오기
```
<button ><img src ="이미지 링크"
    onclick="fetch('파일.py').then(function(response){
        response.text().then(function(text){
            alert(text) # 예) 경고문
        })
    })">
</button>

```


# ajax 가져온 "글" 실행
```
<article>

</article>

<button ><img src ="이미지 링크"
    onclick="fetch('파일.py').then(function(response){
        response.text().then(function(text){
            document.querySelector('article').innerHTML = text;
        })
    })"
    ></button>
```
