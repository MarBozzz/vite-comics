<script>
export default {
  name : 'AppHeader'
}
</script>

<template>

  <header>
    <div class="container">
      <a href="#" class="logo">
        <img src="/public/dc-logo.png" alt="Logo DC">
      </a>
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
    nav {
      height: 100%;
      ul {
        display: flex;
        list-style: none;
        height: 100%;
        li {
          height: 100%;
          display: flex;
          align-items: center;
          a {
            height: 100%;
            line-height: 120px;
            color: #484848;
            margin-left: 40px;
            text-decoration: none;
            text-transform: uppercase;
            font-size: .75rem;
            font-weight: bold;
            border-bottom: 5px solid white;
            &:hover, &.active {
              color: #0282F9;
              border-bottom: 5px solid #0282F9;
            }
          }
        }
      }
    }
  }
}

</style>