<template>
    <h1>Products</h1>
    <div v-for="product in products" :key="product.id">
        <router-link :to="{ name: 'ProductDetails', params: { id: product.id }}">
            <h2> {{ product.title }} </h2>
        </router-link>
    </div>
</template>

<script>
export default {
  data() {
    return {
      products: [
        { id: "1", colorname: "Burgundy", colorpicfile: null, colorord: "1" },
        { id: "2", colorname: "Navy Blue", colorpicfile: null, colorord: "2" },
        { id: "3", colorname: "White", colorpicfile: null, colorord: "3" },
        { id: "4", colorname: "Black", colorpicfile: null, colorord: "4" },
        {
          id: "6", colorname: "Pink", colorpicfile: "pink158.jpg",colorord: "5",
        }
      ]
    }
  }
}
</script>

<style>

</style>