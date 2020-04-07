<template>
  <div>
    <Lifecycle v-if="show" />

    <a href="#" @click.prevent="destroy">Click</a>
  </div>
</template>

<script>
  import { ref } from 'vue'
  import Lifecycle from './components/Lifecycle.vue'

  export default {
    components: {
      Lifecycle
    },

    setup () {
      const show = ref(true)

      function destroy() {
        show.value = false
      }

      return {
        show,
        destroy
      }
    }
  }
</script>