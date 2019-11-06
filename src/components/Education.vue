<script>
export default {
  props: ["education"]
};
</script>
<template>
  <section class="resume-section education-section mb-5">
    <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">{{ education.title }}</h2>
    <div class="resume-section-content">
      <ul class="list-unstyled">
        <li
          class="mb-2"
          v-for="qualification in education.qualifications"
          :key="qualification.school"
        >
          <div class="resume-degree font-weight-bold">{{ qualification.subject }}</div>
          <div class="resume-degree-org">{{ qualification.school }}</div>
          <div
            class="resume-degree-time"
            v-text="`${qualification.started} ${qualification.finished ? ' - '+qualification.finished : ''}`"
          ></div>
        </li>
      </ul>
    </div>
  </section>
</template>