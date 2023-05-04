<template>
  <div class="register">
    <div class="register__content">
      <div class="register__content__form">
        <h1 class="register__content__header--title">S'enregistrer</h1>
        <p class="register__content__header--desc">Vous pouvez vous inscrire</p>
        <RegisterForm />
      </div>
    </div>
    <div class="register__illustration"></div>
  </div>
</template>

<script setup lang="ts">
import RegisterForm from "@/components/forms/RegisterForm.vue";

</script>

<style scoped>
  .register {
    display: grid;
    grid-template-columns: 1fr 1fr;
    height: 100vh;
  }

  .register__illustration {
    background-image: url('../assets/img/register_illustration.jpg');
  }

  .register__content {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .register__content__form {
    width: 100%;
    max-width: 600px;
    padding: 0 2rem;
  }

  .register__content__header--title {
    font-size: 3rem;
    font-weight: 700;
    color: #000;
  }

  @media only screen and (max-width: 790px)  {
    .register {
      grid-template-columns: 1fr;
    }

    .register__illustration {
      display: none;
    }
  }

  @media only screen and (max-width: 790px)  {
    .register__content__header--title {
      font-size: 2rem;
    }
  }
</style>