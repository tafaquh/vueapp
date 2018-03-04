<template>
    <div class="users">
        
    </div>
</template>

<script>
export default {
  name: 'user',
  props: {
    msg: {
      type: String,
      default: 'Foobar'
    }
  },
  data () {
    return {
      title: 'Hello Tafaquh',
      user: {
        firstName: 'Tafaquh',
        lastName: 'Fiddin'
      },
      showName: true,
      items: [
        {title: 'Item One'},
        {title: 'Item Two'},
        {title: 'Item Three'}
      ]
    }
  },
  methods: {
    greet: function (greeting) {
      alert(greeting)
    },
    pressKey: function (e) {
      console.log(e.target.value)
    },
    enterHit: function () {
      console.log('You hit enter')
    }
  },
  computed: {
    fullName: function () {
      return this.user.firstName + ' ' + this.user.lastName
    }
  }
}
</script>

<style scoped>

</style>
