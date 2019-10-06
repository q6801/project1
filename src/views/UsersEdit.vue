<template lang="html">
  <div class="">
    <h1>hello</h1>
    {{$route.params.id}}
  </div>

</template>

<script>
export default {
  data: function() {
    return {
      userId: this.$route.params.id
    }
  }
}
</script>

<style lang="css" scoped>
</style>
