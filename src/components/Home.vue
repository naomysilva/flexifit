<template id="Home">
  <div class="Home text-center">
    <h1>FLEXIFIT</h1>
    <span>ACADEMIA DIGITAL</span>
    <form action="">
      <v-divider class="first-divider"></v-divider>
      <v-text-field type="text" label="Usuário ou e-mail"></v-text-field>
      <v-divider></v-divider>
      <v-text-field type="text" label="Senha" solo hide-details></v-text-field>
      <v-divider></v-divider>
      <v-btn variant="tonal" size="x-large" class="mb-5">
        <svg-icon type="mdi" :path="path"></svg-icon> Entrar
      </v-btn>
      <span class="text"> Não tem cadastro? </span>
      <span class="text"> Esqueceu sua senha?? </span>
    </form>
  </div>
</template>

<script>
import SvgIcon from "@jamescoyle/vue-icon";
import { mdiLoginVariant } from "@mdi/js";
export default {
  name: "Home",
  components: {
    SvgIcon,
  },
  data() {
    return {
      path: mdiLoginVariant,
    };
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");
.Home {
  text-align: center;
  font-family: "Poppins", sans-serif;
  font-weight: 800;
  font-style: normal;
}

.v-divider {
  width: 100%;
  color: #d8580c;
  opacity: 1 !important;
  margin-bottom: 1rem;
  margin-top: 1rem;
}

.first-divider {
  margin-top: 5em;
}

h1 {
  font-size: 75px;
}

span {
  font-size: 26px;
}

.text {
    font-size: 11px;
    text-decoration: underline;
    text-align: end;
}

form {
  display: flex;
  flex-direction: column;
}

.v-btn {
  background-color: #d8580c !important;
  border-radius: 57px !important;
}
</style>
