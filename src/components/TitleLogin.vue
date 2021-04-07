<template>
<div>
  <div class="row justify-content-center">
    <div class="col ">
      <h3 id="title">{{title}}</h3>
    </div>
  </div>
  </div>
</template>

<script>
export default {
  name: "TitleLogin",
  props: ['title']
};
</script>

<style scoped>
#title {
  font-style: bold;
  font-weight: bolder;
  color: #2d4d64;
  }
</style>
