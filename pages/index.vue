<template>
  <div>
    <div class="logo">
      <a href="https://github.com/oleeskild" target="_blank">
        <img src="https://seeklogo.com/images/G/github-logo-5F384D0265-seeklogo.com.png" height="30" 
        style="margin-right: 20px;">
    </a>
        <!-- <img src="https://nb.gravatar.com/avatar/1dfe1530479b8cc71d2420fd12150220" /> -->
    </div>
    <div class="background">
      <jumbotron>
        <div class="info">
          <h2 class="info__intro">Software Developer</h2>
          <h1 class="info__header">Ole Eskild Steensen</h1>
          <h3 class="info__subheader">email: post@ole.dev</h3>
        </div>
      </jumbotron>
    </div>
    <div>
      <project-list></project-list>
    </div>
  </div>
</template>
<script>
import Jumbotron from "../components/Jumbotron.vue";
import Card from "../components/Card.vue";
import ProjectList from "../components/ProjectList.vue"
export default {
  components: {
    Jumbotron,
    Card,
    ProjectList
  },
head () {
    return {
      title: "Ole Eskild Steensen",
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        { hid: '7245f665-1f2f-4d54-8346-5972f1283f82', name: 'description', content: 'Utvikler Ole Eskild Steensen' }
      ]
    }
  }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Varela&display=swap');
body {
    margin: 0;
    background-color: rgb(247, 252, 252)

}
.background {
  /* background-color: #4FA3E1; */
  height: 100%;
  width: 100vw;
}

.info {
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 10px;
}
.info__header {
  margin: 0;
  padding: 0;
  font-size: 56px;
}

.info__subheader {
  margin: 0;
  padding: 0;
  color: rgba(255, 255, 255, 0.8);
  font-size: 36px;
}

.info__intro {
  margin: 0;
  padding: 0;
  color: rgba(255, 255, 255, 0.8);
  font-size: 32px;
}

.center-content {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  height: 100%;
}
@media (max-width: 1024px) {
  .center-content{
    flex-direction: column-reverse;
  }
  
}

.logo {
    position: absolute;
    right: 0;
    margin-right: 20px;
    margin-top: 20px;
    display: flex;
    align-items: center;
    z-index: 1;
}

.logo >img{
    border-radius: 50%;
}

h1,
h2,
h3,
div {
  font-family: "Varela", sans-serif;
}
</style>
