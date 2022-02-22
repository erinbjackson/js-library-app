<script>
// import chartXkcd from "chart.xkcd";
/*global simpleParallax*/

  export default {
    data: function () {
      return {};
    },
    mounted: function () {
        var image = document.getElementsByClassName('thumbnail');
        new simpleParallax(image, {delay: 1, 
        transition: 'cubic-bezier(0,0,0,1)'});
        console.log(simpleParallax);

      var image2 = document.getElementsByClassName('sideways');
        new simpleParallax(image2, {delay: 1, 
        orientation: 'right'});
        console.log(simpleParallax);

          },
          
          
    methods: {},
  };
</script>

<template>
<div>This is a paralax image. </div>
  <img class="thumbnail" src="../assets/forest.jpg" alt="image">
  <p>and another option</p>
  <img class="sideways" src="../assets/forest.jpg" alt="image">

 

</template>

<style>
.thumbnail {
  height: 500px;
}
.sideways {
  max-width: 700px;
}
</style>