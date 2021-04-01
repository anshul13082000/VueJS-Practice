<template>
  <div id="app">
    <HelloWorld/>
    <ParentComponent/><br><br>
    <WatchExample/>
    <ParentComponent2/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import ParentComponent from './components/ParentComponent'
import WatchExample from './components/WatchExample'
import ParentComponent2 from './components/ParentComponent2'
export default {
  name: 'App',
  components: {
    HelloWorld,
    ParentComponent,
    WatchExample,
    ParentComponent2
  }
}
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
