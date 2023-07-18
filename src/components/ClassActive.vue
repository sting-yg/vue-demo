<template>
    <p :class="{ 'active': isActive }">Class 样式绑定</p>
</template>

<script>

export default {
    data() {
        return {
            isActive: true
        }
    }
}

</script>

<style>
.active {
    color: red;
    font-size: 30px;
}
</style>