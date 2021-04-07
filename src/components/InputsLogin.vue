<template>
  <div>
    <div class="row justify-content-center">
      <div class="col">
        <div class="input-group mb-3 justify-content-center flex-nowrap">
          <input
            :type="type"
            class="form-control no-bordes"
            :placeholder="placeholder"
            :aria-label="placeholder"
            aria-describedby="addon-wrapping"
            :id="id"
            v-model="datoInput"
          />
          <span class="input-group-text no-bordes" id="addon-wrapping"
            ><img :src="icon"
          /></span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "InputsLogin",
  props: ["placeholder", "icon", "type",'id'],
  data() {
    return {
      datoInput: ''
    }
  },
  computed: {

    },
  updated() {
      this.$emit('datoInput',this.datoInput)
    }
  };
</script>
<style scoped>
.no-bordes {
  border: white;
  background-color: white;
}
.row {
  margin-top: 15px;
}
</style>
