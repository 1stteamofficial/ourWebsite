<template>
  <div class="hello">
    <md-card class="md-primary">
      <md-card-header>
        <md-card-header-text>
          <div class="md-title">Complete the form...</div>
          <div v-if="name == ''" class="md-subhead">Tell us about you.</div>
          <div v-else class="md-subhead">
            Welcome: {{ name }}
          </div>
        </md-card-header-text>

        <!-- md-card-media>
          <img src="https://avatars3.githubusercontent.com/u/44346564?s=200&v=4" alt="Avatar">
        </md-card-media -->
      </md-card-header>

            <md-card-content>
              <md-steppers md-vertical>
      <md-step id="first" md-label="First Step: About you">
    <md-field>
      <label>Your Name (or Nickname)</label>
      <md-input v-model="name"></md-input>
    </md-field>
    <md-field>
      <label>Your Mail</label>
      <md-input type="email" v-model="email"></md-input>
    </md-field>
    <md-field>
      <label>Age</label>
      <md-input type="number" v-model="age"></md-input>
    </md-field>
      </md-step>

      <md-step id="second" md-label="Second Step: Your Skills">
        <md-field>
          <label>Profession and(or) skills</label>
          <md-textarea v-model="skills"></md-textarea>
        </md-field>
      </md-step>

      <md-step id="third" md-label="Third Step: Complete The form" md-description="Check the data you entered and submit">
        <p>
          <b>Name:</b> {{name}} <br>
          <b>E-Mail:</b> {{email}} <br>
          <b>Age</b>: {{age}} <br>
          <b>Skills:</b> <br>
          <pre>{{skills}}</pre>
          <br>
          <md-button :href="'#/'" class="md-primary">Submit</md-button>
        </p>
      </md-step>
    </md-steppers>
  </md-card-content>
    </md-card>
  </div>
</template>

<script>
export default {
  name: 'JoinUs',
  data () {
    return {
      msg: 'Welcome to 1stTEAM Platform!',
      name: "",
      email: "",
      age: "",
      skills: ""
    }
  }
}
</script>

<style scoped>

</style>
