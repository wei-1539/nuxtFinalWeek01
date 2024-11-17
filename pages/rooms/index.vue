<script setup>
const route = useRoute()
</script>
<template>
  <div>
    <h1>客房列表頁面</h1>
    <ul class="navList">
        <li class="navItem">
          <NuxtLink class="navLink" :to="`${route.fullPath}/room001`">房型001</NuxtLink>
        </li>
        <li class="navItem">
          <NuxtLink class="navLink" :to="`${route.fullPath}/room002`">房型002</NuxtLink>
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
}
</style>