<template>
    <div class="top" id="topbox">box{{ topdata.username }}</div>
</template>


<script>
export default {
    name: 'top',
    data() {
      return {
        topdata:{
            username: 'huzhihong',
            password: 123
        }
    }
    }
      
}
</script>

<style scoped>
  #topbox{
    color: azure;
    height: 10vw;
    widows: 10vw;
    background-color:black;
  }
</style>