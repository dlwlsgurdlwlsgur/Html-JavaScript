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

        function data(id){
            var x = document.getElementById(id);
            if (document.getElementById(id).style.display != "none") {
                alert("성공");
            }}  
    </script>
```

# 다중 개체
```
    <button onclick="hide_input(['a', 'b', '])">삭체&추가</button><br><br>
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

        function data(id){
            var x = document.getElementById(id);
            if (document.getElementById(id).style.display != "none") {
                alert("성공");
            }}  
    </script>
```
