<script>
    import CcUsers from './components/users/main.vue'

    export default {        
        components: {
            CcUsers
        },

        computed: {
            user () {
                const { name, email } = this.$store.state.user

                return `O Usuario ${name} tem o email ${email}`
            }
        }
    }
</script>

<template>
    <div>
        <h1>Funfando !</h1>
        <h4>{{ user }}</h4>
        <hr>
        <cc-users></cc-users>
    </div>
</template>
