<template>
  <div id="carouselExample" class="carousel slide" data-bs-ride="carousel">
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="https://alatlukis.co.id/wp-content/uploads/2023/10/Toko-Alat-alat-Lukis-Terdekat-3.jpg" class="d-block w-100 carousel-img" />
      </div>
      <div class="carousel-item">
        <img src="https://backend.andalanatk.com/upload/blog/1697698814_6.jpg" class="d-block w-100 carousel-img" />
      </div>
      <div class="carousel-item">
        <img src="https://png.pngtree.com/thumb_back/fw800/background/20230116/pngtree-colorful-art-painting-photography-image_1519323.jpg" class="d-block w-100 carousel-img" />
      </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
      <span class="carousel-control-prev-icon"></span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
      <span class="carousel-control-next-icon"></span>
    </button>
  </div>
</template>

<style scoped>
.carousel-img {
  height: 300px;
  object-fit: cover;
}
</style>