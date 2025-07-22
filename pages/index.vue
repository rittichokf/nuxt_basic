<template>
    <div>
        <header>
            <nav>
                <ul>
                    <li><nuxt-link to="/about">About</nuxt-link></li>
                    <li><nuxt-link to="/products">Products</nuxt-link></li>
                </ul>
            </nav>
        </header>
        <div>
            <h2>Home</h2>
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>
nav {
    background-color: #b6cbe0;
    padding: 10px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
nav ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
}
nav li {
    margin-right: 15px;
}
nav a {
    text-decoration: none;
    color: #007bff;
}
nav a:hover {
    text-decoration: underline;
    color: #000;
}
h2 {
    color: #343a40;
    font-size: 24px;
    margin-top: 20px;
}
</style>