<template>
    <div>
        <p>Product details {{ id }}</p>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Officiis doloribus eveniet unde ullam iusto nihil
            distinctio suscipit commodi similique vitae!</p>
    </div>
</template>

<script setup>
const { id } = useRoute().params
definePageMeta({
    layout: "products"
})
</script>

<style scoped></style>