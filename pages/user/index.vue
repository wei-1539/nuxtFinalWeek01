<script setup>
const route = useRoute()
</script>
<template>
  <div>
    <h1>會員首頁</h1>
    <ul class="navList">
        <li class="navItem">
          <NuxtLink class="navLink" :to="`${route.fullPath}/order`">訂單查詢</NuxtLink>
        </li>
        <li class="navItem">
          <NuxtLink class="navLink" :to="`${route.fullPath}/profile`">修改資料</NuxtLink>
        </li>
      
      </ul>
  </div>
</template>
<style scoped>
li{
  list-style: none;
}
a{
  text-decoration: none;
  color:#000;
}
.navList{
  display: flex;
  gap:15px;
}
.navLink{
  transition: all .3s;
  padding: 5px 10px;
  border-radius: 4px;
}
.navLink:hover{
  background-color: #585858;
  color:#fff;
}</style>