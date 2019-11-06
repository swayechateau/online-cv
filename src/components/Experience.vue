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
        <p>
          As the Sole Director and Developer at KiTech Software, my
          responsibilties were vast, from managing the company to
          building
          websites for the company and clients.
          I have worked with multiple technologise as a result of customer demand
          or trailing for use within KiTech Software.
          Due to some NDA's signed I can not go into detail on alot of client
          projects, but I can on company and residential
          projects
        </p>
        <h4 class="resume-timeline-item-desc-heading font-weight-bold">Achievements:</h4>
        <p>Succured two contracts with Dimension Data (NTT).</p>
        <ul>
          <li>
            First Contract involved making a framework, where departments could
            create their own MS Bot without using a bit of code.
          </li>
          <li>Prototype was built in 1 week.</li>
          <li>Learned Node.js and MongoDB on the Job.</li>
          <li>
            Learned Azure platform and wrote a deploy to azure script for the
            project.
          </li>
        </ul>
        <h4 class="resume-timeline-item-desc-heading font-weight-bold">Technologies used:</h4>
        <ul class="list-inline">
          <li class="list-inline-item">
            <span class="badge badge-primary badge-pill">Vue JS / React</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-primary badge-pill">Php / Python</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-primary badge-pill">
              HTML / SASS /
              JavaScript
            </span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-primary badge-pill">
              MSSql / Mysql /
              PostgresSQL
            </span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-primary badge-pill">
              Grunt / Babel /
              Webpack
            </span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-primary badge-pill">
              Jenkins / Gitlab /
              Mattermost
            </span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-primary badge-pill">
              Node.js /
              MongoDB
            </span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-primary badge-pill">Laravel / Lumen</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-primary badge-pill">Pheonix Elixir</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-primary badge-pill">Electron</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-primary badge-pill">Socket I.O</span>
          </li>
        </ul>
      </div>
      <!--//resume-timeline-item-desc-->
      <!--//resume-timeline-item-->
    </article>
  </div>
</template>