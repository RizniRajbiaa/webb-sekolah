<template>
  <div class="welcome-section">
    <div class="content">
      <h1 class="school-name">Selamat Datang di Sekolah Kami</h1>
      <p class="welcome-message">
        Kami dengan bangga mempersembahkan website resmi Sekolah XYZ, tempat untuk menumbuhkan generasi muda yang
        cerdas, kreatif, dan penuh semangat.
      </p>
      <p class="vision">
        Visi kami adalah untuk menciptakan lingkungan pendidikan yang inklusif dan mendukung perkembangan akademik serta
        karakter siswa. Bersama-sama, kita membangun masa depan yang lebih cerah.
      </p>
      <button @click="goToAboutPage" class="explore-button">Jelajahi Lebih Lanjut</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Sambutan",
  methods: {
    goToAboutPage() {
      // Arahkan pengguna ke halaman "About" atau informasi lebih lanjut
      this.$router.push({ name: "about" });
    }
  }
};
</script>

<style scoped>
.welcome-section {
  background-color: #f4f4f9;
  padding: 50px;
  text-align: center;
}

.content {
  max-width: 800px;
  margin: 0 auto;
}

.school-name {
  font-size: 36px;
  font-weight: bold;
  color: #2c3e50;
}

.welcome-message {
  font-size: 18px;
  color: #34495e;
  margin-top: 20px;
}

.vision {
  font-size: 16px;
  color: #7f8c8d;
  margin-top: 20px;
}

.explore-button {
  background-color: #3498db;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  margin-top: 30px;
  cursor: pointer;
}

.explore-button:hover {
  background-color: #2980b9;
}
</style>
