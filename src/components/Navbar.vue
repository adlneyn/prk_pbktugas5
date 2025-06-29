<template>
  <nav class="navbar navbar-expand-lg custom-navbar">
    <div class="container">
      <!-- Logo Toko dengan Ikon Kuas 🎨 -->
      <a class="navbar-brand fw-bold text-gradient" href="#">
        🎨 Artshopku
      </a>

      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link nav-text" href="#">Beranda</a></li>
          <li class="nav-item"><a class="nav-link nav-text" href="#">Produk</a></li>
          <li class="nav-item"><a class="nav-link nav-text" href="#">Kontak</a></li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style scoped>
.custom-navbar {
  background-color: #1f1f1f;
  padding: 0.75rem 1rem;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
}

.text-gradient {
  background: linear-gradient(45deg, #f9a825, #f06292, #64b5f6);
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
}

.nav-text {
  color: #f1f1f1;
  font-weight: 500;
  transition: 0.3s;
}

.nav-text:hover {
  color: #f9a825;
  text-decoration: underline;
}
</style>