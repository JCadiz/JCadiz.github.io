<template>
  <div class="resume-item d-flex flex-column flex-md-row mb-5">
            <div class="resume-content mr-auto">
              <h3 class="mb-0">{{ edu.university }}</h3>
              <div class="subheading mb-3">{{ edu.grado }}</div>
              <div>{{ edu.titulo }}</div>
              <p>GPA: 3.23</p>
            </div>
            <div class="resume-date text-md-right">
              <span class="text-primary">{{ edu.fecha }}</span>
            </div>
          </div>
</template>

<script>
export default {
  name:'edu',
  props:['edu']
}
</script>

