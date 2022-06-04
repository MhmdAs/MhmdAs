<script src="heatmap.js"></script>
<link rel="stylesheet" href="heatmap.css" />
<div id="heatmap"></div>
{
  1.4.2021T0:0:0: 4,
  1.6.2021T0:0:0: 4,
  1.8.2021T0:0:0: 1,
  1.9.2021T0:0:0: 1,
  2.1.2021T0:0:0: 2,
  // ...
}
let heatmap = new HeatmapPlugin('heatmap',data, {
    legend: true,
    timescale: true,
    range: {
        from: '#year#-01-01T00:00:00',
        till: '#year#-12-30T00:00:00',
        grade: 1,
        interval: 'day', //month, year, hours, minutes
        rows: 7,
    },
    units: 5
},{
    width: '10',
    height: '10',
    font: {
      size: '10',
      family: 'Arial',
      color: 'white'
    }
}, true);
