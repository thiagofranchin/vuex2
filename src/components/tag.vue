<script>
    export default {        
        computed: {
            mytag () {
                const { url, time } = this.$store.state.user
                 return `${url}  ===> ${time}`
            }            
        }
    }
</script>
<template>
    <div>
        {{mytag}}
    </div>
</template>
