<template>
<div>
      <div class="row no-gutters my-Dark">
        <div class="col-6 offset-3">
          <div class="text-center bColor my-auto text-white">
            <h1>Derrick Wood</h1>
            <hr class="white">
            <h1>Software Developer</h1>
          </div>
        </div>
      </div>
    <div class="row text-center">


      <div class="col-4">
        <h2>Skills</h2>
        <i class="fab fa-html5 fa-4x m-1"></i>
        <i class="fab fa-css3-alt fa-4x m-1"></i>
        <i class="fab fa-js fa-4x m-1"></i>
        <i class="fab fa-vuejs fa-4x m-1"></i>
        <i class="fab fa-node-js fa-4x m-1"></i>
        <img src="https://img.icons8.com/ios-filled/50/000000/c-sharp-logo.png"/>
        <i class="fab fa-github fa-4x m-1"></i>
      </div>


      <div class="col-4">
        <h1>About Me</h1>
        <img class="my-Pic m-2" src="https://media-exp1.licdn.com/dms/image/C5603AQEAL1BjiwdP5w/profile-displayphoto-shrink_200_200/0?e=1594857600&v=beta&t=RmSFPjHn2IEmUO1-2Cdev19tSUD5yuYm-Ygv854AW5A">
        
        <p class="subheading font-weight-regular m-3">
          A U.S. Army veteran & Full Stack Software Developer with a passion for solving problems and developing clean, modern software. Proficient with the most up to date software development tools and technologies. Proven leadership skills, hard working ethic, and a strong technical aptitude.
        </p>

        <h2 class="headline font-weight-bold mb-3">
          Important Links
        </h2>

        <v-row justify="center">
          <a
            v-for="(link, i) in importantLinks"
            :key="i"
            :href="link.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ link.text }}
          </a>
        </v-row>
      </div>

      <div class="col-4">
        <h2>Connect</h2>
      </div>
     
    </div>
</div>
</template>

<script>
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
  }
</script>

<style scoped>
.bColor{
  height: 70vh;
}

.my-Dark{
  background-color: #1e1e1e;
}

.my-Pic{
  border-radius: 50%;
}
</style>