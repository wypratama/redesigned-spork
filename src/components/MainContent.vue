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
        <ul class="menu-navigasi-utama">
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
      <div class="informasi-umum">
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
        <textarea name="" id="keluhan-utama" placeholder="KELUHAN UTAMA:" cols="8"></textarea>
        <textarea name="" id="riwayat-penyakit-dahulu" placeholder="RIWAYAT PENYAKIT DAHULU:" ></textarea>
        <textarea name="" id="riwayat-penyakit-sekarang" placeholder="RIWAYAT PENYAKIT SEKARANG:" ></textarea>
        <textarea name="" id="riwayat-penyakit-keluarga" placeholder="RIWAYAT PENYAKIT KELUARGA:" ></textarea>
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
  margin: 8px;
  border-radius: 6px;
}

.menu-navigasi-utama {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  height: 100%;
  box-sizing: border-box;         /* Opera/IE 8+ */
  -webkit-box-sizing: border-box; /* Safari/Chrome, other WebKit */
  -moz-box-sizing: border-box;    /* Firefox, other Gecko */
  gap: 6px;
  padding: 10px;

   li {
      list-style-type: none;
      box-sizing: border-box;         /* Opera/IE 8+ */
      -webkit-box-sizing: border-box; /* Safari/Chrome, other WebKit */
      -moz-box-sizing: border-box;    /* Firefox, other Gecko */
      width: 130px;
      background-color: whitesmoke;
      color: gray;
      font-size: 18px;
      font-weight: 800;
      flex-grow: 1;
      border-radius: 6px;
      display: flex;
      justify-content: center;
      align-items: center;

      &:first-of-type {
        background-color: yellow;
        color: navy;
      }
    }
}

.informasi-umum {
  display: flex;
  flex-direction: column;
  background-color: whitesmoke;
  justify-content: space-around;
  color: black;
  flex-grow: 1;
  margin: 8px;
  border-radius: 6px;
  box-sizing: border-box;         /* Opera/IE 8+ */
  -webkit-box-sizing: border-box; /* Safari/Chrome, other WebKit */
  -moz-box-sizing: border-box;    /* Firefox, other Gecko */
  padding: 5px 40px;
  gap: 5px;

  h2 {
    font-size: 18px;
  }

  textarea {
    flex-grow: 1;
    border-radius: 6px;
    padding: 5px;
  }
}

.informasi-pasien {
  display: flex;
  width: 100%;
  justify-content: space-between;
  // margin-bottom: 5px;

  div {
    display: flex;
    flex-direction: column;

    &:first-of-type {
      text-align: left;
      
      span {
        margin-left: 10px;
        padding-left: 5px;
        position: relative;

        &::before {
          content: '';
          height: 5px;
          width: 5px;
          background-color: whitesmoke;
          border: 2px solid black;
          border-radius: 50%;
          position: absolute;
          left: -10px;
          top: 3px;
        }

        &:last-of-type {
           &::before {
            background-color: green;
          }
        }
      }
    }

    &:last-of-type {
      text-align: end;
    }
  }
}

#keluhan-utama {
  // height: 50px;
  // display: l;
}
</style>