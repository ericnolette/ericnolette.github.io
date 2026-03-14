---
permalink: /
layout: home
title: Welcome
---

<style>
.welcome-shell {
  margin-top: 24px;
}

.boot-pre,
.bridge-pre,
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
}

.boot-pre,
.bridge-pre,
.dm-ascii,
.s,
.ac {
  color: #48D597;
}

.sh,
.acd,
.boot-dim {
  color: #236A4C;
}

.lb {
  color: #5B5F61;
}

.lt {
  color: #A1A4A5;
}

.boot-wrap {
  margin-bottom: 18px;
}

.bridge-wrap {
  margin: 14px 0 20px;
}

.blue,
.bridge-node {
  color: #5DA9FF;
  animation: pulseBlue 2.4s ease-in-out infinite;
}

.flow1 { animation: flow 2.6s ease-in-out infinite 0s; }
.flow2 { animation: flow 2.6s ease-in-out infinite .35s; }
.flow3 { animation: flow 2.6s ease-in-out infinite .7s; }
.flow4 { animation: flow 2.6s ease-in-out infinite 1.05s; }
.flow5 { animation: flow 2.6s ease-in-out infinite 1.4s; }

.bridge-flow-1 { animation: bridgeFlow 1.6s linear infinite 0s; }
.bridge-flow-2 { animation: bridgeFlow 1.6s linear infinite .2s; }
.bridge-flow-3 { animation: bridgeFlow 1.6s linear infinite .4s; }
.bridge-flow-4 { animation: bridgeFlow 1.6s linear infinite .6s; }
.bridge-flow-5 { animation: bridgeFlow 1.6s linear infinite .8s; }
.bridge-flow-6 { animation: bridgeFlow 1.6s linear infinite 1s; }

.state {
  animation: blinkRed 1s steps(2, end) infinite;
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

@keyframes bridgeFlow {
  0%, 100% {
    color: #236A4C;
    opacity: .35;
    text-shadow: none;
  }
  50% {
    color: #48D597;
    opacity: 1;
    text-shadow: 0 0 8px rgba(72, 213, 151, .25);
  }
}

@keyframes blinkRed {
  0%, 49% {
    color: #ff4d5a;
    opacity: 1;
    text-shadow: 0 0 10px rgba(255, 77, 90, .45);
  }
  50%, 100% {
    color: #7a2028;
    opacity: .55;
    text-shadow: none;
  }
}

@keyframes pulseBlue {
  0% {
    color: #4A7CFF;
    text-shadow:
      0 0 3px rgba(93,169,255,.25),
      0 0 6px rgba(93,169,255,.15);
  }
  50% {
    color: #79BDFF;
    text-shadow:
      0 0 8px rgba(93,169,255,.6),
      0 0 18px rgba(93,169,255,.35),
      0 0 28px rgba(93,169,255,.25);
  }
  100% {
    color: #4A7CFF;
    text-shadow:
      0 0 3px rgba(93,169,255,.25),
      0 0 6px rgba(93,169,255,.15);
  }
}
</style>

<div class="welcome-shell">

  <div class="boot-wrap">
<pre class="boot-pre">┌─[BOOT FLOW]───────────────────────────┐
│                                       │
│                                       │
│   ┌─[SP]────────┐                     │
│   │            │                      │
│   │ ▊▊▊▊▊▊▊▊▊▊ │                Λ     │
│   │ ▊▊▊▊▊▊▊▊▊▊ │               ╱ ╲    │
│   │ ▊▊▊▊▊▊▊▊▊▊ │    ├──────────────   │
│   │ ▊▊▊▊▊▊▊▊▊▊ │               ╲ ╱    │
│   │ ▊▊▊▊▊▊▊▊▊▊ │                      │
└───────────────────────────────────────┘</pre>
  </div>

  <div class="bridge-wrap">
<pre class="bridge-pre">          <span class="bridge-node">+</span><span class="bridge-flow-1">-</span><span class="bridge-flow-2">-</span><span class="bridge-flow-3">-</span><span class="bridge-flow-4">-</span><span class="bridge-node">+</span><span class="bridge-flow-2">-</span><span class="bridge-flow-3">-</span><span class="bridge-flow-4">-</span><span class="bridge-flow-5">-</span><span class="bridge-node">+</span><span class="bridge-flow-3">-</span><span class="bridge-flow-4">-</span><span class="bridge-flow-5">-</span><span class="bridge-flow-6">-</span><span class="bridge-node">+</span></pre>
  </div>

  <div class="dm-wrap">
<pre class="dm-ascii"><span class="s">+----------------</span><span class="blue">+</span><span class="s">.</span>
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
   <span class="s">`+------+</span></pre>
  </div>

</div>