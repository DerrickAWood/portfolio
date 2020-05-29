<template>
<div class="font">
      <div class="row no-gutters cover d-flex justify-content-center">
        <div class="col-md-6 align-self-center">
          <div class="text-center my-auto text-white mb-5">
            <h1>Derrick Wood</h1>
            <hr class="white">
            <h1>Software Developer</h1>
          </div>
        </div>
      </div>
    <div class="row text-center">

      
      <div class="col-md-4">
        <h2>Skills</h2>
        <div class="row justify-content-center">
        <i class="fab fa-html5 fa-4x m-1"></i>
        <i class="fab fa-css3-alt fa-4x m-1"></i>
        </div>
        <div class="row justify-content-center">
        <i class="fab fa-js fa-4x m-1"></i>
        <i class="fab fa-vuejs fa-4x m-1"></i>
        </div>
        <div class="row justify-content-center">
        <i class="fab fa-node-js fa-4x m-1"></i>
        <img src="https://img.icons8.com/ios-filled/50/000000/c-sharp-logo.png"/>
        </div>
        <i class="fab fa-github fa-4x m-1"></i>
      </div>
      


      <div class="col-md-4">
        <h1>About Me</h1>
        <img class="my-Pic m-2" src="../assets/me.jpg"/>
        
        <p class="subheading font-weight-regular m-3">
          A U.S. Army veteran & Full Stack Software Developer with a passion for solving problems and developing clean, modern software. Proficient with the most up to date software development tools and technologies. Proven leadership skills, hard working ethic, and a strong technical aptitude.
        </p>

        <h2 class="headline font-weight-bold mb-3">
          <button type="button" class="btn btn-secondary btn-lg hover" data-toggle="modal" data-target=".bd-example-modal-xl">View Resume</button>

        <div class="modal fade bd-example-modal-xl" tabindex="-1" role="dialog" aria-labelledby="myExtraLargeModalLabel" aria-hidden="true">
          <div class="modal-dialog modal-xl">
            <button type="button" class="close white hover" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
            <div class="modal-content">
              
               <img class="resume" src="../assets/resume.jpg"/>
      
              </div>
            </div>
          </div>
        </h2>
      </div>

      <div class="col-md-4">
        <h2>Connect</h2>
        <img @click="linkedIn()" class="hover" src="https://img.icons8.com/officel/50/000000/linkedin.png"/>
        <img @click="gitHub()" class="hover" src="https://img.icons8.com/nolan/64/github.png"/>
        <img @click="email()" class="hover" src="https://img.icons8.com/nolan/64/email.png"/>
        <img @click="cell()" class="hover" src="https://img.icons8.com/nolan/64/phone.png"/>
      </div>
     
    </div>
      <Projects></Projects>
</div>
</template>

<script>
import Projects from "../components/Projects.vue"
import swal from 'sweetalert'
  export default {
    name: 'HelloWorld',

    data: () => ({
      ecosystem: [
        {
          text: 'vuetify-loader',
          href: 'https://github.com/vuetifyjs/vuetify-loader',
        },
        {
          text: 'github',
          href: 'https://github.com/vuetifyjs/vuetify',
        },
        {
          text: 'awesome-vuetify',
          href: 'https://github.com/vuetifyjs/awesome-vuetify',
        },
      ],
      importantLinks: [
        {
          text: 'Documentation',
          href: 'https://vuetifyjs.com',
        },
        {
          text: 'Chat',
          href: 'https://community.vuetifyjs.com',
        },
        {
          text: 'Made with Vuetify',
          href: 'https://madewithvuejs.com/vuetify',
        },
        {
          text: 'Twitter',
          href: 'https://twitter.com/vuetifyjs',
        },
        {
          text: 'Articles',
          href: 'https://medium.com/vuetify',
        },
      ],
      whatsNext: [
        {
          text: 'Explore components',
          href: 'https://vuetifyjs.com/components/api-explorer',
        },
        {
          text: 'Select a layout',
          href: 'https://vuetifyjs.com/layout/pre-defined',
        },
        {
          text: 'Frequently Asked Questions',
          href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
        },
      ],
    }),
    methods:{
      linkedIn(){
        window.open("https://www.linkedin.com/in/derrickawood/")
      },
      gitHub(){
        window.open("https://github.com/DerrickAWood")
      },
      email(){
        swal("dwood_1994@yahoo.com");
      },
      cell(){
        swal("(661) 912-4085");
      }
    },
    components:{ Projects }
  }
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Ubuntu&display=swap');

.font {
  font-family: 'Ubuntu', sans-serif;
}

.bColor{
  height: 70vh;
}

.my-Dark{
  background-color: #1e1e1e;
}

.cover{
  background-image: url("https://images.unsplash.com/photo-1497032628192-86f99bcd76bc?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80");
  background-position: center;
  height: 70vh;
  background-size: cover;
}

.my-Pic{
  border-radius: 50%;
  height: 25vh;
}

.resume{
  height: 95vh;
}

.hover:hover{
  transform: scale(1.3);
  cursor: pointer;
}
</style>