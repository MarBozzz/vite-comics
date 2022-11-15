<script>
export default {
  name : 'AppHeader'
}
</script>

<template>

  <header>
    <div class="container">
      <div class="logo">
        <img src="/public/dc-logo.png" alt="Logo DC">
      </div>
      <nav>
        <ul>
          <li>
            <a href="#">Characters</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
  
</template>

<style lang="scss" scoped>
header {
  height: 120px;
  background-color: white;
  .container {
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
}

</style>