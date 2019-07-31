<template>
  <div id="app">
      <div class="container">
          <img class="logo" alt="Vue logo" src="./assets/logo.png" />

          <AddTodo />
          <FilterTodos />
          <Todos />
      </div>
  </div>
</template>

<script>
    import AddTodo from './components/AddTodo'
    import Todos from './components/Todos'
    import FilterTodos from './components/FilterTodos'

    export default {
        name: 'app',
        components: {
            AddTodo,
            Todos,
            FilterTodos
        }
    }
</script>

<style>
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        color: #2c3e50;
        margin-top: 30px;
    }

    .container {
        max-width: 1100px;
        margin: auto;
        overflow: auto;
        padding: 0 2rem;
    }

    .logo {
        max-width: 30px;
        display: block;
        margin-left: auto;
        margin-right: auto 
    }
</style>
