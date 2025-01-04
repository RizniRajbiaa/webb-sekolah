<template>
  <div class="container">
    <h2 class="text-center mb-4">Daftar Ekstrakurikuler</h2>
    <div class="row">
      <div class="col" v-for="ekstra in ekstrakurikuler" :key="ekstra.id">
        <div class="card">
          <img :src="ekstra.gambar" class="card-img-top" :alt="ekstra.nama" />
          <div class="card-body">
            <h5 class="card-title">{{ ekstra.nama }}</h5>
            <p class="card-text">{{ ekstra.deskripsi }}</p>
            <a :href="ekstra.link" class="btn btn-primary">Lihat Detail</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      ekstrakulikuler: [
        {
          id: 1,
          nama: "PRAMUKA",
          gambar: "~/assets/img/PRAMUKA.jpeg",
        },
        {
          id: 2,
          nama: "FUTSAL",
          gambar: '~/assets/img/FUTSAL.jpeg',
        },
        {
          id: 3,
          nama: "ENGLISH CLUB",
          gambar: "~/assets/img/ENGLISHCLUB.jpeg",
        },
        {
          id: 4,
          nama: "Paskibra"
          gambar: "~/assets/img/paskibraa.jpeg"
        },
        {
          id: 5,
          nama: "PLH"
          gambar: "~/assets/img/PLH.jpeg"
        },
        {
          id: 4,
          nama: "PERISAI DIRI"
          gambar: "~/assets/img/PERISAI DIRI.jpeg",
        }
        {
          id: 4,
          nama: "VOLLY"
          gambar: "~/assets/img/VOLLY.jpeg",
        }
        {
          id: 4,
          nama: "BADMINTON"
          gambar: "~/assets/img/BADMINTON.jpeg",
        }
        {
          id: 4,
          nama: "IRMA"
          gambar: "~/assets/img/IRMA.jpeg",
        }
        {
          id: 4,
          nama: "CINEMA"
          gambar: "~/assets/img/CINEMA.jpeg",
        }
        {
          id: 4,
          nama: "ITClub"
          gambar: "~/assets/img/ITCLUB.jpeg",
        }
        {
          id: 4,
          nama: "LASKAR PUSTAKA"
          gambar: "~/assets/img/LASKAR PUSTAKA.jpeg",
        }
        {
          id: 4,
          nama: "PKS"
          gambar: "~/assets/img/PKS.jpeg",
        }
        {
          id: 4,
          nama: "PMR"
          gambar: "~/assets/img/PMR.jpeg",
        }
        {
          id: 4,
          nama: "SRL"
          gambar: "~/assets/img/SRL.jpeg",
        }
      ]
    }
  }
}
</script>

<style scoped>
.container {
  max-width: 1200px;
  margin: auto;
  padding: 20px;
}

h2 {
  font-size: 2rem;
  color: #424242;
}

.row {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}

.col {
  flex: 1 0 21%;
  /* Responsif: 4 kolom di desktop */
  min-width: 250px;
  margin-bottom: 20px;
}

.card {
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}

.card img {
  max-height: 200px;
  object-fit: cover;
  width: 100%;
}

.card-body {
  padding: 15px;
}

.card-title {
  font-size: 1.25rem;
  color: #333;
  margin-bottom: 10px;
}

.card-text {
  font-size: 1rem;
  color: #555;
  margin-bottom: 15px;
}

.btn {
  font-size: 1rem;
  padding: 8px 20px;
}

/* Responsivitas */
@media (max-width: 768px) {
  .row {
    justify-content: center;
  }

  .col {
    flex: 1 0 45%;
    /* 2 kolom di layar kecil */
  }
}

@media (max-width: 480px) {
  .col {
    flex: 1 0 100%;
    /* 1 kolom penuh pada layar ekstra kecil */
  }
}
</style>