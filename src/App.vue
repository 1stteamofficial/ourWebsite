<template>
  <div id="#app" class="page-container">
    <md-app md-waterfall md-mode="flexible">
      <md-app-toolbar class="md-large md-primary">
        <div class="md-toolbar-row">
          <div class="md-toolbar-section-start">
            <md-button class="md-icon-button" @click="menuVisible = !menuVisible">
              <md-icon>menu</md-icon>
            </md-button>
          </div>
        </div>

        <div class="md-toolbar-row md-toolbar-offset">

          <span class="md-display-1">1stTeam <br> <div class="routename">
            {{ $route.name }}
          </div></span>
        </div>
      </md-app-toolbar>

      <md-app-drawer md-theme="default" :md-active.sync="menuVisible">
        <md-toolbar class="md-transparent" md-elevation="0"><b><h3>1stTeam</h3></b> </md-toolbar>

        <md-list>
          <md-list-item>
            <md-icon>home</md-icon>
            <a href="#/" class="md-list-item-text">Home</a>
          </md-list-item>
          <md-list-item>
            <md-icon>add</md-icon>
            <a href="#/joinus" class="md-list-item-text">Join Us</a>
          </md-list-item>

          <md-list-item>
            <md-icon>code</md-icon>
            <a href="http://github.com/1stteamofficial" class="md-list-item-text" >Github</a>
          </md-list-item>

          <md-list-item>
            <md-icon>list</md-icon>
            <span class="md-list-item-text">Team</span>
          </md-list-item>
        </md-list>
      </md-app-drawer>

      <md-app-content>
        <router-view/>
      </md-app-content>
    </md-app>
  </div>
</template>
<%= stylesheet_pack_tag 'hello_vue' %>
<style lang="scss" scoped>
  .md-app-toolbar {
    height: 196px;
  }
  #app, .md-app {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  }
  .routename{
    font-size: 14px;
    letter-spacing: 5px;
    text-align: center;
  }
</style>
<script>
export default {
  name: 'FirststTeamWebsite',
  data: () => ({
    menuVisible: false,
    github_username: "1stteamofficial",
    mail: "1st@marinenko.rf.gd"
  })
}
</script>
