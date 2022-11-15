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
          <li>
            <a href="#">Comics</a>
          </li>
          <li>
            <a href="#">Movies</a>
          </li>
          <li>
            <a href="#">Tv</a>
          </li>
          <li>
            <a href="#">Games</a>
          </li>
          <li>
            <a href="#">Collectibles</a>
          </li>
          <li>
            <a href="#">Fans</a>
          </li>
          <li>
            <a href="#">News</a>
          </li>
          <li>
            <a href="#">Shop</a>
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

    .logo {
      width: 80px;
    }
    nav ul {
      display: flex;
      list-style: none;
      a {
        color: #484848;
        margin-left: 40px;
        text-decoration: none;
        text-transform: uppercase;
        font-size: .75rem;
        font-weight: bold;
        &:hover {
          color: #0282F9;
        }
      }
    }
  }
}

</style>