<template>
    <div class="gorilla__inner">
        <h3>{{ gorilla_info.name }}</h3>
        <strong>{{ gorilla_info.last_name }}</strong>
        <br />
        <b>{{ gorilla_info.weight }}</b>
        <p>{{ gorilla_info.foods }}</p>
        <button>More info</button>
    </div>
</template>
<script setup>

const props = defineProps({
    gorilla_info: {
        type: Object
    }
})

</script>
<style>
.gorilla__inner {
    width: 200px;
    padding: 20px 10px;
    border: 2px solid;
}
</style>