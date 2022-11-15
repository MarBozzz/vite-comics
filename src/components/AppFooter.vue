<script>
export default {
  name : 'AppFooter'
}
</script>

<template>
  
  <footer>

    <div class="upper-footer">
      <div class="container">
        <div class="menues">
          <div class="col">
            <nav>
              <ul>
                <li>
                  <span>DC Comics</span>
                </li>
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
                  <a href="#">Videos</a>
                </li>
                <li>
                  <a href="#">News</a>
                </li>
              </ul>
            </nav>
            <nav>
              <ul>
                <li>
                  <span>Shop</span>
                </li>
                <li>
                  <a href="#">Shop DC</a>
                </li>
                <li>
                  <a href="#">Shop DC Collectibles</a>
                </li>
              </ul>
            </nav>
          </div>
  
          <div class="col">
            <nav>
              <ul>
                <li>
                  <span>DC</span>
                </li>
                <li>
                  <a href="#">Terms Of Use</a>
                </li>
                <li>
                  <a href="#">Privacy Policy (New)</a>
                </li>
                <li>
                  <a href="#">Ad Choices</a>
                </li>
                <li>
                  <a href="#">Advertising</a>
                </li>
                <li>
                  <a href="#">Jobs</a>
                </li>
                <li>
                  <a href="#">Subscriptions</a>
                </li>
                <li>
                  <a href="#">Talent Workshops</a>
                </li>
                <li>
                  <a href="#">CPSC Certificates</a>
                </li>
                <li>
                  <a href="#">Ratings</a>
                </li>
                <li>
                  <a href="#">Shop Help</a>
                </li>
                <li>
                  <a href="#">Contact Us</a>
                </li>
              </ul>
            </nav>
          </div>
  
          <div class="col">
            <nav>
              <ul>
                <li>
                  <span>Sites</span>
                </li>
                <li>
                  <a href="#">DC</a>
                </li>
                <li>
                  <a href="#">MAD Magazine</a>
                </li>
                <li>
                  <a href="#">DC Kids</a>
                </li>
                <li>
                  <a href="#">DC Universe</a>
                </li>
                <li>
                  <a href="#">DC Power Visa</a>
                </li>
              </ul>
            </nav>
          </div>
        </div>

        <div class="logo">
          <img src="/public/dc-logo-bg.png" alt="Logo DC">
        </div>
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
    .container {
      display: flex;
      justify-content: space-between;
      
      height: 100%;
      .menues {
        display: flex;
        justify-content: flex-start;
        .col {
          margin-right: 1rem;
          nav ul {
            list-style: none;
            li:first-child {
              font-size: 1.2rem;
              font-weight: 800;
              padding: 40px 0 15px;
              text-transform: uppercase;
            }
            li {
              font-size: .8rem;
              padding: .15rem;
            }
            a {
              text-decoration: none;
              color: #959595;
            }
          } 
        }
      }
      .logo {
        display: flex;
        align-items: center;
        height: 100%;
        overflow-y: hidden;
      }
    }
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