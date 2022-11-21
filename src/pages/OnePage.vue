<template>
  <q-page paddi ng class="bggrey" >
     <div   class="q-pa-md row no-wrap items-start q-gutter-md">
      <CartaoKpi title="Vendas" icon="show_chart"/>
      <CartaoKpi title="Estoque" icon="bar_chart" class="shadow-9"></CartaoKpi>
      <CartaoKpi title="Devoluções" icon="trending_down"/>
    </div>
  </q-page>
</template>

<script>
import CartaoKpi from 'components/CartaoKpi.vue'

export default {
  name: 'MainLayout',
  components: {
    CartaoKpi
  },
}
</script>

<style scoped>

.bggrey {
  background-color: rgb(246, 246, 249);
}
</style>
