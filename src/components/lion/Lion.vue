<template>
    <div class="lion__inner">
        <h3>{{ lion_info.name }}</h3>
        <strong>{{ lion_info.last_name }}</strong>
        <br />
        <b>{{ lion_info.weight }}</b>
        <p>{{ lion_info.foods }}</p>
        <button>More info</button>
    </div>
</template>
<script setup>

const props = defineProps({
    lion_info: {
        type: Object
    }
})


</script>
<style scoped>
.lion__inner {
    width: 200px;
    padding: 20px 10px;
    border: 2px solid;
}
</style>