<template>
  <div>
    <div class="logo">
        <img src="https://nb.gravatar.com/avatar/1dfe1530479b8cc71d2420fd12150220" />
    </div>
    <div class="background">
      <jumbotron>
        <div class="info">
          <h1 class="info__header">Ole Eskild Steensen</h1>
          <h3 class="info__subheader">tlf: 92618997</h3>
          <h3 class="info__subheader">epost: post@ole.dev</h3>
        </div>
      </jumbotron>
    </div>
  </div>
</template>
<script>
import Jumbotron from "../components/Jumbotron.vue";
import Card from "../components/Card.vue";
export default {
  components: {
    Jumbotron,
    Card
  },
head () {
    return {
      title: "Ole Eskild Steensen",
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        { hid: '7245f665-1f2f-4d54-8346-5972f1283f82', name: 'description', content: 'My custom description' }
      ]
    }
  }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Varela&display=swap');
body {
    margin: 0;
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

.row {
  display: flex;
  flex-direction: row;
}

.row--align-center {
  align-items: center;
}

.row--full-height {
  height: 100%;
}

.logo {
    position: absolute;
    right: 0;
    margin-right: 20px;
    margin-top: 20px;
}

.logo >img{
    border-radius: 50%;
}

h1,
h2,
h3 {
  font-family: "Varela", sans-serif;
}
</style>
