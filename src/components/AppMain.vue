<script>
export default {
  name : 'AppMain',
  data(){
    return {
      buyMenu : [
        {
          image : 'buy-comics-digital-comics.png',
          href : '#',
          text : 'Digital Comics'
        },
        {
          image : 'buy-comics-merchandise.png',
          href : '#',
          text : 'DC Merchandise'
        },
        {
          image : 'buy-comics-subscriptions.png',
          href : '#',
          text : 'Subscription'
        },
        {
          image : 'buy-comics-shop-locator.png',
          href : '#',
          text : 'Comics Shop Locator'
        },
        {
          image : 'buy-dc-power-visa.svg',
          href : '#',
          text : 'DC Power Visa'
        },
      ]
    }
  },
  methods : {
    getImagePath: function(imgPath){
      return new URL (imgPath, import.meta.url).href;
    }
  }
}
</script>

<template>
  <main>
    <div class="container">
      <nav>
        <ul>
          <li
            v-for="(item, index) in buyMenu"
            :key="index">
            <a :href="item.href">
              <div class="image">
                <img :src="getImagePath(`../assets/img/${item.image}`)">
              </div>
              <span>{{item.text}}</span>
            </a>
          </li>
        </ul>
      </nav>
    </div>
  </main>
</template>

<style lang="scss" scoped>
main {
  height: 155px;
  background-color: #0282F9;
  .container {
    height: 100%;
    nav {
      height: 100%;
      ul {
        height: 100%;
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        list-style: none;
        a {
          display: flex;
          justify-content: space-between;
          align-items: center;
          text-decoration: none;
          &:hover {
            transform: scale(1.05);
          }
          .image {
            img {
              height: 50px;
            }
          }
          span {
            color: white;
            text-transform: uppercase;
            font-size: .9rem;
            padding-left: 1rem;
          }
        }
      }
    }
  }
}
</style>