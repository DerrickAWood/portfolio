
<template>
  <div class="bColor my-Dark container-fluid">
    <div class="row">
      <div class="col-12 text-center">
      <div class="text-center my-auto text-white">
          <h1>Projects</h1>
          <hr class="white">
      </div>
      </div>
    </div>
    <div class="row text-center">
      <div class="col-4 d-flex justify-content-center">
            <div @click="localReach()" class="card hover" style="width: 18rem;">
            <img src="https://images.pexels.com/photos/1250452/pexels-photo-1250452.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940" class="card-img-top" alt="...">
            <div class="card-body">
              <h5 class="card-title">Local Reach</h5>
              <hr>
              <p class="card-text">localReach is designed to easily connect people with their community non profits. A fun and easy way to donate to your favorite charities.</p>
            </div>
          </div>
      </div>
      <div class="col-4 d-flex justify-content-center">
        <div class="card hover" style="width: 18rem;">
            <img src="" class="card-img-top" alt="...">
            <div class="card-body">
              <h5 class="card-title">Card title</h5>
              <hr>
              <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
            </div>
          </div>
      </div>
      <div class="col-4 d-flex justify-content-center">
        <div class="card hover" style="width: 18rem;">
            <img src="" class="card-img-top" alt="...">
            <div class="card-body">
              <h5 class="card-title"></h5>
              <hr>
              <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
            </div>
          </div>
      </div>
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
    }
  }
};
</script>

<style scoped>
.bColor{
  height: 60vh;
}

.my-Dark{
  background-color: #1e1e1e;
}

.hover:hover{
  transform: scale(1.1);
  cursor: pointer;
}
</style>