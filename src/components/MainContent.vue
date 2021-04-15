<template>
  <div class="main-information">
    <div class="main-info left">
      <h3>RIWAYAT BEROBAT</h3>
      <div class="timeline">
        <div>
          <span>25 Okt 2020</span>
          <span>IGD-RANAP</span>
        </div>
        <div>
          <span>3 Okt 2020</span>
          <span>RAJAL</span>
        </div>
        <div>
          <span>4 Sep 2020</span>
          <span>RAJAL</span>
        </div>
        <div>
          <span>20 Jun 2020</span>
          <span>IGD</span>
        </div>
        <div>
          <span>1 Feb 2020</span>
          <span>IGD-RANAP</span>
        </div>
      </div>
    </div>
    <div class="main-info right">
      <div class="navigasi-pasien">
        <ul>
          <li>Anamnesis</li>
          <li>Riw. Alergi</li>
          <li>Status Nyeri</li>
          <li>Fungsional</li>
          <li>Resiko Jatuh</li>
          <li>Skrining Gizi</li>
          <li>Edukasi</li>
          <li>Pem. Fisik</li>
          <li>Lab</li>
          <li>Radiologi</li>
          <li>Daf. Masalah</li>
          <li>Tatalaksana</li>
          <li>Riw. obat</li>
        </ul>
      </div>
      <div>
        <h2>PENGKAJIAN AWAL PASIEN RAWAT INAP</h2>
        <div class="informasi-pasien">
          <div>
            <span>Autoanamnesis</span>
            <span>Alloanamnesis: Tn. Rizal (Suami)</span>
          </div>
          <div>
            <span>Tanggal Masuk Bangsal: Senin, 26 Oktober, 12.00 WIB</span>
            <span>Anamnesis oleh: dr. Sukma Ayu</span>
          </div>
        </div>
        <input type="text" name="" id="">
        <input type="text" name="" id="">
        <input type="text" name="" id="">
        <input type="text" name="" id="">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MainContent'
}
</script>

<style lang="scss" scoped>
.main-information {
  display: flex;
  width: 100%;
  margin-top: 10px;
  box-sizing: border-box;         /* Opera/IE 8+ */
  -webkit-box-sizing: border-box; /* Safari/Chrome, other WebKit */
  -moz-box-sizing: border-box;    /* Firefox, other Gecko */
  flex-grow: 1;
  gap: 10px;
  // overflow: scroll;
}

.right {
  display: flex;
  flex-direction: row;
  background-color: navy;
  width: 100%;
  color: white;
}

.left {
  background-color: rgba(steelblue, 0.5);
  height: 100%;
  border-radius: 6px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  gap: 5px;
  box-sizing: border-box;         /* Opera/IE 8+ */
  -webkit-box-sizing: border-box; /* Safari/Chrome, other WebKit */
  -moz-box-sizing: border-box;    /* Firefox, other Gecko */
  padding: 8px;
}

.timeline {
  flex-grow: 1;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  position: relative;

  div {
    display: flex;
    flex-direction: column;

    &:before {
      content: '';
      height: 25px;
      width: 25px;
      background-color: whitesmoke;
      border: 6px solid blue;
      border-radius: 50%;
      position: absolute;
    }
  }

  &::before {
    content: '';
    height: 80%;
    width: 15px;
    background-color: gray;
    position: absolute;
    left: 10px;
  }
}

.navigasi-pasien {
  background-color: black;
  display: flex;
  flex-direction: column;
  
  ul {
    height: 100%;

    li {
      list-style-type: none;
      box-sizing: border-box;         /* Opera/IE 8+ */
      -webkit-box-sizing: border-box; /* Safari/Chrome, other WebKit */
      -moz-box-sizing: border-box;    /* Firefox, other Gecko */
      width: 130px;
      height: 50px;
    }
  }
}
</style>