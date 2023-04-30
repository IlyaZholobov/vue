<template>
  <div class="app">
    <MyComponent />
    <HomeTask />
  </div>
</template>

<script>
import MyComponent from './components/Mycomponent.vue'
import HomeTask from './components/HomeTask.vue'

export default {
  name: 'App',
  components: {
    MyComponent,
    HomeTask
  }
}
</script>


