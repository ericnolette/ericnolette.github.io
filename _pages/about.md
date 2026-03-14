---
permalink: /about
layout: page
title: About
---

<style>
.dm-hero {
  margin: 48px 0 32px;
}

.dm-caption {
  font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;
  font-size: 12px;
  color: #7a7f85;
  margin-bottom: 16px;
}

.dm-wrap {
  display: inline-block;
  overflow-x: auto;
}

.dm-ascii {
  font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;
  font-size: 14px;
  line-height: 1.05;
  white-space: pre;
  margin: 0;
  background: transparent !important;
  border: none !important;
  box-shadow: none !important;
  padding: 0 !important;
  color: #48D597;
}

.s { color: #48D597; }     /* Oxide green */
.sh { color: #236A4C; }    /* darker green */
.lb { color: #5B5F61; }    /* bracket */
.lt { color: #A1A4A5; }    /* label text */
.ac { color: #48D597; }    /* accent green */
.acd { color: #236A4C; }   /* dim accent */

.flow1 { animation: flow 2.6s ease-in-out infinite 0s; }
.flow2 { animation: flow 2.6s ease-in-out infinite .35s; }
.flow3 { animation: flow 2.6s ease-in-out infinite .7s; }
.flow4 { animation: flow 2.6s ease-in-out infinite 1.05s; }
.flow5 { animation: flow 2.6s ease-in-out infinite 1.4s; }

.state {
  animation: blink 1.2s steps(2, end) infinite;
}

@keyframes flow {
  0%, 100% {
    color: #236A4C;
    opacity: .55;
    text-shadow: none;
  }
  45%, 60% {
    color: #48D597;
    opacity: 1;
    text-shadow: 0 0 8px rgba(72, 213, 151, .25);
  }
}

@keyframes blink {
  0%, 49% {
    color: #48D597;
    opacity: 1;
    text-shadow: 0 0 8px rgba(72, 213, 151, .25);
  }
  50%, 100% {
    color: #236A4C;
    opacity: .55;
    text-shadow: none;
  }
}

.dm-sub {
  margin-top: 14px;
  font-size: 12px;
  letter-spacing: .14em;
  text-transform: uppercase;
  color: #7a7f85;
}

.dm-copy {
  max-width: 760px;
  margin-top: 30px;
}
</style>

<div class="dm-hero">
  <div class="dm-caption">Fig 1. DataMachine Layout</div>

  <div class="dm-wrap">
<pre class="dm-ascii">
<span class="s">+----------------+.</span>
<span class="s">|`.</span>              <span class="sh">|</span> <span class="s">`.</span>
<span class="s">|</span>  <span class="s">`+----------------+</span>
<span class="s">|</span>   <span class="s">|</span> DATAMACHINE <span class="sh">|</span>  <span class="s">|</span><span class="lb">[</span><span class="lt">IO</span><span class="lb">]</span>
<span class="s">|</span>   <span class="s">|</span><span class="acd">────────────</span><span class="s">|</span>
<span class="s">|</span><span class="sh">---</span><span class="s">|</span><span class="sh">-</span><span class="ac">feeds</span><span class="sh">.---</span><span class="s">+.</span>  <span class="s">|</span>
<span class="s">|</span>   <span class="s">|</span><span class="ac">logs</span>     <span class="ac">ext</span>   <span class="s">|</span>
<span class="s">|</span>   <span class="s">|</span>raw      bus <span class="sh">|</span>   <span class="s">+---+</span>
<span class="s">|</span>   <span class="s">|</span>trace    link <span class="sh">|</span>   <span class="s">|</span>
<span class="s">+</span><span class="sh">---</span><span class="s">|</span><span class="sh">---</span><span class="flow1">+</span><span class="sh">.--+.--</span><span class="s">|.</span>
 <span class="s">`.</span> <span class="s">|</span>    <span class="sh">|</span> <span class="sh">`.</span>  <span class="sh">`.</span><span class="s">|</span> <span class="s">`.</span>
   <span class="s">`+--------+</span><span class="flow2">-</span><span class="s">--+</span><span class="flow3">-</span><span class="s">--+</span>
         <span class="s">|</span>   <span class="s">|</span>   <span class="sh">|</span>   <span class="s">|</span><span class="lb">[</span><span class="lt">BUS</span><span class="lb">]</span>
         <span class="s">|</span>   <span class="s">|</span>   <span class="sh">|</span>   <span class="s">|</span>
    <span class="s">+----+.</span><span class="sh">--</span><span class="s">|</span><span class="sh">---</span><span class="flow4">╱</span><span class="sh">.</span>  <span class="s">|</span>
    <span class="s">|`.</span>    <span class="s">`.|</span>     <span class="sh">`.</span><span class="s">|</span>
    <span class="s">|</span>  <span class="s">+-----+---+---+</span>
    <span class="s">|</span>  <span class="s">|</span> node <span class="sh">|</span>   <span class="s">|</span><span class="lb">[</span><span class="lt">NODE</span><span class="lb">]</span>
    <span class="s">|</span>  <span class="s">|</span> core <span class="sh">|</span>   <span class="s">|</span>
<span class="s">+---+</span><span class="sh">--</span><span class="s">|</span><span class="sh">-----+.--</span><span class="s">|.</span>
<span class="s">|`.</span>  <span class="s">`.|</span> link  <span class="sh">`.</span><span class="s">|</span> <span class="s">`.</span>
<span class="s">|</span>  <span class="s">`+--+---------+---+</span>
<span class="s">|</span>   <span class="s">|</span><span class="flow5">~&gt;</span> trace     <span class="sh">|</span>   <span class="s">|</span><span class="lb">[</span><span class="lt">CORE</span><span class="lb">]</span>
<span class="s">|</span>   <span class="s">|</span><span class="acd">log</span>       <span class="sh">|</span>   <span class="s">|</span>
<span class="s">|</span><span class="sh">---</span><span class="s">|</span><span class="acd">archive</span><span class="sh">--+.</span>  <span class="s">|</span>
<span class="s">|</span>   <span class="s">|</span>  <span class="sh">|</span> <span class="sh">`.</span>        <span class="sh">`.</span><span class="s">|</span>
<span class="s">|</span>   <span class="s">|</span>  <span class="sh">|</span>   <span class="s">+---------+</span>
<span class="s">|</span>   <span class="s">|</span>  <span class="sh">|</span>   <span class="state">STATE</span>
<span class="s">|</span>   <span class="s">|</span>  <span class="sh">|</span>   watch
<span class="s">+</span><span class="sh">---</span><span class="s">|</span><span class="sh">--+.</span>  <span class="s">|</span>
 <span class="s">`.</span> <span class="s">|</span>    <span class="sh">`.</span><span class="s">|</span>
   <span class="s">`+------+</span>
</pre>
  </div>

</div>

<div class="dm-copy">

</div>