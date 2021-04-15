<template>
  <div class="container">
    <Navbar />
    <div class="main-content">
      <Topbar />
      <Mainbar />
      <MainContent />
    </div>
  </div>
</template>

<script>
import Navbar from '../components/Navbar'
import Topbar from '../components/Topbar'
import Mainbar from '../components/Mainbar'
import MainContent from '../components/MainContent'

export default {
  name: 'Tahap3',
  components: {
    Navbar,
    Topbar,
    Mainbar,
    MainContent
  }
}
</script>

<style lang="scss" scoped>
.container {
  display: flex;
  flex-direction: row;
  height: 100vh;
  width: 100vw;
  -webkit-box-sizing: border-box; /* Safari/Chrome, other WebKit */
  -moz-box-sizing: border-box;    /* Firefox, other Gecko */
  box-sizing: border-box;         /* Opera/IE 8+ */
}

.main-content {
  width: 100%;
  padding: 15px 10px;
  box-sizing: border-box;         /* Opera/IE 8+ */
  -webkit-box-sizing: border-box; /* Safari/Chrome, other WebKit */
  -moz-box-sizing: border-box;    /* Firefox, other Gecko */
  display: flex;
  flex-direction: column;
}
</style>