---
layout: darkplain
title: Facts and Figures
lang: en
---

# 從2019年6月9日截至2019年8月5日,

<p>&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;警方一共發射了<span id="p1num">0</span> 枚催淚彈、<span id="pnuma">約</span><span id="p2num">0</span> 枚橡膠彈 及 <span id="p3num">0</span>枚海綿彈</p>
<p>&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;
	&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;
	&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;<span id="m1num">|</span>名市民被拘捕</p>
<p>&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;
	&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;
	&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;
	&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;
	&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;
	&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;
	年紀最小的被捕者只有<span id="m2num">0</span>歲 </p>
<p>&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;
	&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;<span id="m4num">0</span>大訴求，<span id="p4num">0</span>個兌現</p>
<p>&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;
	&#8195;&#8195;&#8195;&#8195;
	&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;
	&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;&#8195;
	&#8195;&#8195;&#8195;&#8195;&#8195;年紀最大的被捕者已屆<span id="m3num">0</span>歲</p>


<script> 
	function animateValue(id, start, end, duration) {
    // assumes integer values for start and end
    
    var obj = document.getElementById(id);
    var range = end - start;
    // no timer shorter than 50ms (not really visible any way)
    var minTimer = 50;
    // calc step time to show all interediate values
    var stepTime = Math.abs(Math.floor(duration / range));
    
    // never go below minTimer
    stepTime = Math.max(stepTime, minTimer);
    
    // get current time and calculate desired end time
    var startTime = new Date().getTime();
    var endTime = startTime + duration;
    var timer;
  
    function run() {
        var now = new Date().getTime();
        var remaining = Math.max((endTime - now) / duration, 0);
        var value = Math.round(end - (remaining * range));
        obj.innerHTML = value;
        if (value == end) {
            clearInterval(timer);
        }
    }
    
    timer = setInterval(run, stepTime);
    run();
}

animateValue("p1num", 0, 1000, 1000);
animateValue("m1num", 0, 502, 1000);

animateValue("p2num", 0, 160, 1000);
animateValue("m2num", 0, 16, 1000);

animateValue("p3num", 0, 150, 1000);
animateValue("m3num", 0, 76, 1000);

animateValue("p4num", 0, 0, 1000);
animateValue("m4num", 0, 5, 1000);
</script>