<script>
export default {};
</script>
<template>
  <section class="resume-section language-section mb-5">
    <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">{{ languages.title }}</h2>
    <div class="resume-section-content">
      <ul class="list-unstyled resume-lang-list">
        <li class="mb-2" v-for="lang in languages.list" :key="lang.name">
          <span class="resume-lang-name font-weight-bold">{{ lang.name }}</span>
          <small class="text-muted font-weight-normal">({{lang.mastery}})</small>
        </li>
      </ul>
    </div>
  </section>
</template>