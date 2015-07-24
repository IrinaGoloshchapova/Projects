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
<!-- Fri Jul 24 22:31:48 2015 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataGaugeID1c6c9063a3c () {
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
function drawChartGaugeID1c6c9063a3c() {
var data = gvisDataGaugeID1c6c9063a3c();
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
    document.getElementById('GaugeID1c6c9063a3c')
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
callbacks.push(drawChartGaugeID1c6c9063a3c);
})();
function displayChartGaugeID1c6c9063a3c() {
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
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartGaugeID1c6c9063a3c"></script>
 
<!-- divChart -->
  
<div id="GaugeID1c6c9063a3c" 
  style="width: 400; height: 600;">
</div>

---
## System Bank crisis probability

<iframe src="https://plot.ly/~IrinaGoloshchapova/40/none/" width="800" height="500" scrolling="no" frameBorder="0"></iframe>

<span class="footnote">Data source: CMASF</span>

---
## System bank crisis probability 
Playing with Google Graphics

<!-- AnnotationChart generated in R 3.2.1 by googleVis 0.5.9 package -->
<!-- Fri Jul 24 22:31:48 2015 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataAnnotationChartID1c6c446251a9 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 new Date(2014,0,1),
0.133,
0.11 
],
[
 new Date(2014,1,1),
0.136,
0.116 
],
[
 new Date(2014,2,1),
0.13,
0.116 
],
[
 new Date(2014,3,1),
0.123,
0.122 
],
[
 new Date(2014,4,1),
0.121,
0.132 
],
[
 new Date(2014,5,1),
0.113,
0.125 
],
[
 new Date(2014,6,1),
0.112,
0.12 
],
[
 new Date(2014,7,1),
0.112,
0.123 
],
[
 new Date(2014,8,1),
0.107,
0.108 
],
[
 new Date(2014,9,1),
0.109,
0.11 
],
[
 new Date(2014,10,1),
0.11,
0.103 
],
[
 new Date(2014,11,1),
0.105,
0.099 
],
[
 new Date(2015,0,1),
0.11,
0.104 
],
[
 new Date(2015,1,1),
0.099,
0.118 
],
[
 new Date(2015,2,1),
0.087,
0.131 
],
[
 new Date(2015,3,1),
0.083,
0.145 
],
[
 new Date(2015,4,1),
0.088,
0.162 
] 
];
data.addColumn('date','date');
data.addColumn('number','bank.crisis.indicator');
data.addColumn('number','bank.crisis.ending.indicator');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartAnnotationChartID1c6c446251a9() {
var data = gvisDataAnnotationChartID1c6c446251a9();
var options = {};
options["width"] =    600;
options["height"] =    350;
options["fill"] =     10;
options["displayExactValues"] = true;
options["colors"] = ['#0000ff','#00ff00'];

    var chart = new google.visualization.AnnotationChart(
    document.getElementById('AnnotationChartID1c6c446251a9')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "annotationchart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartAnnotationChartID1c6c446251a9);
})();
function displayChartAnnotationChartID1c6c446251a9() {
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
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAnnotationChartID1c6c446251a9"></script>
 
<!-- divChart -->
  
<div id="AnnotationChartID1c6c446251a9" 
  style="width: 600; height: 350;">
</div>

