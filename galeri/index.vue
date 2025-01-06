<template>
  <div>
    <h2 class="title">Galeri Sekolah</h2>
    <div class="container">
      <!-- Kartu pertama -->
      <div class="card">
        <img src="/assets/img/Jobfair.jpeg" alt="Gambar Job fair">
        <div class="card-body">
          <h3>JOB FAIR</h3>
        </div>
      </div>

      <!-- Kartu kedua -->
      <div class="card">
        <img src="/assets/img/Olahraga.jpeg" alt="Gambar Olahraga">
        <div class="card-body">
          <h3>OLAHRAGA</h3>
        </div>
      </div>

      <!-- Kartu ketiga -->
      <div class="card">
        <img src="/assets/img/Pramuka.jpeg" alt="Gambar Pramuka">
        <div class="card-body">
          <h3>PRAMUKA</h3>
        </div>
      </div>

      <!-- Kartu keempat -->
      <div class="card">
        <img src="/assets/img/Upacara.jpeg" alt="Gambar Upacara">
        <div class="card-body">
          <h3>UPACARA</h3>
        </div>
      </div>
      <!--Kartu kelima-->
      <div class="card">
        <img src="/assets/img/Pengajian.jpeg" alt="Gambar Pengajian">
        <div class="card-body">
          <h3>PENGAJIAN</h3>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
/* Gaya dasar untuk kartu galeri */
.container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 20px;
  margin-top: 20px;
}

.card {
  background-color: #fff;
  width: 250px;
  border: 1px solid #ddd;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  overflow: hidden;
  text-align: center;
  transition: transform 0.3s ease;
}

.card:hover {
  transform: scale(1.05);
}

.card img {
  width: 100%;
  height: 150px;
  object-fit: cover;
}

.card-body {
  padding: 15px;
}

.card h3 {
  font-size: 20px;
  color: #333;
  margin-bottom: 10px;
}

.title {
  text-align: center;
  margin-bottom: 20px;
}
</style>