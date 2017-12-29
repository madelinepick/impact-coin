<template>
  <div id="app">
    <ToDoList v-bind:todos="todos"/>
  </div>
</template>

<script>
import ToDoList from './components/ToDoList';

export default {
  name: 'app',
  components: {
    ToDoList,
  },
  data() {
    return {
      todos: [{
        title: 'Project Fi',
        project: 'Communication',
        done: false,
      }, {
        title: 'Clean Bike',
        project: 'Sports',
        done: true,
      }, {
        title: 'Run',
        project: 'Sports',
        done: false,
      }, {
        title: 'Paint',
        project: 'House',
        done: false,
      }],
    };
  },
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
