<template>
    <div class="header">
        <h4 class="header__text"> {{ open }} Header {{ close }}</h4>
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
    .header{
       padding: 10px 20px; 
       background-color: yellow; 
    }
    .header__text{
        text-align: center;
    }
</style>