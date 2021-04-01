<template>
  <div>
  <ChildComponent2 v-on:messageFromChild="childMessageReceived"></ChildComponent2>
  </div>
</template>

<script>
import ChildComponent2 from './ChildComponent2'
export default {
  name: 'ParentComponent2',

  components:{
    ChildComponent2
  },
  methods:{
    childMessageReceived(arg1,arg2,arg3,arg4){
      console.log("Arguments from child"+arg1+" "+arg2+" "+arg3+" "+arg4)
    }

  }
}
</script>


<style>

</style>
