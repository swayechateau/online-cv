<script>
export default {
  props: ["skills"]
};
</script>
<template>
  <section class="resume-section skills-section mb-5">
    <h2 class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3">{{ skills.title }}</h2>
    <div class="resume-section-content">
      <div class="resume-skill-item">
        <h4 class="resume-skills-cat font-weight-bold">Frontend</h4>
        <ul class="list-unstyled mb-4">
          <li class="mb-2">
            <div class="resume-skill-name">Vue Js</div>
            <div class="progress resume-progress">
              <div
                class="progress-bar theme-progress-bar-dark"
                role="progressbar"
                style="width: 92%"
                aria-valuenow="25"
                aria-valuemin="0"
                aria-valuemax="100"
              ></div>
            </div>
          </li>
          <li class="mb-2">
            <div class="resume-skill-name">React</div>
            <div class="progress resume-progress">
              <div
                class="progress-bar theme-progress-bar-dark"
                role="progressbar"
                style="width: 94%"
                aria-valuenow="25"
                aria-valuemin="0"
                aria-valuemax="100"
              ></div>
            </div>
          </li>
          <li class="mb-2">
            <div class="resume-skill-name">JavaScript</div>
            <div class="progress resume-progress">
              <div
                class="progress-bar theme-progress-bar-dark"
                role="progressbar"
                style="width: 96%"
                aria-valuenow="25"
                aria-valuemin="0"
                aria-valuemax="100"
              ></div>
            </div>
          </li>

          <li class="mb-2">
            <div class="resume-skill-name">HTML/CSS/SASS/LESS/STYLUS</div>
            <div class="progress resume-progress">
              <div
                class="progress-bar theme-progress-bar-dark"
                role="progressbar"
                style="width: 96%"
                aria-valuenow="25"
                aria-valuemin="0"
                aria-valuemax="100"
              ></div>
            </div>
          </li>
        </ul>
      </div>
      <!--//resume-skill-item-->

      <div class="resume-skill-item">
        <h4 class="resume-skills-cat font-weight-bold">Backend</h4>
        <ul class="list-unstyled">
          <li class="mb-2">
            <div class="resume-skill-name">Node.js</div>
            <div class="progress resume-progress">
              <div
                class="progress-bar theme-progress-bar-dark"
                role="progressbar"
                style="width: 92%"
                aria-valuenow="25"
                aria-valuemin="0"
                aria-valuemax="100"
              ></div>
            </div>
          </li>
          <li class="mb-2">
            <div class="resume-skill-name">Python/Django</div>
            <div class="progress resume-progress">
              <div
                class="progress-bar theme-progress-bar-dark"
                role="progressbar"
                style="width: 95%"
                aria-valuenow="25"
                aria-valuemin="0"
                aria-valuemax="100"
              ></div>
            </div>
          </li>
          <li class="mb-2">
            <div class="resume-skill-name">Ruby/Rails</div>
            <div class="progress resume-progress">
              <div
                class="progress-bar theme-progress-bar-dark"
                role="progressbar"
                style="width: 92%"
                aria-valuenow="25"
                aria-valuemin="0"
                aria-valuemax="100"
              ></div>
            </div>
          </li>
          <li class="mb-2">
            <div class="resume-skill-name">Elixir/Pheonix</div>
            <div class="progress resume-progress">
              <div
                class="progress-bar theme-progress-bar-dark"
                role="progressbar"
                style="width: 92%"
                aria-valuenow="25"
                aria-valuemin="0"
                aria-valuemax="100"
              ></div>
            </div>
          </li>
          <li class="mb-2">
            <div class="resume-skill-name">PHP</div>
            <div class="progress resume-progress">
              <div
                class="progress-bar theme-progress-bar-dark"
                role="progressbar"
                style="width: 86%"
                aria-valuenow="25"
                aria-valuemin="0"
                aria-valuemax="100"
              ></div>
            </div>
          </li>
          <li class="mb-2">
            <div class="resume-skill-name">Laravel/Lumen</div>
            <div class="progress resume-progress">
              <div
                class="progress-bar theme-progress-bar-dark"
                role="progressbar"
                style="width: 86%"
                aria-valuenow="25"
                aria-valuemin="0"
                aria-valuemax="100"
              ></div>
            </div>
          </li>
          <li class="mb-2">
            <div class="resume-skill-name">WordPress</div>
            <div class="progress resume-progress">
              <div
                class="progress-bar theme-progress-bar-dark"
                role="progressbar"
                style="width: 82%"
                aria-valuenow="25"
                aria-valuemin="0"
                aria-valuemax="100"
              ></div>
            </div>
          </li>
        </ul>
      </div>
      <!--//resume-skill-item-->

      <div class="resume-skill-item">
        <h4 class="resume-skills-cat font-weight-bold">Others</h4>
        <ul class="list-inline">
          <li class="list-inline-item">
            <span class="badge badge-light">DevOps</span>
          </li>

          <li class="list-inline-item">
            <span class="badge badge-light">Git</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-light">Gitlab</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-light">Confluence</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-light">BitBucket</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-light">Jira</span>
          </li>

          <li class="list-inline-item">
            <span class="badge badge-light">Docker</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-light">Jenkins</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-light">Unit Testing</span>
          </li>

          <li class="list-inline-item">
            <span class="badge badge-light">Slack</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-light">Ms Bot Framework</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-light">Dialog Flow</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-light">Wireframing</span>
          </li>

          <li class="list-inline-item">
            <span class="badge badge-light">Electron</span>
          </li>

          <li class="list-inline-item">
            <span class="badge badge-light">Centos 6/7</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-light">Ubuntu</span>
          </li>
          <li class="list-inline-item">
            <span class="badge badge-light">Windows 7/8/10</span>
          </li>
        </ul>
      </div>
      <!--//resume-skill-item-->
    </div>
    <!--resume-section-content-->
  </section>
</template>