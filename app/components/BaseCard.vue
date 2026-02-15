<template>
  <NuxtLink :to="to" class="card">
    <img v-if="image" :src="image" :alt="title" class="card-image" />
    <div class="card-content">
      <h3 class="card-title">{{ title }}</h3>
      <slot />
    </div>
  </NuxtLink>
</template>

<script setup>
defineProps({
  title: String,
  image: String,
  to: String
})
</script>

<style scoped>
.card {
font-weight: 800;
  color: #ce50a8;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  border: 2px solid #ded0d0;
  border-radius: 20px;
  overflow: hidden;
  transition: all 0.2s ease;
  background: white;
  margin: 10px;
  display:flex;
  justify-content: center;
  flex-direction: column;
  height:100%;
  width: 50%;
  margin-left: 60px;
  margin-right: 60px;
  margin-top: 100px;
}
.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  border-color: #ce50a8;
  border-radius: 15px;
}
.card-image {
  width: 100%;
  height: 150px;
  object-fit: cover;
}
.card-content {
  padding: 16px;
  text-align: center;
  margin-top: auto;
}
.card-title{
  font-size: 20px;
}
</style>