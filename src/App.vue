<template>
	<div id="app">
    <div class="container">
      <userList :users="users" />
      <userDetails/>
    </div>
	</div>
</template>
<script>

import userDetails from "@/components/userDetails";
import userList from "@/components/userList";


export default {
  name: "app",
  data(){
    return{
      users:[
        { id: 1, name:'João Divino', age:24},
        { id: 2, name:'Ana Luiza', age:20},
        { id: 3, name:'Daniel Vitor', age:23},
        { id: 4, name: 'Ana', age: 31 },
        { id: 5, name: 'Carlos', age: 22 },
        { id: 6, name: 'Daniel', age: 40 },
        { id: 7, name: 'Ema', age: 17 },
        { id: 8, name: 'Lia', age: 28 }
      ]
    }
  },
  components:{userDetails, userList,},
  props:{

  }
}


</script>

<style>
body{
  background-color: #1b1b2f;
  font-family: 'Montserrat', sans-serif;
}
.container{
  width: 1500px;
  max-width: 90%;
  margin: auto;
  display: flex;
}
h1{
  text-align: center;
  color: #e43f5a;
}
.details, .list{
  width: 50%;
}
p{
  color: #fff;
}
</style>
