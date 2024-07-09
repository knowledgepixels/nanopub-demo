# Nanopub Widgets Demo

---

## Latest Accepted Nanopublications at Biodiversity Data Journal

<ul>
<script type="module">
  import { query } from "https://a.knowledgepixels.com/js/nanopub-utils.js";
  query("RAv_j-NWU-lJO0w0xgSzqJwOl3ATWumHqsQhoa2QmR-qQ/get-latest-bdj-nanopubs", bdj_nanopubs_template);
</script>
<li class="nps_temp"><em>(loading...)</em></li>
<template id="bdj_nanopubs_template"><li><span class="nanopub_icon"></span> <a nps_attribute="href=np" target="_blank"><span nps_innerText=label></span></a>, by <a nps_user=mainAuthor>unknown authors</a><span nps_innerText=authorEtAl></span>, <span nps_innerText=date></span></li></template>
</ul>


## Latest Accepted Nanopublications at RIO Journal

<ul>
<script type="module">
  import { query } from "https://a.knowledgepixels.com/js/nanopub-utils.js";
  query("RAKYgzEn9t0GOPkHpP0s_fkAHPyQRQcMZXWUH3N5a9urw/get-latest-rio-nanopubs", rio_nanopubs_template);
</script>
<li class="nps_temp"><em>(loading...)</em></li>
<template id="rio_nanopubs_template"><li><span class="nanopub_icon"></span> <a nps_attribute="href=np" target="_blank"><span nps_innerText=label></span></a>, by <a nps_user=mainAuthor>unknown authors</a><span nps_innerText=authorEtAl></span>, <span nps_innerText=date></span></li></template>
</ul>


## Latest Accepted Nanopublications at Data Science

<ul>
<script type="module">
  import { query } from "https://a.knowledgepixels.com/js/nanopub-utils.js";
  query("RAWs8m60l7Qk6P0RHhoZK_6cSMzuGO27zLYiZF-QnkhAg/get-latest-ds-nanopubs", ds_nanopubs_template);
</script>
<li class="nps_temp"><em>(loading...)</em></li>
<template id="ds_nanopubs_template"><li><span class="nanopub_icon"></span> <a nps_attribute="href=np" target="_blank"><span nps_innerText=label></span></a>, by <a nps_user=mainAuthor>unknown authors</a><span nps_innerText=authorEtAl></span>, <span nps_innerText=date></span></li></template>
</ul>


## Nanopublication Count per Journal

<ul>
<script type="module">
  import { query } from "https://a.knowledgepixels.com/js/nanopub-utils.js";
  query("RAAllx86xmfVXUeOsduOTdl2RdekO5MjYRUM-JOFSfbVM/get-np-count-per-journal", nanopub_count_template);
</script>
<li class="nps_temp"><em>(loading...)</em></li>
<template id="nanopub_count_template"><li><span nps_innerText=journal></span>: <span nps_innerText=npcount></span></li></template>
</ul>


## Top 10 Authors of Accepted Nanopublications

<ul>
<script type="module">
  import { query } from "https://a.knowledgepixels.com/js/nanopub-utils.js";
  query("RACx9IgQMsU3UZqrGlYk6efLg5jJTFldTrXypwTTJbo40/get-top-authors", top_authors_template);
</script>
<li class="nps_temp"><em>(loading...)</em></li>
<template id="top_authors_template"><li><a nps_user=author></a>: <span nps_innerText=npcount></span></li></template>
</ul>


## Most Used Taxons in Biodiversity Data Journal

<ul>
<script type="module">
  import { query } from "https://a.knowledgepixels.com/js/nanopub-utils.js";
  query("RAINZUI4_X5lNQpOfu1446e8qmZRV2clJ9KNrUUqsTYW4/get-most-used-bdj-taxons", most_used_taxons);
</script>
<li class="nps_temp"><em>(loading...)</em></li>
<template id="most_used_taxons"><li><a nps_innerText=taxonNameLabel nps_attribute="href=taxonName"></a>: <span nps_innerText=taxonNameCount></span></li></template>
</ul>

## Top 10 Creators of the Last 30 Days

<ul>
<script type="module">
  import { query } from "https://a.knowledgepixels.com/js/nanopub-utils.js";
  query("RAna6AB9majJbslfFCtrZaM3_QPKzeDnOUsbGOx2LUgfE/get-top-creators-last30d", top_creators_template);
</script>
<li class="nps_temp"><em>(loading...)</em></li>
<template id="top_creators_template"><li><a nps_user=userid></a>: <span nps_innerText=count></span></li></template>
</ul>

