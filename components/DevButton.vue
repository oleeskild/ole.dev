<template>
<transition name="fade">
   <button class="button" :class="'button' + stroked?'button--stroked' :''">{{text}}</button>
</transition>
</template>
<script>
export default {
   props: ['text', 'stroked'] 
}
</script>

<style lang="css" scoped>
   .button{
      border: #FFA87C 5px solid;
      background-color:#FFA87C;
      width: 100%;
      font-size: 48px;
      color: white;
      border-radius: 20px;
      padding: 10px 50px;
      cursor: pointer;
   }
   .button--stroked {
      background-color: rgba(0,0,0,0);
   }

   .button--stroked:hover {
      background-color:#FFA87C;
   }

   .button,.fade-enter-active, .fade-leave-active {
      transition: background-color .3s;
   }
</style>
