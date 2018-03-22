<template>
   <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="awards">
        <div class="my-auto">
          <h2 class="mb-5">Awards &amp; Certifications</h2>
          <ul class="fa-ul mb-0">
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
              {{ awards.google }}</li>
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
                {{ awards.mobile }} </li>
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
              1<sup>st</sup>
              {{ awards.place }}</li>
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
              1<sup>st</sup>
              {{ awards.category }}</li>
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
              2<sup>nd</sup>
              {{ awards.competin }}</li>
            <li>
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
              1<sup>st</sup>
              {{ awards.h }}</li>
            <li>
              <i class="fa-li fa fa-trophy text-warning"></i>
              3<sup>rd</sup>
              {{ awards.l }}</li>
          </ul>
        </div>
      </section>
</template>
<script>

export default {
   name: 'awards',
  props:['awards']
}
</script>
