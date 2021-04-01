<template>
<div>
<h1>message is {{message}}</h1>
</div>
</template>

<script >
export default{
  name:'ChildComponent',
  
  props:{
    message:String
  },
  methods:{
      callMe(){
          alert('Call me is called')
      }
  },
  watch:{
    'message':function(){
        this.callMe()
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


