<template>
  <footer class="footer">
    <div class="container">
      <div class="footer-content">
        <div class="footer-left">
          <h4>Sekolah XYZ</h4>
          <p>Membentuk Generasi Emas</p>
          <address>
            <p>Jl. Depok, sukamenak, purbaratu</p>
            <p>...</p>
          </address>
        </div>
        <div class="footer-right">
          <h5>Ikuti Kami</h5>
          <ul class="social-links">
            <li><a href="https://facebook.com" target="_blank">Facebook</a></li>
            <li><a href="https://twitter.com" target="_blank">Twitter</a></li>
            <li><a href="https://instagram.com" target="_blank">Instagram</a></li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  background-color: #34495e;
  color: white;
  padding: 20px 0;
}

.footer .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.footer-content {
  display: flex;
  justify-content: space-between;
}

.footer-left {
  width: 50%;
}

.footer-left h4 {
  margin: 0;
  font-size: 1.5rem;
}

.footer-left p {
  margin: 5px 0;
}

.footer-right {
  width: 30%;
}

.footer-right h5 {
  margin: 0;
  font-size: 1.2rem;
}

.social-links {
  list-style-type: none;
  padding: 0;
}

.social-links li {
  display: inline-block;
  margin-right: 10px;
}

.social-links a {
  color: white;
  text-decoration: none;
}

.social-links a:hover {
  text-decoration: underline;
}
</style>
