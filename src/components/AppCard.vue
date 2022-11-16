<script>
export default {
  name : 'AppCard',
  props : {
    cardImage: String,
    cardTitle: String
  }
}
</script>

<template>
  <div class="card">
    <div class="img-container">

      <img :src="cardImage" :alt="cardTitle">
    </div>
    <span>{{cardTitle}}</span>
  </div>
</template>

<style lang="scss" scoped>
  .card {
    width: calc(100% / 6 - 20px);
    margin: 10px;
    height: 240px;
    padding-top: 45px;
    &:hover {
      cursor: pointer;
    }
    .img-container {
      height: 185px;
      width: 100%;
      overflow-y: hidden;
      margin-bottom: 20px;
      &:hover {
      border: 2px solid white;
    }
    }
    span {
      text-transform: uppercase;
      font-size: .8rem;
      display: inline-block;
      &:hover {
      transform: scale(1.05);
    }
    }
  }
</style>