<template>
  <div>
    <TopbarNav />
    <div class="information-bar">
      <div class="information-top">
        <div>
          <span>NAMA (USIA)</span>
          <h3> NY. MARIANA (23)</h3>
        </div>
        <div>
          <span>TANGGAL LAHIR</span>
          <h3>13 JAN 1997</h3>
        </div>
        <div>
          <span>NOMOR REKAM MEDIS</span>
          <h3>001234567</h3>
        </div>
        <div>
          <span>DPJP</span>
          <h3>dr. Febri Bahari, SpPD, KGEH</h3>
        </div>
        <div>
          <span>ANDA MASUK SEBAGAI</span>
          <h3>dr. Dany Petra, SpPD</h3>
        </div>
      </div>
      <div class="information-bot">
        <div class="information-bot-content left-content">
          <div>
            <span>KELUHAN UTAMA</span>
            <h3>KU: Muntah berdarah sejak 1 hari yang lalu</h3>
          </div>
          <div>
            <span>DIAGNOSIS PRIMER DAN SEKUNDER</span>
            <h3>DP: Eshopageal varices with bleeding (I85.01)</h3>
          </div>
        </div>
        <div class="information-bot-content right-content">
          <div class="infotmation-bot-header">
            <h3>TANDA-TANDA VITAL</h3>
            <h3>H+3</h3>
            <span>Last Update: Selasa, 27 Okt 2020, 06.30 WIB</span>
          </div>
          <div class="information-bot-main">
            <div>
              <span>KESADARAN</span>
              <h4>Compos Mentis</h4>
            </div>
            <div>
              <span>Tekanan Darah</span>
              <h4>110/70</h4>
              <span>mmHg</span>
            </div>
            <div>
              <span>LAJU NADI</span>
              <h4>120</h4>
              <span>kali/menit</span>
            </div>
            <div>
              <span>LAJU NAPAS</span>
              <h4>20</h4>
              <span>kali/menit</span>
            </div>
            <div>
              <span>SUHU TUBUH</span>
              <h4>37,3</h4>
              <span>oC</span>
            </div>
            <div>
              <span>EWS</span>
              <h4>3</h4>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TopbarNav from '../components/topbar/TopbarNav'

export default {
  name: 'Topbar',
  components: {
    TopbarNav
  }
}
</script>

<style lang="scss">
.information-bar {
  display: flex;
  flex-direction: column;
  gap: 10px;
  margin-top: 15px;

  div {
    display: flex;
    flex-direction: row;
    // width: 100%;
  }
}

.information-top {
  width: 100%;
  justify-content: space-between;
  gap: 3px;

  div {
    display: flex;
    flex-direction: column;
    background-color: rgba(steelblue, 0.5);
    border-radius: 6px;
    height: 70px;
    justify-content: space-evenly;
    flex-grow: 1;

    span {
      font-size: 12px;
    }

    h3 {
      font-size: 24px;
      font-weight: 800;
    }
  }
}

.information-bot {
  width: 100%;
  justify-content: space-between;
  gap: 10px;
}
  
.information-bot-content {
  display: flex;
  flex-direction: column !important;
  background-color: rgba(steelblue, 0.5);
  border-radius: 6px;
  flex-grow: 1;
  padding: 10px;
}

.left-content {
  gap: 10px;
    div {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }
}

.infotmation-bot-header {
  gap: 3px;
  justify-content: space-around;
}

.information-bot-main {
  justify-content: space-around;

  div {
    display: flex;
    flex-direction: column !important;
  }
}
</style>