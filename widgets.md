# Nanopub Widgets Demo

<script type="module">
  import { query } from "https://a.knowledgepixels.com/js/nanopub-utils.js";
</script>

---

## Latest Accepted Nanopublications at Biodiversity Data Journal

<ul>
<script type="module">
  query("RAv_j-NWU-lJO0w0xgSzqJwOl3ATWumHqsQhoa2QmR-qQ/get-latest-bdj-nanopubs", bdj_nanopubs_template);
</script>
<li class="nps_temp"><em>(loading...)</em></li>
<template id="bdj_nanopubs_template"><li><span class="nanopub_icon"></span> <a nps_attribute="href=np" target="_blank"><span nps_innerText=label></span></a>, by <a nps_user=mainAuthor></a><span nps_innerText=authorEtAl></span>, <span nps_innerText=date></span></li></template>
</ul>


## Latest Accepted Nanopublications at RIO Journal

<ul>
<script type="module">
  query("RAKYgzEn9t0GOPkHpP0s_fkAHPyQRQcMZXWUH3N5a9urw/get-latest-rio-nanopubs", rio_nanopubs_template);
</script>
<li class="nps_temp"><em>(loading...)</em></li>
<template id="rio_nanopubs_template"><li><span class="nanopub_icon"></span> <a nps_attribute="href=np" target="_blank"><span nps_innerText=label></span></a>, by <a nps_user=mainAuthor></a><span nps_innerText=authorEtAl></span>, <span nps_innerText=date></span></li></template>
</ul>

