<template>
  <div class="hello">
      <div>
    <div class="phone-viewport">
      <md-bottom-bar md-type="shift" :md-theme="'bottom-bar-' + theme">
        <md-bottom-bar-item md-label="Home" md-icon="home" @click="theme = 'teal'"></md-bottom-bar-item>
        <md-bottom-bar-item md-label="Pages" md-icon="pages" @click="theme = 'orange'"></md-bottom-bar-item>
        <md-bottom-bar-item md-label="Posts" md-icon="/assets/icon-whatshot.svg" @click="theme = 'blue'"></md-bottom-bar-item>
        <md-bottom-bar-item md-label="Favorites" md-icon="favorite" @click="theme = 'red'"></md-bottom-bar-item>
      </md-bottom-bar>
    </div>
  </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>
<script>
export default {
  name: 'ChangingThemes',
  data: () => ({
    theme: 'teal'
  })
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
