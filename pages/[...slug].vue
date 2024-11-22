<script setup>
const route = useRoute()
const router =useRouter()

definePageMeta({
    layout:'noPage'
})
</script>
<template>
  <div>
    <h1>404</h1>
    <h2>目前沒有這個 {{ route.fullPath }} 的 URL 唷</h2>
    <button type="button" @click="router.push('/')">回到首頁</button>
  </div>
</template>
<style scoped></style>