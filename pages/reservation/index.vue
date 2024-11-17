<script setup>
const route = useRoute()
</script>
<template>
  <div>
    <h1>預約首頁</h1>
    <ul class="navList">
      <li class="navItem">
        <NuxtLink class="navLink" :to="`${route.fullPath}/success`"
          >預約成功/失敗</NuxtLink
        >
      </li>

    </ul>
  </div>
</template>
<style scoped>
li {
  list-style: none;
}
a {
  text-decoration: none;
  color: #000;
}
.navList {
  display: flex;
  gap: 15px;
}
.navLink {
  transition: all 0.3s;
  padding: 5px 10px;
  border-radius: 4px;
}
.navLink:hover {
  background-color: #585858;
  color: #fff;
}
</style>