<template>
  <div>
    <Body :text="text" />

    <input type="text" v-model="text">
  </div>
</template>

<script>
  import { ref } from 'vue'
  import Body from './components/Body.vue'
  export default {
    components: {
      Body
    },

    setup () {
      const text = ref('')

      return {
        text
      }
    }
  }
</script>