<template>
  <div class="home">
    <Navbar id="navbar"></Navbar>
    <div id="containerItems" >
      <form action="" @submit="loginForm">
        <LogoX></LogoX>
        <InputsLogin
          :placeholder="'Correo electrónico'"
          :icon="'https://img.icons8.com/ios/24/000000/new-post.png'"
          :type="'email'"
          :id="'inputEmail'"
          @datoInput="email = $event"
        />
        <InputsLogin
          :placeholder="'Contraseña'"
          :icon="'https://img.icons8.com/metro/26/000000/key.png'"
          :type="'password'"
          :id="'inputPass'"
          @datoInput="pass = $event"
        />
        <Button :title="'Ingresar'" :type="'submit'" />
      </form>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";
import LogoX from "@/components/LogoX.vue";
import InputsLogin from "@/components/InputsLogin.vue";
import TitleLogin from "@/components/TitleLogin.vue";
import Button from "@/components/Button";

export default {
  name: "App",
  components: {
    Navbar,
    LogoX,
    InputsLogin,
    TitleLogin,
    Button,
  },
  data() {
    return {
      email: '',
      pass: ''
    }
  },
  methods: {
    loginForm: function (e) {
      e.preventDefault();
      console.log(this.email)
      }
    }
};
</script>

<style>
#containerItems {
  display: flex;
  flex: 1;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  transform: translateY(50%);
  width: 100%;
}
</style>
