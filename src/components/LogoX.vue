<template>
  <div>
    <div class="container" id="containerLogoX">
      <div class="row">
        <div class="col">
          <img src="../assets/logo-x.png" id="imageLogo" />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "LogoX",
};
</script>

<style scoped>
#containerLogoX {
  background: linear-gradient(0deg, rgba(3,172,196,1) 32%, rgba(0,204,232,1) 100%, rgba(255,255,255,1) 100%);
  border-radius: 100px;
  height: 130px;
  width: 130px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 15px;
}
#imageLogo {
  height: 70px;
  width: 70px;
  margin-top: 0px;
}
</style>
