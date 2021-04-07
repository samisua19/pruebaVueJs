<template>
  <div>
    <header class="header">
      <nav class="navbar navbar-expand-lg navbar-light sticky-top" >
        <div class="container-fluid">
          <img src="../assets/logo.png" id="imageLogo" />
        </div>
        <div class="container-fluid" id="help">
          ?
        </div>
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>
<style scoped>
#imageLogo {
  height: 20px;
  
}
.navbar{
    
    background-color: white;
    
    }
#help {
    height: 27px;
    width: 27px;
    border-radius: 100px;
    margin-right: 5px;
    background-color: #00cce8;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: row;
    color: white;
    }
</style>
