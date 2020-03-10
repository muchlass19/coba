<template>
    <div>
        <NavBar></NavBar>
        <button @click="toggle">klik</button>
        <h1 v-if="show">Post</h1>
    </div>
</template>

<script>
import NavBar from '~/components/navbar.vue';
export default {
    data(){
        return{
            show: true,
        }
    },
    
    components:{
        NavBar,
    },


    methods:{
        toggle(){
            this.show = !this.show
        }
    }
}
</script>