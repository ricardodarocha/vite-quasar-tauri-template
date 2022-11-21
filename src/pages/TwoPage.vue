<template>
  <q-page padding>
    <div class="q-gutter-md">

      <pre>{{ conputedvalue }}</pre>
      <q-item>
        <q-label color="indigo" >Categoria</q-label>
      </q-item>
      <q-input dense outlined v-model="valor" label="valor" class="input"/>
    <q-input dense outlined v-model="nome" label="nome" class="input"/>
    <q-input dense outlined v-model="sobrenome" label="sobrenome" class="input"/>
    <q-input dense outlined v-model="cpf" label="cpf" class="input"/>
  </div>
  </q-page>
</template>

<script>
// import { computed } from '@vue/reactivity'
import { ref } from 'vue'

export default {
  data () {
    return {
      valor: 'bem vindo',
      nome: 'bem vindo',
      sobrenome: 'bem vindo',
      cpf: 'bem vindo'
    }
  },
  computed: {
    // a computed getter
    conputedvalue () {
      // `this` points to the component instance
      return this.valor + " " + this.nome + " " + this.sobrenome
    }
  },
  setup () {
    const mensagem = ref('Olá')

    return {
      mensagem
    }
  }
}
</script>

<style scoped>
.input {
  max-width: 400px;
}

</style>
