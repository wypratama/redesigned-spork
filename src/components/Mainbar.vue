<template>
  <div class="main-bar">
    <ul>
      <li>Pengkajian Awal</li>
      <li>Lab/Radiologi</li>
      <li>CPPT Ranap</li>
      <li>Informed Concern</li>
      <li>Skrining</li>
      <li>Rekonsiliasi Obat</li>
      <li>Resume Medis</li>
    </ul>
      <img src="../assets/img/menu.png" alt="">
  </div>
</template>

<script>
export default {
  name: 'Mainbar'
}
</script>

<style lang="scss" scoped>
.main-bar {
  width: 100%;
  height: 50px;
  background-color: navy;
  color: navy;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  -webkit-box-sizing: border-box; /* Safari/Chrome, other WebKit */
  -moz-box-sizing: border-box;    /* Firefox, other Gecko */
  box-sizing: border-box;         /* Opera/IE 8+ */
  padding: 0 5px;
  gap: 5px;
  font-size: 18px;
  font-weight: 800;
  margin-top: 15px;

  ul {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    list-style-type: none;
    gap: 2px;
    flex-grow: 1;
    height: 35px;
  }

  li {
    background-color: slategray;
    padding: 5px 10px;
    flex-grow: 1;
    flex-basis: 0;
    display: flex;
    justify-content: center;
    align-items: center;

    &:first-of-type {
      background-color: yellow;
    }
  }

  img {
    width: 20px;
    height: 20px;
  }
}
</style>