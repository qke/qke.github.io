---
layout: page
---

<script src="https://d3js.org/d3.v3.min.js"></script>
<script>
d3.text("top_sb_aps.tsv", function(data) {
    var parsedTSV = d3.tsv.parseRows(data);
    var table = d3.select("#top_sb_aps")
    .append("table")
    .style("border-collapse", "collapse")
    .style("border", "2px black solid")
    .selectAll("tr")
    .data(parsedTSV)
    .enter()
    .append("tr")
    .on("mouseover", function(){d3.select(this).style("background-color", "Aquamarine")})
    .on("mouseout", function(){d3.select(this).style("background-color", "white")})
    .selectAll("td")
    .data(function(d){return d;})
    .enter()
    .append("td")
    .style("border", "1px black solid")
    .style("padding", "5px")
    .text(function(d){return d;})
    .style("font-size", "12px");
});
</script>

### Top 100 Sleeping Beauties in Physics

This list is derived based on the [APS dataset](http://journals.aps.org/datasets).

[Get the data](top_sb_aps.tsv)

[back](/projects/beauty/beauty.html)

<div id="top_sb_aps"></div>
