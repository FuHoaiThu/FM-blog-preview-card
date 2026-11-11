<script setup>
import aritcleImg from '@/assets/illustration-article.svg'
import avatarImg from '@/assets/image-avatar.webp'
const cardInfo = {
  id: 1,
  category: 'Learning',
  publishedAt: '21 Dec 2023',
  title: 'HTML & CSS foundations',
  description:
    'These languages are the backbone of every website, defining structure, content, and presentation.',
  image: aritcleImg,
  author: {
    name: 'Greg Hooper',
    avatar: avatarImg,
  },
}
</script>

<template>
  <main class="card">
    <div class="card-image">
      <img :src="cardInfo.image" alt="Article Illustration" />
    </div>
    <div class="info">
      <div class="info-category text-preset-3-bold">{{ cardInfo.category }}</div>
      <div class="info-published-at text-preset-3">{{ cardInfo.publishedAt }}</div>
      <div class="info-title text-preset-1">{{ cardInfo.title }}</div>
      <div class="info-description text-preset-2">{{ cardInfo.description }}</div>
    </div>
    <div class="author">
      <img :src="cardInfo.author.avatar" :alt="cardInfo.author.name" />
      <span class="text-preset-3-bold">{{ cardInfo.author.name }}</span>
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
  width: min(384px, calc(100vw - 48px));
}
.card .card-image {
  margin-bottom: 24px;
}
.card .card-image img {
  width: 100%;
  border-radius: 10px;
  display: block;
}
.info {
  display: flex;
  color: var(--cl-gray-950);
  flex-direction: column;
  gap: 12px;
  margin-bottom: 24px;
}
.info .info-category {
  border-radius: 4px;
  background-color: var(--cl-yellow);
  padding: 4px 12px;
  width: fit-content;
}
.info .info-description {
  color: var(--cl-gray-500);
}
.info .info-title:hover {
  color: var(--cl-yellow)
}
.author {
  display: flex;
  align-items: center;
  gap: 12px;
}
.author img {
  width: 32px;
  height: 32px;
}
</style>
