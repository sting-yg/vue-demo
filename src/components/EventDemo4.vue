<template>
    <h3>内联事件处理器</h3>
    <button @click="addCount('abcd')">Add</button>
    <p>{{ count }}</p>
</template>

<script>

    export default {
        data(){
            return {
                count: 0
            }
        },
        methods:{
            // event 对象
            addCount(e){
                console.log(msg);
                this.count++
            }
        }
    }
</script>