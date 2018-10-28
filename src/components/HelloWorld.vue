<template>
  <div class="hello">
    <md-card class="md-primary">
      <md-card-header>
        <md-card-header-text>
          <div class="md-title">Join to 1stTeam Members!</div>
          <div class="md-subhead">Join Us!</div>
        </md-card-header-text>

        <!-- md-card-media>
          <img src="https://avatars3.githubusercontent.com/u/44346564?s=200&v=4" alt="Avatar">
        </md-card-media -->
      </md-card-header>
      <md-card-expand>
          <md-card-actions md-alignment="space-between">
            <div>
              <md-button>Github</md-button>
              <md-button>Mail Us</md-button>
            </div>

            <md-card-expand-trigger>
              <md-button class="md-icon-button">
                <md-icon>keyboard_arrow_down</md-icon>
              </md-button>
            </md-card-expand-trigger>
          </md-card-actions>

          <md-card-expand-content>
            <md-card-content>
              <b>1stTeam</b> 🏢  – The greatest <b>Freelance Team 🏡</b> of Designers, Developers, Specialists of Cyber Security, Web Developers, Web Designer, SysAdmin and <u>even more</u>...
            </md-card-content>
          </md-card-expand-content>
        </md-card-expand>
    </md-card>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to 1stTEAM Platform!'
    }
  }
}
</script>

<style scoped>

</style>
