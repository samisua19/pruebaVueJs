<template>
  <div>
    <div class="row justify-content-center">
      <div class="d-grid gap-2">
        <button class="btn btn-primary" id="btnIngresar" :type="type" >{{ title }}</button>
      </div>
    </div>
  </div>
</template>

<script>
import { mapState, mapMutations } from 'vuex';
export default {
  name: "Button",
  props: ["title","type"],
};
</script>

<style scoped>
#btnIngresar {
  background-color: #04c5e2;
  border-color: #04c5e2;
  width: 270px;
}
</style>
