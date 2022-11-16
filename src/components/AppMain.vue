<script>

import AppCard from './AppCard.vue';

export default {
  name : 'AppMain',
  components : {
    AppCard,
  },
  data(){
    return {
      products : [
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          "price": "$19.99",
          "series": "Action Comics",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          "price": "$3.99",
          "series": "American Vampire 1976",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          "price": "$16.99",
          "series": "Aquaman",
          "type": "graphic novel"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          "price": "$2.99",
          "series": "Batgirl",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$3.99",
          "series": "Batman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$2.99",
          "series": "Batman Beyond",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          "price": "$3.99",
          "series": "Batman/Superman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          "price": "$4.99",
          "series": "Batman/Superman Annual",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          "price": "$5.99",
          "series": "Batman: The Joker War Zone",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          "price": "$6.99",
          "series": "Batman: Three Jokers",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          "price": "$4.99",
          "series": "Batman: White Knight Presents: Harley Quinn",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          "price": "$16.99",
          "series": "Catwoman",
          "type": "graphic novel"
        }
      ],
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

    <div class="cards">

      <div class="container">
        <AppCard v-for="(card, index) in products" :key="index" 
        :cardImage="card.thumb"
        :cardTitle="card.series"
        />
      </div>

      <div class="load-more">
        <a class="btn" href="#">Load More</a>
      </div>

    </div>

    <section>
  
      <div class="lower container">
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
    </section>

  </main>
</template>

<style lang="scss" scoped>
.cards {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  height: 666px;
  background-color: #1C1C1C;
  .container {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
  }
}
.load-more {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 185px;
  height: 35px; 
  background-color: #0282F9;
  margin-bottom: 20px;
  &:hover {
      border: 2px solid #0282F9;
      background-color: white;
      color: #0282F9;
      a {
        color: #0282F9;
      }
  }
  a {
    text-decoration: none;
    text-transform: uppercase;
    color: white;
    font-size: .8rem;
    font-weight: bold;
  }
}
section {
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