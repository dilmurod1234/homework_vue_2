<template>
    <div class="section">
        <div>
            <div class="figure">
                <p>figure</p>
            </div>
            <div class="figcaption">
                <p>figcaption</p>
            </div>
        </div>
        <div>
            <div class="header">
                <p>header</p>
            </div>
            <div class="article">
                <h5>article</h5>
            </div>
            <div class="footer">
                <p>footer</p>
            </div>
        </div>
    </div>
</template>
<script setup>

</script>
<style scoped>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.section {
    display: flex;
    border: 2px solid gray;
}

.figure {
    padding: 18px 15px;
    text-align: center;
    background-color: greenyellow;
}

.figcaption {
    padding: 5px 0;
    background-color: #b2b2b2;
}

.header {
    width: 675px;
    padding: 1px 0;
    text-align: center;
    background-color: #f6d971;
}

.article {
    width: 675px;
    padding: 5px;
    text-align: center;
    background-color: #8cc3ff;
}

.footer {
    width: 675px;
    padding: 5px;
    text-align: center;
    background-color: #f6d971;
}
</style>