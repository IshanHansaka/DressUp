<template>
    <div>
        <header>
            <nav>
                <NuxtLink to="/products">DressUp</NuxtLink>
            </nav>
        </header>
        <div>
            <slot />
        </div>
        <footer>
            <ul>
                <li>
                    <NuxtLink to="/">Home</NuxtLink>
                </li>
                <li>
                    <NuxtLink to="/about">About</NuxtLink>
                </li>
                <li>
                    <NuxtLink to="/products">Products</NuxtLink>
                </li>
            </ul>
        </footer>
    </div>
</template>

<script setup>
</script>

<style scoped>
.router-link-exact-active {
    color: #12b488;
}
</style>