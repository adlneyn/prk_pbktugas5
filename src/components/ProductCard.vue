<template>
  <div class="col-md-4">
    <div class="card h-100">
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