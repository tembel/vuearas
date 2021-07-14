<template>
  <h1>Product Details Page</h1>
  <p>The product id is {{ $route.params.id }}</p>
</template>

<script>
export default {
  data() {
    return {
        id: this.$route.params.id
    }
  }
}
</script>


<style>

</style>