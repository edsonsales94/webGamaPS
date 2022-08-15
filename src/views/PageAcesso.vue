<template>
    <div class="body">
        <FormLogin />
    </div>

</template>

<script>
// @ is an alias to /src
import FormLogin from "../components/FormLogin.vue"

export default {
  name: 'PageAcesso',
  components: {
      FormLogin,
  }
}
</script>

<style >
.body {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background: linear-gradient(rgb(255, 255, 255) 10%,rgb(185, 192, 224) );
  margin: 0; 
}

</style>