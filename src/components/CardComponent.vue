<script setup>
import { ref } from 'vue';

const card = ref([
  {
    title: '如何申請帳號',
    description: '線上註冊個人帳號，快速建立專屬資料。',
    link: '#',
    linkText: '觀看教學影片',
  },
  {
    title: '如何使用系統',
    description: '系統操作說明，讓您快速上手。',
    link: '#',
    linkText: '觀看教學影片',
  },
]);

const
</script>

<template>
  <div class="flex flex-col items-center justify-center w-1/2 h-screen bg-gray-100">
    <div><h3 class="text-lg font-semibold text-cyan-600">如何申請帳號</h3></div>
    <div><p>線上註冊個人帳號，快速建立專屬資料。</p></div>
    <div><a href="#" class="text-cyan-600"> 觀看教學影片</a></div>
  </div>
</template>
