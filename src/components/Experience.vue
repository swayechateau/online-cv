<script>
export default {
  props: ["jobs"]
};
</script>
<template >
  <div class="resume-timeline position-relative">
    <article
      v-for="job in jobs"
      :key="job.position"
      class="resume-timeline-item position-relative pb-5"
    >
      <div class="resume-timeline-item-header mb-2">
        <div class="d-flex flex-column flex-md-row">
          <h3 class="resume-position-title font-weight-bold mb-1">{{ job.position}}</h3>
          <div class="resume-company-name ml-auto">{{ job.company }}</div>
        </div>
        <!--//row-->
        <div
          class="resume-position-time"
          v-text="`${job.started } - ${job.left ? job.left : 'Present' }`"
        ></div>
      </div>
      <!--//resume-timeline-item-header-->
      <div class="resume-timeline-item-desc">
        <p v-text="job.summary"></p>
        <template v-if="job.achievements">
          <h4 class="resume-timeline-item-desc-heading font-weight-bold">{{ job.achievements.title}}</h4>
          <p>{{ job.achievements.summary}}</p>
          <ul>
            <li v-for="achievement in job.achievements.list" :key="achievement">{{achievement}}</li>
          </ul>
        </template>
        <template v-if="job.tools">
          <h4 class="resume-timeline-item-desc-heading font-weight-bold">{{job.tools.title}}</h4>
          <ul class="list-inline">
            <li class="list-inline-item" v-for="tool in job.tools.list" :key="tool">
              <span class="badge badge-primary badge-pill">{{tool}}</span>
            </li>
          </ul>
        </template>
      </div>
      <!--//resume-timeline-item-desc-->
      <!--//resume-timeline-item-->
    </article>
  </div>
</template>