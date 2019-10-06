<template>
  <div class="about">
    클릭
    <router-link :to="{ name: 'home', params: {} }">클릭</router-link>
    컴공이라면 hello {{ $route.query.hello }}
    {{ $route.query.world}}
  </div>
</template>
