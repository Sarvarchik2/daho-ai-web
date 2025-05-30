<template>
  <div class="dahoai-wrapper">


  <header>
    <h1>Все необходимые вам <br> инструменты ИИ.</h1>
    <NuxtLink>Начните бесплатно</NuxtLink>
    <span class="header-span"></span>
    <p>Присоединяйтесь к 7383 счастливым <br>  пользователям, и их число растёт</p>
    <div class="header-ai">
      <img src="@/assets/ai/image%202.svg" alt="ai">
      <img src="@/assets/ai/image%203.svg" alt="ai">
    </div>
  </header>
  </div>
</template>


<style>
header{
  width: 100%;
  display: flex;
  flex-direction: column;
  gap: 30px;
  align-items: center;
}
header h1{
  font-size: 64px;
  line-height: 80px;
  text-align: center;
  font-weight: bold;
}
header a{
  text-decoration: none;
  color: #000;
  font-size: 32px;
  border: 2px solid #000000;
  width: max-content;
  border-radius: 50px;
  padding: 16px 30px;
}
header p{
  color: #000;
  font-size: 32px;
  text-align: center;
}
.header-span{
  width: 50%;

  height: 2px;
  background-color: #000000;
}
</style>
<script setup lang="ts">
</script>