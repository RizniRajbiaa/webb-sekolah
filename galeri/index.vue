<template>
    <div class="gallery-page">
      <header>
        <h1>Galeri Sekolah</h1>
      </header>
      <section class="gallery-grid">
        <div v-for="photo in photos" :key="photo.id" class="gallery-item">
          <img :src="photo.src" :alt="photo.alt" class="gallery-photo" />
          <p class="photo-caption">{{ photo.caption }}</p>
        </div>
      </section>
    </div>
  </template>
  
  <script>
  export default {
    name: 'GalleryPage',
    data() {
      return {
        photos: [
          { id: 1, src: 'https://via.placeholder.com/300x200?text=Kegiatan+1', alt: 'Kegiatan 1', caption: 'Kegiatan Belajar' },
          { id: 2, src: 'https://via.placeholder.com/300x200?text=Acara+1', alt: 'Acara 1', caption: 'Acara Lomba' },
          { id: 3, src: 'https://via.placeholder.com/300x200?text=Ekskul+1', alt: 'Ekskul 1', caption: 'Ekskul Musik' },
          { id: 4, src: 'https://via.placeholder.com/300x200?text=Kegiatan+2', alt: 'Kegiatan 2', caption: 'Kegiatan Olahraga' },
          { id: 5, src: 'https://via.placeholder.com/300x200?text=Acara+2', alt: 'Acara 2', caption: 'Acara Peringatan' },
          { id: 6, src: 'https://via.placeholder.com/300x200?text=Ekskul+2', alt: 'Ekskul 2', caption: 'Ekskul Seni' },
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  .gallery-page {
    text-align: center;
    padding: 20px;
  }
  
  header {
    margin-bottom: 20px;
  }
  
  h1 {
    font-size: 2.5rem;
    color: #333;
  }
  
  .gallery-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 16px;
    padding: 20px;
  }
  
  .gallery-item {
    text-align: center;
    border: 1px solid #ddd;
    border-radius: 8px;
    padding: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }
  
  .gallery-photo {
    max-width: 100%;
    height: auto;
    border-radius: 8px;
  }
  
  .photo-caption {
    margin-top: 10px;
    font-size: 1rem;
    color: #333;
  }
  </style>
  