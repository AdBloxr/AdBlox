---
title: Scanning your browser...
filename: Browser-Scan.md
--- 
<style>
.fa-beat {
  animation:fa-beat 5s ease infinite;
}
@keyframes fa-beat {
  0% {
    transform:scale(1);
  }
  5% {
    transform:scale(1.25);
  }
  20% {
    transform:scale(1);
  }
  30% {
    transform:scale(1);
  }
  35% {
    transform:scale(1.25);
  }
  50% {
    transform:scale(1);
  }
  55% {
    transform:scale(1.25);
  }
  70% {
    transform:scale(1);
  }
}






body {
  text-align:center;
  background:white;
  color:#a0a9b8;
  font:1em sans-serif;
}


.heart {
  color:#ffd119;
}

a {
    color:#a0a9b8;
}
</style>
  <div style="font-size: 35px;">
<p class="heart">
  <i class="fa fa-bolt fa-4x fa-beat"></i>
</p>
  </div>
<h1>Checking your browser before accessing AdBlox.</h1>
<h2>
  This process is automatic. Your browser will redirect to your requested content shortly.</h2>
<div style="font-size: 20px;">
<h3>Please allow up to 5 seconds…</h3>
</div>
<div style="font-size: 19px;">
  <h3>LightningBlox Ray ID: <a href="javascript:generateRay();" id="demo">Loading ID</a></h3>
  </div>
  <script>function generateRay() {
        var hash = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ012346789";
        var random8 = '';
        for(var i = 0; i < 5; i++){
            random8 += hash[parseInt(Math.random()*hash.length)];
        }
        console.log(random8);
    document.getElementById("demo").innerHTML = ""+random8;
}        
        
window.onload=function(){
  document.getElementById("demo").click();
};

 var date = new Date();
 var minutes = 30;
 date.setTime(date.getTime() + (minutes * 60 * 1000));

document.cookie = "BrowserScan=Passed; expires= date ";

         setTimeout(function(){
            window.location.href = 'https://lightningblox.github.io/AdBlox/';
         }, 9000);</script>
