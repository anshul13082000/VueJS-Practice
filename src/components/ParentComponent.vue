
<template>
  <div>
    <ChildComponent message="Static Message frmo Parent Component"/>
    <ChildComponent :message="msg"/>
    
  </div>
</template>

<script>
import ChildComponent from './ChildComponent'
export default {
  name: 'ParentComponent',
  data () {
    return {
      msg: 'Dynamic Message from parent Component'
    }
  },
  components:{
    ChildComponent
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

</style>


