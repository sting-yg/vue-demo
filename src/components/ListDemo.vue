<template>
    <h3>列表渲染</h3>
    <p v-for="item in names">{{ item }}</p>
    <div v-for="item in result">
        <p>{{ item.title }}</p>        
    </div>

    <div>
        <p v-for="(value,key,index) of userInfo">{{ value }}-{{ key }}-{{ index }}</p>
    </div>
</template>

<script>

export default{
    data(){
        return{
            names:["百战程序员","尚学堂","IT"],
            result:[
                    {"id":"id1","title":"title1","avator":"avator1"},
                    {"id":"id2","title":"title2","avator":"avator2"},
                    {"id":"id3","title":"title3","avator":"avator3"}              
                    ]
        }
    }
}

</script>