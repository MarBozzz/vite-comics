<script>
export default {
  name : 'AppJumbotron'
}
</script>

<template>
  <div class="jumbotron"></div>
  <div class="current-series">
    <a class="btn" href="#">Current Series</a>
  </div>
</template>

<style lang="scss" scoped>
.jumbotron {
  height: 400px;
  background-image: url(../assets/img/jumbotron.jpg);
}
.current-series {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 245px;
  height: 55px; 
  background-color: #0282F9;
  position: absolute;
  top: 495px;
  left: 320px;
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
    font-size: 1.5rem;
    font-weight: bold;
  }
}
</style>