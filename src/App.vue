<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>
<style lang="scss">
$accent-1: #D6CA47;
$accent-2: #F4F8F8;
$accent-3: #F4DC13;
$foreground: #FFFFFF;
$background: #2A2A33;
@import "~vue-material/dist/theme/engine"; 

@include md-register-theme("default", (
  primary: md-get-palette-color($foreground, A200),
  accent: md-get-palette-color($accent-1, A200), 
  theme: dark
));

@import "~vue-material/dist/theme/all"; 
#app {
position: absolute;
top: 0;
left: 0;
width: 100%;
height: 100%;
background: $background;
}
</style>

<style >

</style>
