<script setup lang="ts">
</script>

<template>
  <div class="default-container">
    <header class="header">
      <div class="logo">LOGO</div>

      <ul class="menu">
        <li class="item"><nuxt-link class="link" to="/">トップ</nuxt-link></li>
        <li class="item"><nuxt-link class="link" to="/home">Home</nuxt-link></li>
        <li class="item"><nuxt-link class="link" to="/about">About</nuxt-link></li>
        <li class="item"><nuxt-link class="link" to="/videos">Videos</nuxt-link></li>
      </ul>
    </header>
    <main class="main">
      <slot />
    </main>
  </div>
</template>

<style lang="scss" scoped>
.default-container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;

  .header {
    background-color: #333;
    color: #fff;
    padding: 20px;
    display: flex;
    align-items: center;
    justify-content: space-between;

    .menu {
      display: flex;
      list-style: none;
      padding: 0;

      .item {
        margin-right: 20px;
        .link {
          color: #fff;
          text-decoration: none;
          &:hover {
            text-decoration: underline;
          }
        }

      }
    }
  }
}


</style>