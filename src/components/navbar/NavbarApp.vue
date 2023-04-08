<template>
    <div class="nav">
        <h4 class="nav__text">{{ open }} Nav {{ close }}</h4>
    </div>
</template>
<script setup>
const props = defineProps({
    open: {
        type: String
    },
    close: {
        type: String
    }
})
</script>
<style scoped>
    *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
.nav{
    width: 110px;
    height: 312px;
    background-color: #fc7a7a;
    position: relative;
}
.nav > h4{
    transform: rotate(270deg);
    position: absolute;
    top: 120px;
    right: 1px;
}
</style>