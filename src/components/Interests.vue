<script>
export default {
  props: ["interests"]
};
</script>
<template>
  <section class="resume-section interests-section mb-5">
    <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">{{ interests.title }}</h2>
    <div class="resume-section-content">
      <ul class="list-unstyled">
        <li class="mb-1" v-for="item in interests.list" :key="item">{{ item }}</li>
      </ul>
    </div>
  </section>
</template>