<template>
  <div>
    <BodyComputed :text="text" />

    <input type="text" v-model="text">
  </div>
</template>

<script>
  import { ref } from 'vue'
  import BodyComputed from './components/BodyComputed.vue'

  export default {
    components: {
      BodyComputed
    },

    setup () {
      const text = ref('')

      return {
        text
      }
    }
  }
</script>