<template>
  <div class="d-flex justify-content-center">
      <h1 class="align-self-center">No hay nada seleccionado</h1>
  </div>

    <FlorinActionButton />

</template>

<script>
import { defineAsyncComponent } from 'vue'

export default {
    components: {
        FlorinActionButton: defineAsyncComponent(() => import('../components/FlorinActionButton'))
    }
}
</script>

<style lang="scss" scoped>
div {
    height: 100%;
}
</style>