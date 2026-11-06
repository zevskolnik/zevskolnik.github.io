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
  /* To add a country: add its two-letter code here, and its name to the list below the map */
  const visited = ["MX","IL","CA","US","BZ","PA","EC","CR","CU","JM","FR","ES","IT","CZ","HU","AT","HR","BA","DE","PT","BE","NL","MA","IE","NI","AU","LK","NZ","FJ","GB","MY","ID","TH","JP","PH","NA","ZA","NP","VN","LA","AR","CL","GT","CO","PE","CH"];
  /* Countries too small to see on the map get a dot instead */
  const dots = [
    { name: "Singapore", coords: [1.35, 103.82] },
    { name: "Vatican City", coords: [41.9, 12.45] }
  ];
  new jsVectorMap({
    selector: '#visited-map',
    map: 'world',
    zoomButtons: true,
    selectedRegions: visited,
    regionsSelectable: false,
    markers: dots,
    markerStyle: { initial: { fill: '#2a9d8f', stroke: '#ffffff', r: 4 } },
    regionStyle: { initial: { fill: '#d6d9de' }, selected: { fill: '#2a9d8f' }, hover: { fillOpacity: 0.8 } }
  });
</script>

**48 countries so far:**

- **North & Central America:** Belize, Canada, Costa Rica, Cuba, Guatemala, Jamaica, Mexico, Nicaragua, Panama, USA
- **South America:** Argentina, Chile, Colombia, Ecuador (and the Galápagos), Peru
- **Europe:** Austria, Belgium, Bosnia & Herzegovina (for about 2 seconds), Croatia, Czech Republic, England, France, Germany, Hungary, Ireland, Italy, Netherlands, Portugal, Spain, Switzerland, Vatican City
- **Africa & Middle East:** Israel, Morocco, Namibia, South Africa
- **Asia:** Indonesia, Japan, Laos, Malaysia, Nepal, Philippines, Singapore, Sri Lanka, Thailand, Vietnam
- **Oceania:** Australia, Fiji, New Zealand
