<template>
  <div class="basic-slide">
    <img src="https://cdn1.thr.com/sites/default/files/imagecache/list_landscape_960x541/2016/02/karate_kid_1984_16.jpg">
    <button>Display</button>
    <div class="details">
      <a href="/">sensei</a> to <a href="/">kid</a> - The Karate Kid, 1984
    </div>
    <div class="quote">
      <p>"Wax on, wax off."</p>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Basic',
  };
</script>

<style>
  .basic-slide {
    padding: 20px;
  }

  img {
    width: 50%;
    vertical-align: bottom;
  }

  button {
    float: right;
  }

  .details {
    display: inline-block;
    padding: 20px;
    width: 250px;
    background-color: aliceblue;
    margin-left: 19.9%;
  }

  .quote {
    padding: 20px;
    background-color: aliceblue;
    min-height: 20%;
    margin-top: 20px;
  }

</style>
