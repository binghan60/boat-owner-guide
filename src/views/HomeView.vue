<script setup>
import HeaderComponent from '@/components/HeaderComponent.vue'
import FooterComponent from '@/components/FooterComponent.vue'
</script>

<template>
  <HeaderComponent></HeaderComponent>

  <div class="container mx-auto">
    <div class="grid grid-cols-1 lg:grid-cols-2 gap-6 mx-4 my-8">
      <div class="bg-blue-50 min-h-[200px] rounded-2xl shadow-md p-6 hover:shadow-xl transition duration-300">
        <h3 class="text-xl font-semibold text-blue-900 mb-4">📌 申請帳號</h3>
        <p class="text-gray-700">線上註冊個人帳號，快速建立專屬資料。</p>
      </div>
      <div class="bg-blue-50 min-h-[200px] rounded-2xl shadow-md p-6 hover:shadow-xl transition duration-300">
        <h3 class="text-xl font-semibold text-blue-900 mb-4">📄 登入系統</h3>
        <p class="text-gray-700">使用手機號碼做為登入，無須記任何密碼，登入後享有完整服務。</p>
      </div>
      <div class="bg-blue-50 min-h-[200px] rounded-2xl shadow-md p-6 hover:shadow-xl transition duration-300">
        <h3 class="text-xl font-semibold text-blue-900 mb-4">✅ 線上預約檢查</h3>
        <p class="text-gray-700">自由選擇檢查日期和時間，簡單便利。</p>
      </div>
      <div class="bg-blue-50 min-h-[200px] rounded-2xl shadow-md p-6 hover:shadow-xl transition duration-300">
        <h3 class="text-xl font-semibold text-blue-900 mb-4">📬 如何查詢申請進度</h3>
        <p class="text-gray-700">隨時掌握申請進度，不再需要多次確認。</p>
      </div>
      <div class="bg-blue-50 min-h-[200px] rounded-2xl shadow-md p-6 hover:shadow-xl transition duration-300">
        <h3 class="text-xl font-semibold text-blue-900 mb-4">💡 常見問題</h3>
        <details class="rounded-lg overflow-hidden">
          <summary class="cursor-pointer bg-sky-50 text-sky-700 font-semibold py-3 px-4 hover:bg-sky-100">登入需要密碼嗎？如果我忘記密碼怎麼辦？</summary>
          <p class="text-gray-700 py-3 px-4 bg-white">您在本平臺無須記錄任何密碼，只要輸入傳送到您手機上的驗證碼即可。</p>
        </details>

        <details class="rounded-lg overflow-hidden">
          <summary class="cursor-pointer bg-sky-50 text-sky-700 font-semibold py-3 px-4 hover:bg-sky-100">可以在線上下載繳費單嗎？</summary>
          <p class="text-gray-700 py-3 px-4 bg-white">可以，請進入「僅查進度查詢」進行下載。</p>
        </details>

        <details class="rounded-lg overflow-hidden">
          <summary class="cursor-pointer bg-sky-50 text-sky-700 font-semibold py-3 px-4 hover:bg-sky-100">查詢進度時無法顯示資料？</summary>
          <p class="text-gray-700 py-3 px-4 bg-white">請確認帳號是否正確登入，或聯絡客服協助。</p>
        </details>
      </div>
    </div>
  </div>
  <footer-component></footer-component>
</template>

<style scoped>
summary::-webkit-details-marker {
  display: none;
}
summary::marker {
  font-size: 0;
}
summary::before {
  content: '▶';
  display: inline-block;
  transition: transform 0.2s;
  margin-right: 0.5rem;
}
details[open] > summary::before {
  transform: rotate(90deg);
}
</style>
