<template>
  <div>
    <Navbar />
    <Carousel />
    <section class="py-5 bg-light">
      <div class="container">
        <h2 class="text-center mb-4">Produk Unggulan</h2>
        <div class="row g-4">
          <ProductCard
            v-for="(product, index) in products"
            :key="index"
            :title="product.title"
            :desc="product.desc"
            :img="product.img"
          />
        </div>
      </div>
    </section>
    <Footer />
  </div>
</template>

<script setup>
import Navbar from './components/Navbar.vue'
import Carousel from './components/Carousel.vue'
import ProductCard from './components/ProductCard.vue'
import Footer from './components/Footer.vue'

const products = [
  {
    title: 'Kuas Lukis Premium',
    desc: 'Rasakan sapuan halus dan detail sempurna dengan kuas berbulu lembut, kuat, dan nyaman digenggam. Bikin lukisan lebih rapi dan memukau.',
    img: 'https://ae01.alicdn.com/kf/Sadbb03fb22b846309803a1fca8f62764g.jpg_640x640q90.jpg'
  },
  {
    title: 'Kanvas Lukis',
    desc: 'Kanvas berkualitas dengan permukaan halus dan rangka kokoh. Siap pakai, warna lebih hidup, cocok untuk berbagai teknik lukis.',
    img: 'https://www.robians.com/wp-content/uploads/2024/02/3bb73a1c-bdc9-4a3f-b5ec-1c0cef14fcb6-1.jpg'
  },
  {
    title: 'Cat Akrilik',
    desc: 'Cat akrilik warna cerah, cepat kering, dan mudah diaplikasikan di berbagai media. Bikin karya awet dan detail lebih tajam.',
    img: 'https://sc04.alicdn.com/kf/H535ea4c7f1dd4acb9e1c03a14a89f99em.jpg'
  }
]
</script>