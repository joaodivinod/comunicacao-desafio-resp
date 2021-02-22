<template>
	<div id="app">
    <div class="container">
      <userList></userList>
      <userDetails></userDetails>
    </div>
	</div>
</template>
<script>
import userDetails from "@/components/userDetails";
import userList from "@/components/userList";


export default {
  components:{
    userDetails,
    userList,
  },
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
</style>
