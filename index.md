---
title       : CMASF Graphics Example
subtitle    : 
author      : Irina Goloshchapova
job         : Expert
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Crisis Pulse
- 3 - high probability
- 2 - medium probability
- 1 - low probability

<!-- Gauge generated in R 3.2.1 by googleVis 0.5.9 package -->
<!-- Fri Jul 24 18:04:28 2015 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataGaugeID1c7c71491bcc () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "Crisis",
3 
],
[
 "NPL",
3 
],
[
 "Liquidity",
1 
],
[
 "Exch.rate",
2 
] 
];
data.addColumn('string','Indicator');
data.addColumn('number','Probability');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartGaugeID1c7c71491bcc() {
var data = gvisDataGaugeID1c7c71491bcc();
var options = {};
options["allowHtml"] = true;
options["min"] =      0;
options["max"] =      3;
options["greenFrom"] =      0;
options["greenTo"] =    1.5;
options["yellowFrom"] =    1.5;
options["yellowTo"] =    2.5;
options["redFrom"] =    2.5;
options["redTo"] =      3;
options["width"] =    400;
options["height"] =    600;

    var chart = new google.visualization.Gauge(
    document.getElementById('GaugeID1c7c71491bcc')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "gauge";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartGaugeID1c7c71491bcc);
})();
function displayChartGaugeID1c7c71491bcc() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartGaugeID1c7c71491bcc"></script>
 
<!-- divChart -->
  
<div id="GaugeID1c7c71491bcc" 
  style="width: 400; height: 600;">
</div>

---
## System Bank crisis probability

<iframe src="https://plot.ly/~IrinaGoloshchapova/40/none/" width="800" height="500" scrolling="no" frameBorder="0"></iframe>

<span class="footnote">Data source: CMASF</span>

---
