<template>
  <div class="col-md-4">
    <div class="card h-100 product-card">
      <img :src="img" class="card-img-top" :alt="title" />
      <div class="card-body">
        <h5 class="card-title">{{ title }}</h5>
        <p class="card-text">{{ desc }}</p>
        <a href="#" class="btn btn-primary">Beli Sekarang</a>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps(['title', 'desc', 'img'])
</script>

<style scoped>
.product-card {
  background-color: #f7f7f7;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
  border-radius: 12px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.product-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.25);
}
</style>