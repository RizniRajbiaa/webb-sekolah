<template>
  <div>
    <h2 class="title">Konsentrasi Keahlian</h2>
    <div class="container">
        <!-- Kartu pertama -->
        <div class="card">
            <img src="/assets/img/TKJ.jpeg" alt="Gambar Teknik Informatika">
            <div class="card-body">
                <h3>Teknik Informatika</h3>
            </div>
        </div>
        
        <!-- Kartu kedua -->
        <div class="card">
            <img src="/assets/img/PPLG.jpeg" alt="Gambar PPLG">
            <div class="card-body">
                <h3>PPLG</h3>
            </div>
        </div>
        
        <!-- Kartu ketiga -->
        <div class="card">
            <img src="/assets/img/TSM.jpeg" alt="Gambar TSM">
            <div class="card-body">
                <h3>TSM</h3>
            </div>
        </div>
        
        <!-- Kartu keempat -->
        <div class="card">
            <img src="/assets/img/TOI.jpeg" alt="Gambar TOI">
            <div class="card-body">
                <h3>TOI</h3>
            </div>
        </div>
    </div>
  </div>
</template>

<style scoped>
        /* Gaya dasar untuk kartu jurusan */
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