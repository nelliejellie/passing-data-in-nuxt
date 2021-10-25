<template lang="">
    <div>
        <ListOne />
    </div>
</template>
<script>

export default {
    computed:{
        clubs() {
            return this.$store.state.clubs
        }
    },
    created() {
        console.log(this.clubs)
    }
}
</script>
<style lang="">
    
</style>