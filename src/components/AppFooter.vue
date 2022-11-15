<script>
export default {
  name : 'AppFooter'
}
</script>

<template>
  
  <footer>

    <div class="upper-footer">
      <div class="container">

      </div>
    </div>

    <div class="lower-footer">
      <div class="container">
      <div class="cta">
        <a href="#">Sign-Up Now!</a>
      </div>
      <nav>
        <ul>
          <li>
            <span>Follow Us</span>
          </li>
          <li>
            <a href="#">
              <img src="../assets/img/footer-facebook.png" alt="Facebook">
            </a>
          </li>
          <li>
            <a href="#">
              <img src="../assets/img/footer-twitter.png" alt="Twitter">
            </a>
          </li>
          <li>
            <a href="#">
              <img src="../assets/img/footer-youtube.png" alt="Youtube">
            </a>
          </li>
          <li>
            <a href="#">
              <img src="../assets/img/footer-pinterest.png" alt="Pinterest">
            </a>
          </li>
          <li>
            <a href="#">
              <img src="../assets/img/footer-periscope.png" alt="Periscope">
            </a>
          </li>
        </ul>
      </nav>
      </div>
    </div>
    
  </footer>

</template>

<style lang="scss" scoped>
footer {
  .upper-footer {
    height: 370px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
  }
  .lower-footer {
    height: 120px;
    background-color: #303030;
    text-transform: uppercase;
    .container {
      height: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;

      .cta {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 150px;
        height: 50px;
        font-size: 1.1rem;
        font-weight: 800;
        border: 2px solid #0282F9;
        a {
          text-decoration: none;
          color: white;
        }
      }
      nav ul {
        display: flex;
        align-items: center;
        list-style: none;
        li:first-child {
          color: #0282F9;
          font-size: 1.2rem;
          font-weight: 800;
          margin-right: 10px;
        }
        a {
          margin-left: 20px;
          text-decoration: none;
        }
      }
    }
  }
}
</style>