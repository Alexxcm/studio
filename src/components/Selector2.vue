<template>
<html>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <body>
    <div class="bg-image img1"></div>
    <div class="bg-image img2"></div>
    <div class="bg-image img3"></div>
    <div class="bg-image img4"></div>
    <div class="bg-image img5"></div>
    <div class="bg-image img6"></div>
</body></html>
</template>

<script>
export default {
  name: 'Selector2'
}
</script>

<style>
body, html {
  height: 100%;
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
}

* {
  box-sizing: border-box;
}
.bg-image {
  /* Full height */
  height: 50%;
  /* Center and scale the image nicely */
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

/* Images used */
.img1 { background-image: url("../assets/ca1.jpg"); }
.img2 { background-image: url("../assets/ca2.jpg"); }
.img3 { background-image: url("../assets/ca3.jpg"); }
.img4 { background-image: url("../assets/ca1.jpg"); }
.img5 { background-image: url("../assets/ca2.jpg"); }
.img6 { background-image: url("../assets/ca3.jpg"); }

/* Position text in the middle of the page/image */
</style>
