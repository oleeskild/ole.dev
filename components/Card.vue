<template>
    <div class="card" :class="{'card--shadow': shadow}">
        <slot></slot>
    </div>
</template>
<script>
export default {
    props:['shadow']
}
</script>

<style scoped>
    .card{
        background-color: white;
        width: 100%;
        border-radius: 25px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .card--shadow {
        box-shadow: 10px 10px 5px 0px rgba(0,0,0,0.75);
    }
</style>

