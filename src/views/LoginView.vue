<template>
  <div class="login">
    <div class="login__content">
      <div class="login__content__form">
        <h1 class="login__content__header--title">Welcome Back</h1>
        <p class="login__content__header--desc">Vous pouvez vous connecter</p>
        <LoginForm />
      </div>
    </div>
    <div class="login__illustration"></div>
  </div>
</template>

<script setup lang="ts">
import LoginForm from "@/components/forms/LoginForm.vue";
</script>

<style scoped>
.login {
  display: grid;
  grid-template-columns: 1fr 1fr;
  height: 100vh;
}

.login__illustration {
  background-image: url('../assets/img/login_illustration.jpg');
}

.login__content {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.login__content__form {
  width: 100%;
  max-width: 600px;
  padding: 0 2rem;
}

.login__content__header--title {
  font-size: 3rem;
  font-weight: 700;
  color: #000;
}

@media only screen and (max-width: 790px)  {
  .login {
    grid-template-columns: 1fr;
  }

  .login__illustration {
    display: none;
  }
}

@media only screen and (max-width: 790px)  {
  .login__content__header--title {
    font-size: 2rem;
  }
}

</style>