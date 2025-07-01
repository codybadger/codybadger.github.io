---
layout: default
title: Cody Badger
---

<script src="https://code.jquery.com/jquery-3.7.1.min.js" integrity="sha256-/JqT3SQfawRcv/BIHPThkBvs0OEvtFFmqPF/lYI/Cxo=" crossorigin="anonymous"></script>

<center><img id="face-img" src="/images/CodyFloatingHead.png" alt="that's me" style="width:600px; PADDING-TOP: 100px; PADDING-BOTTOM: 100px;"></center>

<script>
var rotating = false;
$(document).ready(function() {
    $("#face-img").click(function() {
        if (rotating == false){
            $(this).css("transform","rotate(720deg)");
            rotating = true;
        } else {
            $(this).css("transform","");
            rotating = false;
        }
    });
});
</script>
