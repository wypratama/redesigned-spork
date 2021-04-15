<template>
  <div class="topbar-nav">
    <img src="../../assets/img/back-arrow.png" alt="">
    <div class="top-header">
      <h3>RAWAT JALAN</h3>
    </div>
    <input type="text" name="" id="">
  </div>
</template>

<script>
export default {
  name: 'TopbarNav'
}
</script>

<style lang="scss" scoped>
.topbar-nav {
  display: flex;
  flex-direction: row;
  width: 100%;
  justify-content: space-between;
  img {
    width: 30px;
    height: 30px;
  }

  .top-header {
    border: red;
    border-width: 2px;
    background-color: red;
    width: 100%;
  }
}
</style>