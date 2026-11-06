---
title: Countries Visited
icon: fas fa-globe-americas
order: 4
---

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/jsvectormap@1.6.0/dist/jsvectormap.min.css">
<div id="visited-map" style="height: 420px; margin-bottom: 1.5rem;"></div>
<script src="https://cdn.jsdelivr.net/npm/jsvectormap@1.6.0/dist/jsvectormap.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/jsvectormap@1.6.0/dist/maps/world.js"></script>
<script>
  /* Add a country by adding its two-letter code to this list */
  const visited = ["NZ","MX","LK","SG","EC","NI","JM","BZ","PA","CR","CU","MA","AT","NL","CZ","IE","PT","IT","BA","HR","DE","ES","FR","BE","HU","AU","CA","US"];
  new jsVectorMap({
    selector: '#visited-map',
    map: 'world',
    zoomButtons: true,
    selectedRegions: visited,
    regionsSelectable: false,
    regionStyle: { initial: { fill: '#d6d9de' }, selected: { fill: '#2a9d8f' }, hover: { fillOpacity: 0.8 } }
  });
</script>

**28 countries so far:** Australia, Austria, Belgium, Belize, Bosnia & Herzegovina, Canada, Costa Rica, Croatia, Cuba, Czechia, Ecuador, France, Germany, Hungary, Ireland, Italy, Jamaica, Mexico, Morocco, Netherlands, New Zealand, Nicaragua, Panama, Portugal, Singapore, Spain, Sri Lanka, United States
