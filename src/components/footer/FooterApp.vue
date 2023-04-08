<template>
    <div class="footer">
        <h4> {{ open }} Footer {{ close }} </h4>
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
.footer {
    width: 100%;
    margin-bottom: 100px;
    padding: 10px 0;
    background-color: #f6c364;
    text-align: center;
}
</style>