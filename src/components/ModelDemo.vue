<template>
    <h3>表单输入绑定</h3>
    <form>

        <!-- <input type="text" v-model="message"> -->
        <input type="text" v-model.lazy="message">
        <p>{{ message }}</p>
    </form>
</template>

<script>

export default {

    data() {
        return {
            message: ""
        }
    }
}
</script>