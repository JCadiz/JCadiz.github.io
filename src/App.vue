<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary fixed-top" id="sideNav">
      <a class="navbar-brand js-scroll-trigger" href="#page-top">
        <span class="d-block d-lg-none">Start Bootstrap</span>
        <span class="d-none d-lg-block">
          <img class="img-fluid img-profile rounded-circle mx-auto mb-2" src="./assets/img/foto.jpg">
        </span>
      </a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#about">About</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#experience">Experience</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#education">Education</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#skills">Skills</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#interests">Interests</a>
          </li>
          <li class="nav-item">
            <a class="nav-link js-scroll-trigger" href="#awards">Awards</a>
          </li>
        </ul>
      </div>
    </nav>

    <div class="container-fluid p-0">

      <about :about="misdatos"></about>
      
      <experiences :experiences="experiences"></experiences>

      <education :education="education"></education>

      <habilidades :habilidades="mishabilidades"></habilidades>

      <gustos :gustos="contenido"></gustos>
      
      <awards :awards="certificados"></awards>
      <!-- <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="awards">
        <div class="my-auto">
          <h2 class="mb-5">Awards &amp; Certifications</h2>
          <ul class="fa-ul mb-0">
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
              Google Analytics Certified Developer</li>
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
              Mobile Web Specialist - Google Certification</li>
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
              1<sup>st</sup>
              Place - University of Colorado Boulder - Emerging Tech Competition 2009</li>
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
              1<sup>st</sup>
              Place - University of Colorado Boulder - Adobe Creative Jam 2008 (UI Design Category)</li>
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
              2<sup>nd</sup>
              Place - University of Colorado Boulder - Emerging Tech Competition 2008</li>
            <li>
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
              1<sup>st</sup>
              Place - James Buchanan High School - Hackathon 2006</li>
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
              3<sup>rd</sup>
              Place - James Buchanan High School - Hackathon 2005</li>
          </ul>
        </div>
      </section> -->

    </div>
  </div>
</template>

<script>
import About from './components/About.vue'
import Experiences from './components/Experiences.vue'
import Education from './components/Education.vue'
import Habilidades from './components/Habilidades.vue'
import Gustos from './components/Gustos.vue'
import Awards from './components/Awards.vue'
import axios from 'axios'

export default {
  name: 'app',
  mounted(){
    console.log('componente cargado....')
    this.prueba();
  },
  components:{
    'about': About,
    'experiences': Experiences,
    'education': Education,
    'habilidades': Habilidades,
    'gustos': Gustos,
    'awards': Awards
  },
  data(){
    return{
      misdatos: {
        name: 'Jesus I.',
        lastname: 'Cadiz B.',
        address:'Ud-4 conjunto Canagua Bloq 2 piso 7 apart 0703, Caricuao - Caracas',
        email:'jesuscadiz22@gmail.com',
        phone:'+58(0414)389-13-51',
        description:'I am experienced in leveraging agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches to corporate strategy foster collaborative thinking to further the overall value proposition.',
        facebook:'https://www.facebook.com/jesuscadizb',
        instagram:'https://www.instagram.com/jesuscad95/',
        linkedin:'https://www.linkedin.com/in/jesus-cadiz-b169a811b/',
        github:'https://github.com/JCadiz'
      },

      experiences:[
        {job:'SENIOR WEB DEVELOPER',
         company:'INTELITEC SOLUTIONS',
         description:'Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation X is on the runway heading towards a streamlined cloud solution. User generated content in real-time will have multiple touchpoints for offshoring.',
         date:'March 2013 - Present'},

         {job:'SENIOR WEB DEVELOPER',
         company:'INTELITEC SOLUTIONS',
         description:'Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation X is on the runway heading towards a streamlined cloud solution. User generated content in real-time will have multiple touchpoints for offshoring.',
         date:'March 2013 - Present'},

         {job:'SENIOR WEB DEVELOPER',
         company:'INTELITEC SOLUTIONS',
         description:'Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation X is on the runway heading towards a streamlined cloud solution. User generated content in real-time will have multiple touchpoints for offshoring.',
         date:'March 2013 - Present'},

         {job:'SENIOR WEB DEVELOPER',
         company:'INTELITEC SOLUTIONS',
         description:'Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation X is on the runway heading towards a streamlined cloud solution. User generated content in real-time will have multiple touchpoints for offshoring.',
         date:'March 2013 - Present'},
        
      ],
      education:[
        {university:'University of Colorado Boulder',
         grado:'Bachelor of Science',
         titulo:'Computer Science - Web Development Track',
         fecha:'August 2006 - May 2010'},
      ],
      mishabilidades:{
        mobile:'Mobile-First, Responsive Design',
        testing:'Cross Browser Testing',
        debug: 'Debugging',
        cross:'Cross Functional Teams',
        agil:'Agile Development',
        scrum:'Scrum'
      },
      contenido:{
        1:'Apart from being a web developer, I enjoy most of my time being outdoors. In the winter, I am an avid skiier and novice ice climber. During the warmer months here in Colorado, I enjoy mountain biking, free climbing, and kayaking.',
        2:'When forced indoors, I follow a number of sci-fi and fantasy genre movies and television shows, I am an aspiring chef, and I spend a large amount of my free time exploring the latest technolgy advancements in the front-end web development world.'
      },
      certificados:{
        google:'Google Analytics Certified Developer',
        mobile:'Mobile Web Specialist - Google Certification',
        place:' Place - University of Colorado Boulder - Emerging Tech Competition 2009',
        category:'Place - University of Colorado Boulder - Adobe Creative Jam 2008 (UI Design Category)',
        competin:'Place - University of Colorado Boulder - Emerging Tech Competition 2008',
        h:'Place - James Buchanan High School - Hackathon 2006',
        l:'Place - James Buchanan High School - Hackathon 2005'
    }
  } 
  },
  methods:{
    prueba(){
      axios.get('https://swapi.co/api/people').then(response =>{
      console.log(response.data)
    }).catch(error => {
      console.log(error)
    });
    }
  }
}
</script>

<style>

</style>
