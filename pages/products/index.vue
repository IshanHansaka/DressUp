<template>
    <div>
        <div class="grid grid-cols-4 gap-5">
            <div v-for="product in products">
                <ProductCard :product = "product"/>
            </div>
        </div>
    </div>
</template>

<script setup>
definePageMeta({
    layout: "products"
})

//fetch products
const { data: products } = await useFetch("https://fakestoreapi.com/products")

useHead({
    title: "DressUp | Products",
    meta: [
        { name: "description", content: "Nuxt 3 products" }
    ]
})
</script>

<style scoped></style>