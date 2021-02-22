<template>
  <div class="list">
    <h1>Lista de usuarios</h1>

    <!--  topo da lista  -->
    <div class="top">
      <h2>ID</h2>
      <h2>Nome</h2>
      <h2>Idade</h2>
    </div>
    <!--  usuario  -->

    <div v-for="user in users" :key="user.id">
      <div class="user">
        <p>{{user.id}}</p>
        <p>{{user.name}}</p>
        <p>{{user.age}}</p>
      </div>
      <hr>
    </div>

  </div>
</template>

<script>
export default {
name: "userList",
  props: { users: Array },
}
</script>

<style scoped>
.user, .top{
  display: flex;
  justify-content: space-between;
  color: #fff;
  padding: 15px;
}
.user{

}
</style>