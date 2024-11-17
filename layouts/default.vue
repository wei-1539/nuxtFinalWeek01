<script setup lang="ts"></script>

<template>
  <div>
    <header>
      <ul class="navList">
        <li class="navItem">
          <NuxtLink class="navLink" to="/">首頁</NuxtLink>
        </li>
        <li class="navItem">
          <NuxtLink class="navLink" to="/rooms">客房介紹</NuxtLink>
        </li>
        <li class="navItem">
          <NuxtLink class="navLink" to="/reservation">預約頁面</NuxtLink>
        </li>
        <li class="navItem">
          <NuxtLink class="navLink" to="/user">會員頁面</NuxtLink>
        </li>
        <li class="navItem">
          <NuxtLink class="navLink" to="/login">登入</NuxtLink>
        </li>
        <li class="navItem">
          <NuxtLink class="navLink" to="/register">註冊</NuxtLink>
        </li>
      </ul>
    </header>
    <slot />
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
