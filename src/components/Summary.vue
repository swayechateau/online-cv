<script>
export default {
  props: ["summary"]
};
</script>
<template>
  <section class="resume-section summary-section mb-5">
    <h2
      class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3"
      v-text="summary.title"
    />
    <div class="resume-section-content">
      <p class="mb-0" v-text="summary.text" />
    </div>
  </section>
</template>