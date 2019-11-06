<script>
export default {
  props: ["skills"]
};
</script>
<template>
  <section class="resume-section skills-section mb-5">
    <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">{{ skills.title }}</h2>
    <div class="resume-section-content">
      <div class="resume-skill-item" v-for="group in skills.groups" :key="group.title">
        <h4 class="resume-skills-cat font-weight-bold">{{group.title}}</h4>
        <ul class="list-unstyled mb-4" v-if="group.featured">
          <li class="mb-2" v-for="list in group.list" :key="list.skill">
            <div class="resume-skill-name">{{list.skill}}</div>
            <div class="progress resume-progress">
              <div
                class="progress-bar theme-progress-bar-dark"
                role="progressbar"
                :style="`width: ${list.mastery}%`"
                :aria-valuenow="list.mastery"
                aria-valuemin="0"
                aria-valuemax="100"
              ></div>
            </div>
          </li>
        </ul>
        <ul class="list-inline" v-else>
          <li class="list-inline-item" v-for="skill in group.list" :key="skill">
            <span class="badge badge-light">{{skill}}</span>
          </li>
        </ul>
      </div>
      <!--//resume-skill-item-->
    </div>
    <!--resume-section-content-->
  </section>
</template>