---
permalink: /about
layout: page
title: 
---

<style>

.dm-hero{
margin:48px 0 32px;
}

.dm-caption{
font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,monospace;
font-size:12px;
color:#7a7f85;
margin-bottom:16px;
}

.dm-wrap{
display:inline-block;
overflow-x:auto;
}

.dm-ascii{
font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,monospace;
font-size:14px;
line-height:1.05;
white-space:pre;
margin:0;

background:transparent !important;
border:none !important;
box-shadow:none !important;
padding:0 !important;

color:#48D597;
}

.s{color:#48D597;}
.sh{color:#236A4C;}
.lb{color:#5B5F61;}
.lt{color:#A1A4A5;}
.ac{color:#48D597;}
.acd{color:#236A4C;}

.blue{
color:#5DA9FF;
animation:pulseBlue 2.4s ease-in-out infinite;
}

.flow1{animation:flow 2.6s ease-in-out infinite 0s;}
.flow2{animation:flow 2.6s ease-in-out infinite .35s;}
.flow3{animation:flow 2.6s ease-in-out infinite .7s;}
.flow4{animation:flow 2.6s ease-in-out infinite 1.05s;}
.flow5{animation:flow 2.6s ease-in-out infinite 1.4s;}

.state{
animation:blinkRed 1s steps(2,end) infinite;
}

@keyframes flow{
0%,100%{
color:#236A4C;
opacity:.55;
text-shadow:none;
}

45%,60%{
color:#48D597;
opacity:1;
text-shadow:0 0 8px rgba(72,213,151,.25);
}
}

@keyframes blinkRed{

0%,49%{
color:#ff4d5a;
opacity:1;
text-shadow:0 0 10px rgba(255,77,90,.45);
}

50%,100%{
color:#7a2028;
opacity:.55;
text-shadow:none;
}

}

@keyframes pulseBlue{

0%{
color:#4A7CFF;
text-shadow:
0 0 3px rgba(93,169,255,.25),
0 0 6px rgba(93,169,255,.15);
}

50%{
color:#79BDFF;
text-shadow:
0 0 8px rgba(93,169,255,.6),
0 0 18px rgba(93,169,255,.35),
0 0 28px rgba(93,169,255,.25);
}

100%{
color:#4A7CFF;
text-shadow:
0 0 3px rgba(93,169,255,.25),
0 0 6px rgba(93,169,255,.15);
}

}

.dm-sub{
margin-top:14px;
font-size:12px;
letter-spacing:.14em;
text-transform:uppercase;
color:#7a7f85;
}

.dm-copy{
max-width:760px;
margin-top:30px;
}

</style>

<div class="dm-hero">

<div class="dm-caption">Fig 1. DataMachine Layout</div>

<div class="dm-wrap">

<pre class="dm-ascii">

<span class="s">+----------------</span><span class="blue">+</span><span class="s">.</span>
<span class="s">|`.</span>              <span class="sh">|</span> <span class="s">`.</span>
<span class="s">|</span>  <span class="s">`+----------------</span><span class="blue">+</span>
<span class="s">|</span>   <span class="s">|</span> DATAMACHINE <span class="sh">|</span>  <span class="s">|</span><span class="lb">[</span><span class="lt">IO</span><span class="lb">]</span>
<span class="s">|</span>   <span class="s">|</span><span class="acd">────────────</span><span class="s">|</span>
<span class="s">|</span><span class="sh">---</span><span class="s">|</span><span class="sh">-</span><span class="ac">feeds</span><span class="sh">.---</span><span class="blue">+</span><span class="s">.</span>  <span class="s">|</span>
<span class="s">|</span>   <span class="s">|</span><span class="ac">logs</span>     <span class="ac">ext</span>   <span class="s">|</span>
<span class="s">|</span>   <span class="s">|</span>raw      bus <span class="sh">|</span>   <span class="blue">+</span><span class="s">---+</span>
<span class="s">|</span>   <span class="s">|</span>trace    link <span class="sh">|</span>   <span class="s">|</span>
<span class="blue">+</span><span class="sh">---</span><span class="s">|</span><span class="sh">---</span><span class="flow1 blue">+</span><span class="sh">.--</span><span class="blue">+</span><span class="sh">.--</span><span class="s">|.</span>
 <span class="s">`.</span> <span class="s">|</span>    <span class="sh">|</span> <span class="sh">`.</span>  <span class="sh">`.</span><span class="s">|</span> <span class="s">`.</span>
   <span class="blue">+</span><span class="s">--------</span><span class="blue">+</span><span class="flow2">-</span><span class="s">--</span><span class="blue">+</span><span class="flow3">-</span><span class="s">--</span><span class="blue">+</span>
         <span class="s">|</span>   <span class="s">|</span>   <span class="sh">|</span>   <span class="s">|</span><span class="lb">[</span><span class="lt">BUS</span><span class="lb">]</span>
         <span class="s">|</span>   <span class="s">|</span>   <span class="sh">|</span>   <span class="s">|</span>
    <span class="blue">+</span><span class="s">----</span><span class="blue">+</span><span class="s">.</span><span class="sh">--</span><span class="s">|</span><span class="sh">---</span><span class="flow4">╱</span><span class="sh">.</span>  <span class="s">|</span>
    <span class="s">|`.</span>    <span class="s">`.|</span>     <span class="sh">`.</span><span class="s">|</span>
    <span class="s">|</span>  <span class="s">+-----+---+</span><span class="blue">+</span>
    <span class="s">|</span>  <span class="s">|</span> node <span class="sh">|</span>   <span class="s">|</span><span class="lb">[</span><span class="lt">NODE</span><span class="lb">]</span>
    <span class="s">|</span>  <span class="s">|</span> core <span class="sh">|</span>   <span class="s">|</span>
<span class="blue">+</span><span class="sh">---</span><span class="s">|</span><span class="sh">-----</span><span class="blue">+</span><span class="sh">.--</span><span class="s">|.</span>
<span class="s">|`.</span>  <span class="s">`.|</span> link  <span class="sh">`.</span><span class="s">|</span> <span class="s">`.</span>
<span class="s">|</span>  <span class="s">`+--+</span><span class="s">---------</span><span class="blue">+</span><span class="s">---+</span>
<span class="s">|</span>   <span class="s">|</span><span class="flow5">~&gt;</span> trace     <span class="sh">|</span>   <span class="s">|</span><span class="lb">[</span><span class="lt">CORE</span><span class="lb">]</span>
<span class="s">|</span>   <span class="s">|</span><span class="acd">log</span>       <span class="sh">|</span>   <span class="s">|</span>
<span class="s">|</span><span class="sh">---</span><span class="s">|</span><span class="acd">archive</span><span class="sh">--</span><span class="blue">+</span><span class="s">.</span>  <span class="s">|</span>
<span class="s">|</span>   <span class="s">|</span>  <span class="sh">|</span> <span class="sh">`.</span>        <span class="sh">`.</span><span class="s">|</span>
<span class="s">|</span>   <span class="s">|</span>  <span class="sh">|</span>   <span class="s">+---------+</span>
<span class="s">|</span>   <span class="s">|</span>  <span class="sh">|</span>   <span class="state">STATE</span>
<span class="s">|</span>   <span class="s">|</span>  <span class="sh">|</span>   watch
<span class="blue">+</span><span class="sh">---</span><span class="s">|</span><span class="sh">--</span><span class="blue">+</span><span class="s">.</span>  <span class="s">|</span>
 <span class="s">`.</span> <span class="s">|</span>    <span class="sh">`.</span><span class="s">|</span>
   <span class="s">`+------+</span>

</pre>

</div>


</div>

<div class="dm-hero">

<div class="dm-caption">Fig 2. Chaos Pendulum &mdash; two runs, 0.001 rad apart</div>

<div class="dm-wrap cp-wrap" title="click to reset">
<pre class="dm-ascii cp-ascii" id="cp-ascii" aria-label="Animated ASCII double pendulum"></pre>
</div>

<div class="cp-readout" id="cp-readout">&nbsp;</div>

</div>

<style>
.cp-wrap{cursor:pointer;}
.cp-ascii{color:#A1A4A5;line-height:1.05;}
.cp-ascii .pv{color:#5B5F61;}
.cp-ascii .ar{color:#236A4C;}
.cp-ascii .br{color:#2F5E99;}
.cp-ascii .ab{color:#48D597;text-shadow:0 0 8px rgba(72,213,151,.45);}
.cp-ascii .bb{color:#5DA9FF;text-shadow:0 0 8px rgba(93,169,255,.55);}
.cp-ascii .a0,.cp-ascii .a1,.cp-ascii .a2,.cp-ascii .a3{color:#48D597;}
.cp-ascii .b0,.cp-ascii .b1,.cp-ascii .b2,.cp-ascii .b3{color:#5DA9FF;}
.cp-ascii .a1,.cp-ascii .b1{opacity:.7;}
.cp-ascii .a2,.cp-ascii .b2{opacity:.42;}
.cp-ascii .a3,.cp-ascii .b3{opacity:.2;}
.cp-readout{
margin-top:14px;
font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,monospace;
font-size:12px;
color:#7a7f85;
}
.cp-readout .ka{color:#48D597;}
.cp-readout .kb{color:#5DA9FF;}
.cp-readout .kd{color:#ff4d5a;}
</style>

<script>
(function(){
  var el = document.getElementById('cp-ascii');
  var out = document.getElementById('cp-readout');
  if (!el) return;

  // grid + projection (monospace cells are ~1.75x taller than wide)
  var W = 51, H = 29, PX = 25, PY = 14, SY = 6.4, SX = SY * 1.75;
  var G = 9.81, DT = 0.004, TRAIL = 150, RESET_AFTER = 45;

  // double pendulum, equal masses and lengths
  function deriv(s){
    var t1 = s[0], t2 = s[1], w1 = s[2], w2 = s[3];
    var d = t1 - t2, den = 3 - Math.cos(2 * d);
    var a1 = (-3 * G * Math.sin(t1) - G * Math.sin(t1 - 2 * t2)
              - 2 * Math.sin(d) * (w2 * w2 + w1 * w1 * Math.cos(d))) / den;
    var a2 = (2 * Math.sin(d) * (2 * w1 * w1 + 2 * G * Math.cos(t1)
              + w2 * w2 * Math.cos(d))) / den;
    return [w1, w2, a1, a2];
  }
  function rk4(s, h){
    function add(a, b, k){ return [a[0]+b[0]*k, a[1]+b[1]*k, a[2]+b[2]*k, a[3]+b[3]*k]; }
    var k1 = deriv(s), k2 = deriv(add(s, k1, h/2)), k3 = deriv(add(s, k2, h/2)), k4 = deriv(add(s, k3, h));
    return [0,1,2,3].map(function(i){ return s[i] + h/6 * (k1[i] + 2*k2[i] + 2*k3[i] + k4[i]); });
  }

  var runs, t;
  function reset(){
    var sign = Math.random() < 0.5 ? -1 : 1;
    var t1 = sign * (1.9 + Math.random() * 0.8);
    var t2 = t1 + (Math.random() - 0.5) * 1.2;
    runs = [
      { s: [t1, t2, 0, 0],         trail: [], k: 'a' },
      { s: [t1, t2 + 0.001, 0, 0], trail: [], k: 'b' }
    ];
    t = 0;
  }

  function pos(s){
    var x1 = Math.sin(s[0]), y1 = Math.cos(s[0]);
    var x2 = x1 + Math.sin(s[1]), y2 = y1 + Math.cos(s[1]);
    return [[PX, PY], [PX + x1 * SX, PY + y1 * SY], [PX + x2 * SX, PY + y2 * SY]];
  }

  var ch, cl;
  function put(x, y, c, k){
    x = Math.round(x); y = Math.round(y);
    if (x < 0 || y < 0 || x >= W || y >= H) return;
    ch[y][x] = c; cl[y][x] = k;
  }
  function rod(p, q, k){
    var dx = q[0] - p[0], dy = q[1] - p[1];
    var c = Math.abs(dx) < Math.abs(dy) * 0.4 ? '|'
          : Math.abs(dy) < Math.abs(dx) * 0.25 ? '-'
          : (dx * dy > 0 ? '\\' : '/');
    var n = Math.ceil(Math.max(Math.abs(dx), Math.abs(dy)));
    for (var i = 1; i < n; i++) put(p[0] + dx * i / n, p[1] + dy * i / n, c, k);
  }

  function render(){
    ch = []; cl = [];
    for (var y = 0; y < H; y++){
      ch.push(new Array(W).fill(' '));
      cl.push(new Array(W).fill(''));
    }
    runs.forEach(function(r){
      var n = r.trail.length;
      r.trail.forEach(function(p, i){
        var age = 1 - i / n;
        var lvl = age < 0.12 ? 0 : age < 0.35 ? 1 : age < 0.65 ? 2 : 3;
        put(p[0], p[1], '*+:.'[lvl], r.k + lvl);
      });
    });
    // draw run b first so a sits on top while they still overlap
    runs.slice().reverse().forEach(function(r){
      var p = pos(r.s);
      rod(p[0], p[1], r.k + 'r');
      rod(p[1], p[2], r.k + 'r');
      put(p[1][0], p[1][1], 'o', r.k + 'b');
      put(p[2][0], p[2][1], '@', r.k + 'b');
    });
    put(PX - 1, PY, '[', 'pv'); put(PX, PY, '#', 'pv'); put(PX + 1, PY, ']', 'pv');

    var html = '';
    for (var y2 = 0; y2 < H; y2++){
      var cur = null, run = '';
      for (var x = 0; x < W; x++){
        if (cl[y2][x] !== cur){
          if (run) html += cur ? '<span class="' + cur + '">' + run + '</span>' : run;
          cur = cl[y2][x]; run = '';
        }
        run += ch[y2][x];
      }
      if (run) html += cur ? '<span class="' + cur + '">' + run + '</span>' : run;
      html += '\n';
    }
    el.innerHTML = html;

    var d = Math.abs(runs[0].s[1] - runs[1].s[1]);
    out.innerHTML = '<span class="ka">@ run a</span> &nbsp; <span class="kb">@ run b</span> &nbsp; '
      + '<span class="kd">&Delta;&theta;&#8322; ' + d.toFixed(d < 0.01 ? 5 : 2) + ' rad</span>'
      + ' &nbsp; t ' + t.toFixed(1) + 's &nbsp; &middot; click to reset';
  }

  function step(seconds){
    var n = Math.round(seconds / DT);
    for (var i = 0; i < n; i++){
      runs.forEach(function(r){ r.s = rk4(r.s, DT); });
      t += DT;
      if (i % 4 === 0) runs.forEach(function(r){
        var p = pos(r.s)[2];
        r.trail.push([p[0], p[1]]);
        if (r.trail.length > TRAIL) r.trail.shift();
      });
    }
  }

  reset();
  el.parentNode.addEventListener('click', function(){ reset(); render(); });

  if (window.matchMedia && window.matchMedia('(prefers-reduced-motion: reduce)').matches){
    step(12); render();
    el.parentNode.addEventListener('click', function(){ step(12); render(); });
    return;
  }

  var last = null;
  function frame(now){
    if (last !== null) step(Math.min((now - last) / 1000, 0.05));
    last = now;
    if (t > RESET_AFTER) reset();
    render();
    requestAnimationFrame(frame);
  }
  requestAnimationFrame(frame);
})();
</script>

<div class="dm-copy">

</div>