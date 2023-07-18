<template>
    <h3>事件参数</h3>
    <p @click="getNameHandler(item)" v-for="(item, index) of names" :key="index">{{ item }}</p>   
</template>

<script>

    export default {
        data(){
            return {
                names:["iwen","ime","frank"]
            }
        },
        methods:{
            
            getNameHandler(name){
                console.log(name);
            }
        }
    }
    
</script>