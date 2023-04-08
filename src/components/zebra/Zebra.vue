<template>
    <div class="zebra__inner">
        <h3>{{ zebra_info.name }}</h3>
        <strong>{{ zebra_info.last_name }}</strong>
        <br />
        <b>{{ zebra_info.weight }}</b>
        <p>{{ zebra_info.foods }}</p>
        <button>More info</button>
    </div>
</template>
<script setup>

const props = defineProps({
    zebra_info: {
        type: Object
    }
})

</script>
<style scoped>
.zebra__inner {
    width: 200px;
    padding: 20px 10px;
    border: 2px solid;
}
</style>