<template>
  <div >
    <h1>this is userlist</h1>
    <section v-for="(user, index) in users" :key="index">
        <h2 @click="highlight_username(index)">this is: {{user}}</h2>
    
    
    </section>
<h3>this is component</h3>
  </div>
  
</template>

<script>
    export default {
       
        methods: {
            highlight_username(index) {
                index
                this.$root.$emit(`user_clicked`, this.users[index])
                
            }
        },
        data() {
            return {
                users: [`userOne`, `userTwo`, `userThree`]
            }
        },
        name: 'user-lists'
    }
</script>

<style scoped>

</style>