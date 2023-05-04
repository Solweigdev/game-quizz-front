<template>
  <form action="" class="mt-5">
    <div class="form-control mt-5 w-full">
      <label for="pseudo" class="label"><span class="label-text ">Pseudo</span></label>
      <input type="text" placeholder="CyberSpectre" id="pseudo" class="input input-bordered w-full">
    </div>
    <div class="form-control mt-5 w-full">
      <label for="email" class="label"><span class="label-text ">Email</span></label>
      <input type="text" placeholder="Entrez votre adresse mail" id="email" class="input input-bordered w-full">
    </div>
    <div class="form-control mt-5 w-full">
      <label for="password" class="label"><span class="label-text">Password</span></label>
      <input type="password" placeholder="********" id="password" class="input input-bordered w-full">
    </div>
    <div class="form-control mt-5 w-full">
      <label for="password_confirmed" class="label"><span class="label-text">Confirmation Password</span></label>
      <input type="password" placeholder="********" id="password_confirmed" class="input input-bordered w-full">
    </div>
    <div class="mt-5 w-full text-right">
      <div class="form-control">
        <label class="cursor-pointer label">
          <span class="label-text">Afficher le mot de passe</span>
          <input type="checkbox" checked="checked" class="checkbox checkbox-warning" />
        </label>
      </div>
    </div>
    <div class="form-control mt-5 w-full">
      <button type="submit" class="btn btn-primary w-full">S'inscrire</button>
    </div>
    <div class="mt-14 w-full text-center">
      <p class="text-gray-500">Déjà un compte ? <a href="#" class="text-primary font-bold">Connectez-vous</a></p>
    </div>
  </form>
</template>

<script>
export default {
  name: "RegisterForm"
}
</script>

<style scoped>

</style>