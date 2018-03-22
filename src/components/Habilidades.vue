<template>
  <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="skills">
        <div class="my-auto">
          <h2 class="mb-5">Habilidades</h2>

          <div class="subheading mb-3">Lenguajes de Programacion &amp; Herramientas</div>
          <ul class="list-inline list-icons">
            <li class="list-inline-item">
              <i class="devicons devicons-html5"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicons devicons-css3"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicons devicons-javascript"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicons devicons-jquery"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicons devicons-react"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicons devicons-nodejs"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicons devicons-bootstrap"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicons devicons-java"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicons devicons-vue.js"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicons devicons-c#"></i>
            </li>
            <li class="list-inline-item">
              <i class="devicons devicons-npm"></i>
            </li>
          </ul>

          <div class="subheading mb-3">Forma de Trabajo</div>
          <ul class="fa-ul mb-0">
            <li>
              <i class="fa-li fa fa-check"></i>
             {{ habilidades.mobile }}</li>
            <li>
              <i class="fa-li fa fa-check"></i>
               {{ habilidades.testing }} &amp;  {{ habilidades.debug }}</li>
            <li>
              <i class="fa-li fa fa-check"></i>
              {{ habilidades.cross }}</li>
            <li>
              <i class="fa-li fa fa-check"></i>
              {{ habilidades.agil }} &amp;  {{ habilidades.scrum }}</li>
          </ul>
        </div>
      </section>
</template>

<script>
export default {
  name: 'habilidades',
  props:['habilidades']
}
</script>

