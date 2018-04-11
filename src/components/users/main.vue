<script>
    import CcTag from '../tag.vue'
    export default {
        components: {
            CcTag
        },

        computed: {
            email () {
                return this.$store.state.user.email
            }
        }
    }

</script>

<template>
    <div>
        Email: {{ email }}
        <hr />  
        <cc-tag></cc-tag>
    </div>
</template>
