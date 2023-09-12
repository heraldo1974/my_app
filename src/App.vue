<template>
  <form>
    <h1><b>Nome</b></h1>
    <input placeholder="Digite seu nome" v-model="name" />
    <button type="button" @click="mudarEnviado">Enviar Mensagem</button>
    <hr />
    <h1 v-if="enviado">Olá {{ name }}</h1>
  </form>
</template> asdasd

<script>
export default {
  data() {
    return {
      name: null,
      enviado: false,
    };
  },
  methods: {
    mudarEnviado() {
      this.enviado = !this.enviado;
    },
  },
};
</script>

<style>
</style>