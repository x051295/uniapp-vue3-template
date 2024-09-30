<script setup>
const { locale, setLocale } = useI18n()
</script>

<template>
  <div class="h-full">
    <div>
      <button @click="setLocale('en')">英文</button>
      <br />
      <button @click="setLocale('zh-CN')">中文</button>
      <p>{{ locale }}</p>
      <h1>{{ $t('welcome') }}</h1>
    </div>
  </div>
</template>
