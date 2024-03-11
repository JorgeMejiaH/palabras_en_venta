<template>
  <div>
    <img src="@/assets/Logo.png" alt="Logo de la pagina" class="img-logo" />
    <img
      src="@/assets/PageTitle.png"
      alt="Titulo de la pagina"
      class="img-title"
    />

    <img
      src="@/assets/LoginBackground.png"
      alt="Fondo de la pagina"
      class="login-background"
    />
    <img
      src="@/assets/WhiteBackground.png"
      alt="fondo blanco"
      class="white-background"
    />
    <p class="txt-not-account">¿Aún no tienes cuenta? Regístrate</p>
    <h1 class="txt-welcome">¡Bienvenido!</h1>
    <h2 class="txt-login">Ingresa a tu cuenta</h2>
    <form @submit.prevent="handleSubmit" class="block-inputs" name="login-form">
      <UsernameInput />
      <PasswordInput />
      <button type="submit" class="btn-login">Iniciar Sesión</button>
    </form>
  </div>
</template>

<script>
import PasswordInput from "./PasswordInput.vue";
import UsernameInput from "./UsernameInput.vue";
export default {
  components: { UsernameInput, PasswordInput },
};
</script>

<style>
.img-logo {
  position: absolute;
  top: 0.5%;
  left: 1%;
  width: 6%;
  height: auto;
}
.img-title {
  position: absolute;
  top: 3.5%;
  left: 7.5%;
  width: 8%;
  height: auto;
}
.txt-not-account {
  text-align: end;
  margin-right: 5%;
  margin-top: -1%;
}

.login-background {
  position: absolute;
  top: 0;
  left: 0;
  width: 55%;
  height: 100%;
  z-index: -2;
  background: #050835;
}

.white-background {
  position: absolute;
  top: 0;
  left: 50%;
  width: 55%;
  height: 100%;
  z-index: -1;
  border-top-left-radius: 40px;
  border-bottom-left-radius: 40px;
}
.txt-welcome {
  text-align: end;
  margin-right: 32%;
  margin-top: 15%;
  font-size: 220%;
  color: #3b63a8;
  font-weight: bold;
  z-index: 1;
}

.txt-login {
  text-align: end;
  margin-top: 0;
  margin-right: 28%;
  font-size: 201%;
  font-weight: bold;
}
.in-user-login {
  width: 30%;
  padding: 8px;
  box-sizing: border-box;
  border-radius: 8px;
}

label {
  display: block;
  margin-bottom: 0;
  font-size: 100%;
}

.block-inputs {
  margin-left: 30%;
}

.btn-login {
  margin-top: 5%;
  width: 30%;
  height: 15%;
  padding: 8px;
  box-sizing: border-box;
  border-radius: 8px;
  background-color: #050835;
  color: white;
  cursor: pointer;
}
</style>
