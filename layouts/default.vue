<template>
  <div>
    <header>
      <nav>
        <div class="logo">Nuxt Basic</div>
        <ul>
          <li><nuxt-link to="/">Home</nuxt-link></li>
          <li><nuxt-link to="/about">About</nuxt-link></li>
          <li><nuxt-link to="/products">Products</nuxt-link></li>
        </ul>
      </nav>
    </header>

    <!-- Slot content from pages จะมาแสดงตรงนี้ -->
    <main class="main-content">
      <slot />
    </main>
  </div>
</template>

<script setup>
</script>

<style scoped>

nav {
  background-color: #29824e;
  color: white;
  padding: 15px 30px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;      
  max-width: 100vw;
  box-sizing: border-box; 
  overflow-x: hidden; 
  z-index: 1000;
}

.logo {
  font-size: 20px;
  font-weight: bold;
  color: #ffffff;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 20px;
  margin: 0;
  padding: 0;
}

nav li {
  margin: 0;
}

nav a {
  text-decoration: none;
  color: #ffffff;
  font-weight: 500;
  transition: color 0.3s ease;
}

nav a:hover {
  color: #ffd700;
}

.main-content {
  padding-top: 80px;
  padding-left: 30px;
  padding-right: 30px;
  padding-bottom: 40px;
  background-color: #ffffff;
  min-height: 100vh;
}

h2 {
  color: #1e293b;
  font-size: 28px;
  margin-bottom: 10px;
}

p {
  color: #4b5563;
  font-size: 16px;
}
</style>
