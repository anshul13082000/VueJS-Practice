<template>
<div>
{{sendMessageToParent()}}
</div>
</template>

<script >
export default{
  name:'ChildComponent2',
  
  methods:{
    sendMessageToParent:function(){
      this.$emit('messageFromChild',10,20,30,40)
    }
  }
}

</script>

<style>
h1{
font-size:20px;
color: red;

}
</style>
