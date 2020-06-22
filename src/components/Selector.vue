<template>
<div>
   <b-container fluid>
  <b-row>
    <b-col max-height = "180px" class="col-lg-4 col-md-6 col-sm-12">
      <b-img rounded="circle" class = "image" thumbnail fluid :src="require('../assets/sel1.jpg')" alt="Image 1"></b-img>

    </b-col>
    <b-col class="col-lg-4 col-md-6 col-sm-12">
        <router-link to="/About">
      <b-img rounded="circle" class = "image" thumbnail fluid :src="require('../assets/sel2.jpg')" alt="Image 2"></b-img>
        </router-link>
    </b-col>
    <b-col class="col-lg-4 col-md-6 col-sm-12">
      <b-img rounded="circle" class = "image" thumbnail fluid :src="require('../assets/sel3.png')" alt="Image 3"></b-img>
    </b-col>
    <b-col class="col-lg-4 col-md-6 col-sm-12">
      <b-img rounded="circle" class = "image" thumbnail fluid :src="require('../assets/sel4.jpg')" alt="Image 1"></b-img>
    </b-col>
    <b-col class="col-lg-4 col-md-6 col-sm-12">
        <router-link to="/About">
      <b-img rounded="circle" class = "image" thumbnail fluid :src="require('../assets/sel5.jpg')" alt="Image 2"></b-img>
        </router-link>
    </b-col>
    <b-col class="col-lg-4 col-md-6 col-sm-12">
      <b-img rounded="circle" class = "image" thumbnail fluid :src="require('../assets/sel6.jpg')" alt="Image 3"></b-img>
    </b-col>
  </b-row>
</b-container>
</div>
</template>
<script>
export default {
  name: 'Selector'
}
</script>

<style scoped>
.image:hover {
    -webkit-transform: scale(1.2);
    transform: scale(1.2);
}
.image {
  max-width: 80%;
}
div {
    padding-top: 1%;
    padding-left: 4%;
    padding-right: 3%;
}

@media (min-width: 500px){
  .col-lg-4 {
      flex: 0 0 33.3333%;
      max-width: 33.3333%;
      padding-top: 4%;
}}

@media (max-width: 500px){
  .col-md-6 {
      flex: 0 0 50%;
      max-width: 50%;
      padding-top: 6%;
}}

@media (max-width: 300px){
  .col-sm-12 {
      flex: 0 0 100%;
      max-width: 100%;
      padding-top: 11%;
  }
}
</style>
