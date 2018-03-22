<template>
  <section class="resume-section p-3 p-lg-5 d-flex flex-column" id="education">
        <div class="my-auto">
          <h2 class="mb-5">Education</h2>
           <edu v-for="(exp,index) in education" :edu="exp" :key="index"></edu>
        </div>  

    </section>
</template>

<script>
import Edu from './subcomponents/Edu.vue'

export default {
  name: 'education',
  props:['education'],
  components:{
      'edu': Edu
  }
}
</script>

