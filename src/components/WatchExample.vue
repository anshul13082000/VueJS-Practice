<template>

<div id="demo">
  Kilometers <input type="text" v-model="kilometers">
  Meters <input type="text" v-model="meters">


</div>

</template>

<script >
export default{
  name:'WatchExample',
  data(){
    return{
      kilometers:0,
      meters:0
    }
  },
  watch:{
    kilometers:function(val){
      this.kilometers=val
      this.meters=val*1000
    },
    meters:function(val){
      this.kilometers=val/1000;
      this.meters=val
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