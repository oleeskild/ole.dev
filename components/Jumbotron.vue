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
    DevButton,
  },
};
</script>

<style scoped>
@keyframes hovering {
  0% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(10px);
  }
  to {
    transform: translateY(0);
  }
}
.container {
  width: 100%;
  height: 720px;
  min-height: 100vh;
  color: white;
  background-color: #4fa3e1;
}

.header {
  font-size: 128px;
  margin: 0;
}
.image {
  width: 50%;
  margin-top: 80px;
  animation-name: hovering;
  animation-duration: 6s;
  animation-iteration-count: infinite;
}
.logo {
  font-size: 64px;
  padding-left: 20px;
  margin: 0;
  padding-top: 20px;
}

#workstation {
  margin-left: -100px;
}
</style>
