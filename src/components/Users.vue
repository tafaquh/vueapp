<template>
    <div class="users">
      <h1>Users</h1>
      <form v-on:submit="addUser">
        <input type="text" v-model="newUser.name" placeholder="Input name"> <br/>
        <input type="text" v-model="newUser.email" placeholder="Input email"><br/>
        <input type="submit" value="Submit">
      </form>
      <ul>
        <li v-for="user in users">
          {{user.name}}: {{user.email}}
        </li>
      </ul>
    </div>
</template>

<script>
export default {
  name: 'users',
  data () {
    return {
      newUser: {},
      users: [
        {
          name: 'Tafaquh Fiddin',
          email: 'tafaquh@pens.ac.id',
          contact: false
        },
        {
          name: 'Monkey D Luffy',
          email: 'luffy@pens.ac.id',
          contact: false
        },
        {
          name: 'Roronoa Zoro',
          email: 'zoro@pens.ac.id',
          contact: false
        }
      ]
    }
  },
  methods: {
    addUser: function () {
      console.log('add')
    }
  }
}
</script>

<style scoped>

</style>
