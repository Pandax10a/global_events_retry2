<template>
    <div>
        <h1> this is specialUser</h1>
        <h1 ref="aname">a</h1>
        <article v-for="(name2, index) in names_two" :key="index">
        <h3> {{name2}}</h3>
        </article>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                names_two: [`abe`, `abc`, `abcd`]
            }
        },
       
        methods: {
            show_user(user) {
                this.names_two = user
                console.log(user)
            }
        },
        mounted () {
            this.$root.$on(`user_clicked`, this.show_user);
        },
        name: 'special-user'
    }
</script>

<style scoped>

</style>