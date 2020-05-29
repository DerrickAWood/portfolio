
<template>
  <div id="projects" class="bColor my-Dark container-fluid font">
    <div class="row">
      <div class="col-12 text-center">
      <div class="text-center my-auto text-white">
          <h1>Projects</h1>
          <hr class="white">
      </div>
      </div>
    </div>
    <div class="row text-center">
      <div class="col-md-6 d-flex justify-content-center">
            <div @click="localReach()" class="card hover" style="width: 18rem;">
            <img src="https://images.pexels.com/photos/1250452/pexels-photo-1250452.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940" class="card-img-top" alt="...">
            <div class="card-body">
              <h5 class="card-title">Local Reach</h5>
              <hr>
              <p class="card-text">localReach is designed to easily connect people with their community non profits. A fun and easy way to donate to your favorite charities.</p>
            </div>
          </div>
      </div>
      <div class="col-md-6 d-flex justify-content-center">
        <div @click="bugLogger()" class="card hover" style="width: 18rem;">
            <img src="https://www.stockvault.net/data/2016/10/25/214456/preview16.jpg" class="card-img-top" alt="...">
            <div class="card-body">
              <h5 class="card-title">Bug Logger</h5>
              <hr>
              <p class="card-text">Bug Logger is designed to help you report and track bugs on an application. </p>
            </div>
          </div>
      </div>
     

     <!-- more projects here -->


    </div>
  </div>
</template>

<script>
export default {
  name: "projects",
  data() {
    return {};
  },
  methods: {
    localReach(){
      window.open("https://localreach.herokuapp.com/#/")
    },
    bugLogger(){
      window.open("https://debug-logger.herokuapp.com/#/")
    }
  }
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Ubuntu&display=swap');

.font {
  font-family: 'Ubuntu', sans-serif;
}

.bColor{
  /* height: 100vh; */
}

.my-Dark{
  background-color: #1e1e1e;
}

.hover:hover{
  transform: scale(1.1);
  cursor: pointer;
}
</style>