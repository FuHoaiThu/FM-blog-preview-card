<script setup>
const cardInfo = {
  id: 1,
  category: 'Learning',
  publishedAt: '21 Dec 2023',
  title: 'HTML & CSS foundations',
  description:
    'These languages are the backbone of every website, defining structure, content, and presentation.',
  image: '/images/illustration-article.svg',
  author: {
    name: 'Greg Hooper',
    avatar: '/images/image-avatar.webp',
  },
}
</script>

<template>
  <main class="card">
    <div class="card-image">
      <img src="./assets/illustration-article.svg" alt="Article Illustration" />
    </div>
    <div class="info">
      <div class="info-category">{{ cardInfo.category }}</div>
      <div class="info-published-at">{{ cardInfo.publishedAt }}</div>
      <div class="info-title">{{ cardInfo.title }}</div>
      <div class="info-description">{{ cardInfo.description }}</div>
      <!-- <div class="info-author">
        <img src="{{ cardInfo.author.avatar }}" alt="{{ cardInfo.author.name }}" />
        <span>{{ cardInfo.author.name }}</span>
      </div> -->
    </div>
  </main>
</template>

<style scoped>
.card {
  background-color: var(--cl-white);
  border: 1px solid var(--cl-gray-950);
  border-radius: 20px;
  box-shadow: 8px 8px 0px 0px #000000;
  padding: 20px;
  width: 336px;
}
.card .card-image {
  margin-bottom: 24px;
}
.card .card-image img {
  width: 100%;
  border-radius: 10px;
}
</style>
