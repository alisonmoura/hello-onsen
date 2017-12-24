<template>
  <v-ons-page>
    <v-ons-toolbar style="background-color: blue;">
      <div class="left">
        <v-ons-toolbar-button @click="$store.commit('splitter/toggle')">
          <v-ons-icon icon="ion-navicon, material:md-menu"></v-ons-icon>
        </v-ons-toolbar-button>
      </div>
      <div class="center white-text">{{ title }}</div>
    </v-ons-toolbar>

    <div class="background"></div>

    <div class="content"></div>

  </v-ons-page>
</template>

<script>
export default {
  name: 'home',
  data () {
    return {
      title: 'Home'
    }
  },
  methods: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.header {
  text-align: center;
}

.white-text{
  color: white;
}

img {
  max-width: 300px;
}

.background{
  background-color: white;
}

ons-icon{
  color: white;
}

ons-list-title {
  text-transform: none;
}

ons-list-title:not(:first-of-type) {
  margin-top: 30px;
}

ons-card {
  text-align: center;
}

ons-list-item, ons-card {
  cursor: pointer;
}
</style>
