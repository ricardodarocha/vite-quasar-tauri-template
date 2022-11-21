<template>
  <q-card flat shaddow-12 class="my-card">
        <q-card-section >
          <div class="row items-center ">
            <div class="text-subtitle2">{{title}}</div>
            <q-btn
              dense
              unelevated round
              color="deep-purple-1"
              text-color="deep-purple-10"
              :icon="icon"
              class="absolute"
              style="right: 18px; top: 12px;"
            />
          </div>
          <div class="text-h6">18,417</div>

          <div class="row items-center ">
            <div class="text-subtitle1 text-primary">
              7,34%
            </div>
            <div class="text-caption text-grey">
               🔺 último mês
            </div></div>
        </q-card-section>

      </q-card>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'CartaoKpi',
  props: {
    title: {
      type: String,
      required: true
    },

    caption: {
      type: String,
      default: ''
    },

    link: {
      type: String,
      default: '#'
    },

    icon: {
      type: String,
      default: ''
    }
  }
})
</script>

<style scoped>

.my-card{
  width: 260px
}

</style>
