<template lang="">
  <div class="container">
    <div class="row justify-content-md-center">
      <h2 class="col-md-4">유저 정보를 검색하세요</h2>
    </div>
    <div class="row justify-content-md-center">
      <textarea v-model="userId" class="col-md-6" name="name" rows="8" cols="10"></textarea>
      <button type="button" @click="$router.push({name: 'users-detail', params: {id: userId}})" name="button">버튼</button>
    </div>
    <div class="row justify-content-md-center">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: null
    }
  }
}
</script>

<style lang="css" scoped>
</style>
