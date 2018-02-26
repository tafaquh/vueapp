<template>
    <div class="test">
        <h1>{{title}}</h1>
        <p>{{user.firstName}}</p>
    </div
</template>

<script>
    export default{
        name: 'test',
        data() {
            return{
                title: 'Hello Tafaquh',
                use: {
                    firstName: 'Tafaquh',
                    lastName: 'Fiddin'
                }
            }
        }
    }
</script>

<style scoped>

</style>