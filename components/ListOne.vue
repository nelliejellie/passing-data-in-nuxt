<template>
    <section>
        <div class="title">
            <h3><img src="~assets/checklist-form-hi.png" alt="">List One</h3>
        </div>
        <div class="listcontainer">
            <li v-for="club in clubs" :key="club">{{ club }}</li>
        </div>
    </section>
</template>
<script>
export default {
    component: 'ListOne',
    computed:{
        clubs() {
            return this.$store.state.clubs
        }
    }, 
}
</script>
<style scoped>
    section{
        width: 99vw;
    }
    .title{
        display: flex;
        justify-content: center;
        width: 99vw;
    }
    h3{
        color: hotpink;
    }
    img{
        height: 5vh;
        width: 3vw;
    }
    .listcontainer{
        background-color: rgb(224, 162, 162);
        width: 40vw;
        height: 50vh;
        margin: 0 auto;
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        align-items: center;
    }
    li{
        list-style-type: none;
    }
</style>