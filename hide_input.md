# Hide Input & Alert input_data
```
    <button onclick="hide_input('a');">삭제&추가</button>
    <button onclick="data('a');">확인</button>

    <input id="a" type="text" placeholder="" size="30" style="display : none";>
    <script>
        function hide_input(id) {
        if (document.getElementById(id).style.display === "none") {
            x.style.display = "block";
        } else {
            x.style.display = "none";
        }} 
        function data(id){
            var x = document.getElementById(id);
            if (document.getElementById(id).style.display != "none") {
                pass;
            }}  
    </script>
```
