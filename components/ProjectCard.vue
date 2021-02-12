<template>
    <a :href="url" class="project-card">
        <div class="project-icon">
            <span v-html="icon"></span>
        </div>
        <div class="title">
            <div class="prepend">ole.dev/</div>
            <h2 class="name">{{title}}</h2>
        </div>
    </a>
</template>
<script>
export default {
    props: [
        'url',
        'title',
        'icon'
    ]
}
</script>
<style scoped>
.project-card {
    padding: 10px;
    margin: 10px;
    background-color: #fff;
    border-radius: 25px;
    box-shadow: rgba(14, 30, 37, 0.12) 0px 2px 4px 0px;
    text-decoration: none;
}
.project-icon {
    height: 150px;
    font-size: 120px;
    text-align: center;
 }
.title{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: #c3490d;
}
.prepend {
     color: #3d78a1d1;
    font-size: 15px;
    padding-top: 10px;
}
.name {
    text-align: center;
    border-bottom: 3px solid #ffd147;
    padding-bottom: 3px;
    width: fit-content;
    margin-top:0;
    padding-top:0;
}
.name:hover{
    color: #3d78a1;
    border-color: #3d78a1;
}
</style>