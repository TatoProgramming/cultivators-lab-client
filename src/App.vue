<template>
  <v-app id="inspire" dark>
    <navigation-bar/>
    <v-content>
      <v-container fluid fill-height>
        <div>
          <v-btn color="primary" @click="addField">Add Field</v-btn>
        </div>
      </v-container>
    </v-content>
    <v-footer app fixed>
      <span>&copy; 2017</span>
    </v-footer>
  </v-app>
</template>

<script>
  import NavigationBar from './components/NavigationBar'
  export default {
    components: {
      NavigationBar
    },
    data: () => ({
      drawer: null
    }),
    methods:{
      addField(){
        alert("adding field")
      }
    }
  }
</script>
