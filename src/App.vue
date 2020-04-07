<template>
  <div>
    <Suspense>
      <template #default>
        <TodoIndex />
      </template>
      <template #fallback>
        <div>Loading...</div>
      </template>
    </Suspense>
  </div>
</template>

<script>
  import TodoIndex from "./components/TodoIndex.vue";
  export default {
    components: {
      TodoIndex
    }
  }
</script>