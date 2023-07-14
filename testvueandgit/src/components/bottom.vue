<template>
    <div class="bottom" >boxbottom</div>
    <button @click="btnclick" class="btn">btn</button>
    <div>{{ bottomdata.text}}</div>
    <p :class="{ active: isActive }" >Hi!</p>
</template>


<script > 
   export default{
     name: 'bottom',
     data() {
      return {
        isActive: true,
        bottomdata:{
            text: 1
        }
      }   
     },
     methods: {
      btnclick(func){
        this.bottomdata.text++;
        this.isActive = !this.isActive;
        if(func){
          console.log(func);
        }
       
      }
     }

  


   }
</script>

<style scoped>
  .bottom{
    height: 100px;
    width: 100px;
    background-color: aqua;
  }

  .btn{
    height: 30px;
    width: 30px;
    
  }

  .active{
    font-size: 20px;
    color: red;
  }
</style>
