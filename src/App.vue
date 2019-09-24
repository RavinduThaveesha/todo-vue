<template>
  <div id="app">
      <Todos v-bind:todos="todos"/>
  </div>
</template>

<script>
import Todos from './components/Todos';

export default {
  name: 'app',
  components: {
    Todos
  },
  data() {
      return {
          todos: [
              {
                  id: 1,
                  text: "Bank Appointment",
                  isCompleted: true
              },
              {
                  id: 2,
                  text: "Team Meeting",
                  isCompleted: false
              },
              {
                  id: 3,
                  text: "Dinner with Amy",
                  isCompleted: false
              }
          ]
      }
  }
}
</script>

<style>
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: Arial, "Helvetica Neue", Helvetica, sans-serif;
    line-height: 1.4;
}
</style>
