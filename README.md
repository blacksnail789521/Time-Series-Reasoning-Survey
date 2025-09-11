# A Survey of Reasoning and Agentic Systems in Time Series with Large Language Models

Time series reasoning treats time as a first-class axis and integrates intermediate evidence into the answer itself.  
This survey organizes the field along two levels:

* **Reasoning Topology** — execution structures:  
  * Direct reasoning (single step)  
  * Linear chain reasoning (sequential intermediate steps)  
  * Branch-structured reasoning (exploration, feedback, and aggregation)  

* **Primary Objective** — the main intent:  
  * Traditional time series analysis (forecasting, classification, anomaly detection, segmentation)  
  * Explanation and understanding (temporal QA, diagnostics, structure discovery)  
  * Causal inference and decision making (counterfactuals, policy evaluation, decision support)  
  * Time series generation (simulation, editing, synthesis)  

We complement this two-level taxonomy with **attribute tags** that capture control-flow operators (decomposition, verification, ensembling), execution actors (tool use, agents), information sources (knowledge access, multimodality), and alignment regimes (prompting, supervised finetuning, reinforcement/preference, hybrid).

This repository curates and classifies papers in the field.  
The following table presents the unified taxonomy and tags for all papers we review.

---

## Curated Papers

<div class="tg-wrap"><table id="tg-ZCaZj"><thead>
  <tr>
    <th>Paper</th>
    <th>Reasoning Topology</th>
    <th>Primary Objective</th>
    <th>Primary Objective Subcategory</th>
    <th>T-Dec</th>
    <th>T-Ver</th>
    <th>T-Ens</th>
    <th>T-Tool</th>
    <th>T-Know</th>
    <th>T-Multi</th>
    <th>T-Agent</th>
    <th>T-Align</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Large Language Models Are   Zero-Shot Time Series Forecasters</td>
    <td>Direct Reasoning</td>
    <td>Traditional Time Series Analysis</td>
    <td>Forecasting</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>TRUE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>0</td>
    <td>P</td>
  </tr>
  <tr>
    <td>Context is Key: A Benchmark   for Forecasting with Essential Textual Information</td>
    <td>Direct Reasoning</td>
    <td>Traditional Time Series Analysis</td>
    <td>Forecasting</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>TRUE</td>
    <td>0</td>
    <td>P</td>
  </tr>
  <tr>
    <td>DP-GPT4MTS: Dual-Prompt Large   Language Model for Textual-Numerical Time Series Forecasting</td>
    <td>Direct Reasoning</td>
    <td>Traditional Time Series Analysis</td>
    <td>Forecasting</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>TRUE</td>
    <td>0</td>
    <td>S</td>
  </tr>
  <tr>
    <td>TEMPO: PROMPT-BASED GENERATIVE   PRE-TRAINED TRANSFORMER FOR TIME SERIES FORECASTING</td>
    <td>Direct Reasoning</td>
    <td>Traditional Time Series Analysis</td>
    <td>Forecasting</td>
    <td>TRUE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>FALSE</td>
    <td>TRUE</td>
    <td>0</td>
    <td>S</td>
  </tr>
</tbody></table></div>
<script charset="utf-8">var TGSort=window.TGSort||function(n){"use strict";function r(n){return n?n.length:0}function t(n,t,e,o=0){for(e=r(n);o<e;++o)t(n[o],o)}function e(n){return n.split("").reverse().join("")}function o(n){var e=n[0];return t(n,function(n){for(;!n.startsWith(e);)e=e.substring(0,r(e)-1)}),r(e)}function u(n,r,e=[]){return t(n,function(n){r(n)&&e.push(n)}),e}var a=parseFloat;function i(n,r){return function(t){var e="";return t.replace(n,function(n,t,o){return e=t.replace(r,"")+"."+(o||"").substring(1)}),a(e)}}var s=i(/^(?:\s*)([+-]?(?:\d+)(?:,\d{3})*)(\.\d*)?$/g,/,/g),c=i(/^(?:\s*)([+-]?(?:\d+)(?:\.\d{3})*)(,\d*)?$/g,/\./g);function f(n){var t=a(n);return!isNaN(t)&&r(""+t)+1>=r(n)?t:NaN}function d(n){var e=[],o=n;return t([f,s,c],function(u){var a=[],i=[];t(n,function(n,r){r=u(n),a.push(r),r||i.push(n)}),r(i)<r(o)&&(o=i,e=a)}),r(u(o,function(n){return n==o[0]}))==r(o)?e:[]}function v(n){if("TABLE"==n.nodeName){for(var a=function(r){var e,o,u=[],a=[];return function n(r,e){e(r),t(r.childNodes,function(r){n(r,e)})}(n,function(n){"TR"==(o=n.nodeName)?(e=[],u.push(e),a.push(n)):"TD"!=o&&"TH"!=o||e.push(n)}),[u,a]}(),i=a[0],s=a[1],c=r(i),f=c>1&&r(i[0])<r(i[1])?1:0,v=f+1,p=i[f],h=r(p),l=[],g=[],N=[],m=v;m<c;++m){for(var T=0;T<h;++T){r(g)<h&&g.push([]);var C=i[m][T],L=C.textContent||C.innerText||"";g[T].push(L.trim())}N.push(m-v)}t(p,function(n,t){l[t]=0;var a=n.classList;a.add("tg-sort-header"),n.addEventListener("click",function(){var n=l[t];!function(){for(var n=0;n<h;++n){var r=p[n].classList;r.remove("tg-sort-asc"),r.remove("tg-sort-desc"),l[n]=0}}(),(n=1==n?-1:+!n)&&a.add(n>0?"tg-sort-asc":"tg-sort-desc"),l[t]=n;var i,f=g[t],m=function(r,t){return n*f[r].localeCompare(f[t])||n*(r-t)},T=function(n){var t=d(n);if(!r(t)){var u=o(n),a=o(n.map(e));t=d(n.map(function(n){return n.substring(u,r(n)-a)}))}return t}(f);(r(T)||r(T=r(u(i=f.map(Date.parse),isNaN))?[]:i))&&(m=function(r,t){var e=T[r],o=T[t],u=isNaN(e),a=isNaN(o);return u&&a?0:u?-n:a?n:e>o?n:e<o?-n:n*(r-t)});var C,L=N.slice();L.sort(m);for(var E=v;E<c;++E)(C=s[E].parentNode).removeChild(s[E]);for(E=v;E<c;++E)C.appendChild(s[v+L[E-v]])})})}}n.addEventListener("DOMContentLoaded",function(){for(var t=n.getElementsByClassName("tg"),e=0;e<r(t);++e)try{v(t[e])}catch(n){}})}(document)</script>



---

## How to Contribute

We welcome contributions to keep this table updated:

1. Add missing papers as new rows following the same format.  
2. Ensure each paper is annotated with exactly one **Reasoning Topology** and one **Primary Objective**, plus appropriate tags.  
3. Submit a pull request.

---

## Citation

If you find this resource useful, please cite our survey (bibtex entry forthcoming).
