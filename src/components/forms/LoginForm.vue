<template>
  <form action="" class="mt-5">
    <div class="form-control mt-5 w-full">
      <label for="email" class="label"><span class="label-text ">Email</span></label>
      <input type="text" placeholder="Entrez votre adresse mail" id="email" class="input input-bordered w-full">
    </div>
    <div class="form-control mt-5 w-full">
      <label for="password" class="label"><span class="label-text">Password</span></label>
      <input type="password" placeholder="********" id="password" class="input input-bordered w-full">
    </div>
    <div class="mt-5 w-full text-right">
      <a href="#" class="text-primary font-bold">Mot de passe oublié</a>
    </div>
    <div class="form-control mt-5 w-full">
      <button type="submit" class="btn btn-primary w-full">Se connecter</button>
    </div>
    <div class="mt-14 w-full text-center">
      <p class="text-gray-500">Pas de compte ? <a href="#" class="text-primary font-bold">Inscrivez-vous</a></p>
    </div>
  </form>
</template>

<script setup lang="ts">
</script>

<style scoped>

</style>