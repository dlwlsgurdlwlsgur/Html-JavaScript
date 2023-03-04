# Hide Input & Alert input_data

# 단일 개체
```
    <button onclick="hide_input('a');">삭제&추가</button>
    <button onclick="data('a');">확인</button>

    <input id="a" type="text" placeholder="" size="30" style="display : none";>
    <script>
        function hide_input(id){
            if (document.getElementById(id).style.display === "none") {
                document.getElementById(id).style.display = "block";
            } else {
                document.getElementById(id).style.display = "none";
            }} 
            
    </script>
```

# 다중 개체
```
    <button onclick="hide_input(['a', 'b', 'c'])">삭체&추가</button><br><br>
    <input id="a"; type="text"; placeholder=""; size="30"; style="display : none";>
    <input id="b"; type="text"; placeholder=""; size="30"; style="display : none";>
    <input id="c"; type="text"; placeholder=""; size="30"; style="display : none";>


    <script>
        function hide_input(id){
            for(i in id){
                if (document.getElementById(id[i]).style.display === "none") {
                    document.getElementById(id[i]).style.display = "block";
                }else {
                    document.getElementById(id[i]).style.display = "none";
                }}}
    </script>
```

# input이 none(숨김)이 아니라면 데이터 가져오기
```
        function data(id){
            for(i in id){
                check = 1;
                if (document.getElementById(id[i]).style.display != "none") {
                    check = 0
                }}
            if (check == 0){
                alert('성rhd')
            }}
```
