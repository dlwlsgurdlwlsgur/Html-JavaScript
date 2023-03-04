# 파일 생성
```
function download(filename, text) {
    let element = document.createElement('a');
    element.setAttribute('href', 'data:text/plain;charset=utf-8,' + encodeURIComponent(text));
    element.setAttribute('download', filename);
    element.style.display = 'none'; //하이퍼링크 요소가 보이지 않도록 처리
    document.body.appendChild(element); //DOM body요소에 하이퍼링크 부착
    element.click(); //클릭 이벤트 트리거 - 이 시점에 다운로드 발생
    document.body.removeChild(element); //하이퍼링크 제거
}
```

# 파일 호출
```
<script src="index.js"></script>
```
