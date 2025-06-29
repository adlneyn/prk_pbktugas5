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
    desc: 'Kuas lukis premium ini hadir untuk kamu yang ingin merasakan sensasi melukis yang lebih halus dan profesional. Dibuat dari bulu pilihan yang lembut namun kuat, kuas ini mampu memberikan sapuan warna yang rata, detail yang tajam, dan hasil karya yang tampak hidup. Gagangnya pun dirancang nyaman digenggam, sehingga tangan tidak cepat pegal meski melukis berjam-jam. Dengan kuas lukis premium ini, setiap goresan kuas akan terasa lebih presisi dan hasil lukisan pun terlihat lebih memukau. Cocok untuk pemula hingga seniman berpengalaman yang mengutamakan kualitas dalam setiap karya.',
    img: 'https://ae01.alicdn.com/kf/Sadbb03fb22b846309803a1fca8f62764g.jpg_640x640q90.jpg'
  },
  {
    title: 'Kanvas Lukis',
    desc: 'Kanvas berkualitas ini siap jadi teman setia setiap ide kreatifmu. Terbuat dari bahan linen atau katun tebal dengan anyaman rapat, kanvas ini mampu menahan cat dengan baik dan membuat warna terlihat lebih hidup. Rangkanya kokoh dan permukaannya sudah dipersiapkan agar cat menempel sempurna, sehingga kamu bisa langsung mulai melukis tanpa repot. Dengan kanvas ini, setiap detail karya akan tampak lebih tajam dan tahan lama. Cocok untuk cat minyak, cat akrilik, maupun media campuran, kanvas ini jadi pilihan tepat untuk siapa saja yang ingin menghasilkan lukisan yang indah dan bernilai seni tinggi.',
    img: 'https://www.robians.com/wp-content/uploads/2024/02/3bb73a1c-bdc9-4a3f-b5ec-1c0cef14fcb6-1.jpg'
  },
  {
    title: 'Cat Akrilik',
    desc: 'Cat akrilik ini hadir untuk kamu yang ingin berkarya dengan warna-warna cerah dan tahan lama. Teksturnya kental dan mudah diaplikasikan, sehingga cocok untuk berbagai teknik lukis, mulai dari sapuan tipis hingga lapisan tebal dengan efek tekstur. Warnanya cepat kering, tidak mudah pudar, dan melekat sempurna di kanvas, kertas, kayu, atau media lainnya. Dengan cat akrilik ini, setiap detail lukisanmu akan tampak hidup dan memukau. Pilihan warnanya pun lengkap, memudahkan kamu untuk berkreasi dan mencampur warna sesuai imajinasi. Cocok untuk pemula hingga seniman profesional yang ingin hasil karya berkualitas tinggi.',
    img: 'https://sc04.alicdn.com/kf/H535ea4c7f1dd4acb9e1c03a14a89f99em.jpg'
  }
]
</script>