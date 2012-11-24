Apply geocoding in R with GeoPlot and GoogleVis
========================================================




Importing data and Recoding




Geocoding: using the package geoPlot to get the latitude and longitude through zip code of patients


```r
geoLoc <- data.frame(zip = c(1:nrow(hpvData)), lat = c(1:nrow(hpvData)), long = c(1:nrow(hpvData)))

for (i in 1:nrow(hpvData)) {
    
    hpvGeo <- geoAddress(c("", "", as.character(hpvData$city[i]), as.character(hpvData$state[i]), 
        as.character(hpvData$zip_code[i]), "BR"))
    
    geoLoc$zip[i] <- hpvGeo$address
    geoLoc$lat[i] <- hpvGeo$latitude
    geoLoc$long[i] <- hpvGeo$longitude
    
}
```



You can also embed plots, for example:

<!-- Map generated in R 2.15.1 by googleVis 0.3.3 package -->
<!-- Sat Nov 24 16:54:00 2012 -->


<!-- jsHeader -->
<script type="text/javascript" src="http://www.google.com/jsapi">
</script>
<script type="text/javascript">
 
// jsData 
function gvisDataMapID16c571cfed31 ()
{
  var data = new google.visualization.DataTable();
  var datajson =
[
 [
 -9.5449382,
-35.7263551,
" \"Maceió\" \"Alagoas\" \"57085-737" 
],
[
 -9.5449382,
-35.7263551,
" \"Maceió\" \"Alagoas\" \"57085-737" 
],
[
 -9.538284,
-35.7161158,
" \"Maceió\" \"Alagoas\" \"57084-655" 
],
[
 -9.5545308,
-35.7884464,
" \"Maceió\" \"Alagoas\" \"57084-083" 
],
[
 -9.5699791,
-35.7338613,
" \"Maceió\" \"Alagoas\" \"57084-052" 
],
[
 -9.5545308,
-35.7884464,
" \"Maceió\" \"Alagoas\" \"57084-083" 
],
[
 -9.509315,
-35.793903,
" \"Maceió\" \"Alagoas\" \"57086-288" 
],
[
 -9.509315,
-35.793903,
" \"Maceió\" \"Alagoas\" \"57086-177" 
],
[
 -9.538284,
-35.7161158,
" \"Maceió\" \"Alagoas\" \"57084-121" 
],
[
 -9.538284,
-35.7161158,
" \"Maceió\" \"Alagoas\" \"57084-612" 
],
[
 -9.5544984,
-35.7284028,
" \"Maceió\" \"Alagoas\" \"57084-800" 
],
[
 -9.538284,
-35.7161158,
" \"Maceió\" \"Alagoas\" \"57084-792" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57084-792" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57084-800" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57086-246" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57086-042" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57086-476" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57085-500" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57086-024" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57086-194" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57084-792" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57084-792" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57086-158" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57084-421" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57085-062" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57084-100" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57084-027" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57084-612" 
],
[
 -9.509315,
-35.793903,
" \"Maceió\" \"Alagoas\" \"57086-146" 
],
[
 -9.5701256,
-35.7618271,
" \"Maceió\" \"Alagoas\" \"57084-040" 
],
[
 -9.5624951,
-35.7208942,
" \"Maceió\" \"Alagoas\" \"57085-018" 
],
[
 -9.5517523,
-35.7318156,
" \"Maceió\" \"Alagoas\" \"57084-780" 
],
[
 -9.538284,
-35.7161158,
" \"Maceió\" \"Alagoas\" \"57084-810" 
],
[
 -9.5624951,
-35.7208942,
" \"Maceió\" \"Alagoas\" \"57085-480" 
],
[
 -9.53773,
-35.7563829,
" \"Maceió\" \"Alagoas\" \"57073-451" 
],
[
 -9.509315,
-35.793903,
" \"Maceió\" \"Alagoas\" \"57086-056" 
],
[
 -9.509315,
-35.793903,
" \"Maceió\" \"Alagoas\" \"57086-462" 
],
[
 -9.5701256,
-35.7618271,
" \"Maceió\" \"Alagoas\" \"57084-040" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57084-134" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57085-030" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57086-106" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57085-030" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57086-434" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57085-030" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57086-448" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57084-081" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57085-753" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57086-448" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57084-648" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57084-653" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57085-753" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57084-248" 
],
[
 0,
0,
" \"Maceió\" \"Alagoas\" \"57020-250" 
],
[
 -9.538284,
-35.7161158,
" \"Maceió\" \"Alagoas\" \"57084-086" 
],
[
 -9.538284,
-35.7161158,
" \"Maceió\" \"Alagoas\" \"57084-622" 
],
[
 -9.538284,
-35.7161158,
" \"Maceió\" \"Alagoas\" \"57084-023" 
],
[
 -9.5449382,
-35.7263551,
" \"Maceió\" \"Alagoas\" \"57085-737" 
] 
];
data.addColumn('number','Latitude');
data.addColumn('number','Longitude');
data.addColumn('string','label');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartMapID16c571cfed31() {
  var data = gvisDataMapID16c571cfed31();
  var options = {};
options["showTip"] = true;
options["mapType"] = "normal";
options["enableScrollWheel"] = true;
options["zoomLevel"] =     15;

     var chart = new google.visualization.Map(
       document.getElementById('MapID16c571cfed31')
     );
     chart.draw(data,options);
    

}
  
 
// jsDisplayChart 
function displayChartMapID16c571cfed31()
{
  google.load("visualization", "1", { packages:["map"] }); 
  google.setOnLoadCallback(drawChartMapID16c571cfed31);
}
 
// jsChart 
displayChartMapID16c571cfed31()
 
<!-- jsFooter -->  
//-->
</script>
 
<!-- divChart -->
  
<div id="MapID16c571cfed31"
  style="width: 600px; height: 500px;">
</div>


