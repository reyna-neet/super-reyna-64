<template>
  <div class="container">
    <h1 v-if="error.statusCode === 404">Page not found</h1>
    <h1 v-else-if="error.statusCode === 418">I'm a teapot!</h1>
    <h1 v-else>An error occurred</h1>
  </div>
</template>

<script>
export default {
  props: ['error']
}
</script>
