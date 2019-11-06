<script>
export default {
  props: ["content"],
  components: {
    Summary: () => import("./Summary"),
    Experience: () => import("./Experience"),
    Skills: () => import("./Skills"),
    Interests: () => import("./Interests"),
    Education: () => import("./Education"),
    Languages: () => import("./Languages")
  }
};
</script>
<template>
  <div class="resume-body p-5">
    <Summary :summary="content.summary" />
    <!--//summary-section-->
    <div class="row">
      <div class="col-lg-9">
        <section class="resume-section experience-section mb-5">
          <h2
            class="resume-section-title text-uppercase font-weight-bold pb-3 mb-3"
            v-text="content.experience.title"
          />
          <div class="resume-section-content">
            <Experience :jobs="content.experience.jobs" />
            <!--//resume-timeline-->
          </div>
        </section>
        <!--//experience-section-->
      </div>
      <div class="col-lg-3">
        <Skills :skills="content.skills" />
        <!--//skills-section-->
        <Education :education="content.education" />
        <!--//education-section-->
        <!-- <Achievements /> -->
        <!--//interests-section-->
        <Languages />
        <!--//language-section-->
        <Interests :interests="content.interests" />
        <!--//interests-section-->
      </div>
    </div>
    <!--//row-->
  </div>
</template>