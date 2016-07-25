---
layout: default
title: Cody Badger
---

<script src="https://code.jquery.com/jquery-3.1.0.min.js" integrity="sha256-cCueBR6CsyA4/9szpPfrX3s49M9vUU5BgtiJj06wt/s=" crossorigin="anonymous"></script>

<center><img id="face-img" src="/images/CodyFloatingHead.png" alt="that's me" style="width:600px; PADDING-TOP: 100px; PADDING-BOTTOM: 100px;"></center>

<script>
var rotating = false;
$(document).ready(function() {
    $("#face-img").click(function() {
        if (rotating == false){
            $(this).css("-webkit-transform","rotate(720deg)");
            $(this).css("-moz-transform","rotate(720deg)"); 
            $(this).css("-o-transform","rotate(720deg)");
            rotating = true;
        } else {
            $(this).css("-webkit-transform","");
            $(this).css("-moz-transform",""); 
            $(this).css("-o-transform","");
            rotating = false;
        }
    });
});
</script>
