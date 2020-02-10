<template>
<div class="container">
    <div class="row row--justify-start row--align-center row--full-height">
        <div class="image">
            <img id="workstation" src="~assets/Workstation.svg" />
        </div>
        <div style="justify-self: flex-start">
            <slot></slot>
        </div>

    </div>
</div>
</template>
<script>
import DevButton from "./DevButton.vue";
export default {
    components: {
        DevButton
    }
}
</script>

<style scoped>
    .container{
        width: 100%;
        height: 720px;
        min-height: 100vh;
        color: white;
        background-color: #4FA3E1;
    }
    
    .header {
        font-size: 128px;
        margin:0;
    }
    .image {
        width: 50%;
        margin-top: 80px;
    }
    .logo {
        font-size: 64px;
        padding-left: 20px;
        margin:0;
        padding-top:20px;
    }


    #workstation {
        margin-left: -100px;
    }
</style>
