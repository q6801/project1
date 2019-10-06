<template>
  <div class>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <a class="navbar-brand" href="#">Awesome</a>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link">
              <router-link :to="{ name: 'home'}">home</router-link>
            </a>
          </li>
          <li class="nav-item" >
            <a class="nav-link">
              <router-link :to="{ name: 'about', query: {hello:'world'}}">about</router-link>
            </a>
          </li>
          <li class="nav-item" >
            <a class="nav-link">
              <router-link
              :to="{ name: 'users', params: {id: '123', name: 'helloWOrld'}}">users</router-link>
            </a>
          </li>
        </ul>
      </div>
    </nav>
    <div class="container">
      <router-view></router-view>
    </div>
  </div>

</template>

<script>
export default {
}
</script>
