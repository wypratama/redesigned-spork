<template>
  <div class="navbar">
    <div>
      Home
    </div>
    <div>
      Antrian
    </div>
    <div>
      Regis
    </div>
    <div>
      Rajal
    </div>
    <div>
      Ranap
    </div>
    <div>
      Rekmed
    </div>
    <div>
      Farmasi
    </div>
    <div>
      Radiologi
    </div>
    <div>
      Lab
    </div>
    <div>
      Kasir
    </div>
    <div>
      Skere
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style lang="scss" scoped>
.navbar {
  background-color: navy;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  color: whitesmoke;
  width: 80px;
  height: 100%;
  webkit-box-sizing: border-box; /* Safari/Chrome, other WebKit */
  -moz-box-sizing: border-box;    /* Firefox, other Gecko */
  box-sizing: border-box;         /* Opera/IE 8+ */
}
</style>