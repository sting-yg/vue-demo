<template>
    <h3>事件修饰符</h3>
    <a @click.prevent="clickHandle" href="https://itbaizhan.com">百战程序员</a>
    <div @click="clickDiv">
        <p @click.stop="clickP">测试冒泡</p>
    </div>
</template>

<script>

export default{
    data(){
        return{

        }
    },
    methods:{
        clickHandle(e){
            //阻止默认事件
            //e.preventDefault();
            console.log("点击了");
        },
        clickDiv(){
            console.log("点击了 DIV");
        },
        clickP(e){
            //e.stopPropogation()
            console.log("点击了 P");
        }
    }
}
</script>