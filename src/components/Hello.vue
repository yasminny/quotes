<template>
  <div class="page">
    <Layout/>
  </div>
</template>

<script>
  import Layout from './Layout/Layout';

  export default {
    name: 'hello',
    components: { Layout },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #35495E;
}

.page {
  width: 100%;
  height: 100%;
}
</style>
