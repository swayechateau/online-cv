<template>
  <div>
    <div id="nav">
      <b-navbar type="dark" variant="primary">
        <b-navbar-brand href="/">Resume</b-navbar-brand>
        <!--
        <b-navbar-nav class="ml-auto">
          <b-nav-item-dropdown :text="lang.toUpperCase()" right>
            <b-dropdown-item @click="updateLang('en')">English</b-dropdown-item>
            <b-dropdown-item @click="updateLang('ja')">Japanese</b-dropdown-item>
            <b-dropdown-item @click="updateLang('fr')">French</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>-->
      </b-navbar>
    </div>
    <div id="resume">
      <article class="resume-wrapper text-center position-relative">
        <div class="resume-wrapper-inner mx-auto text-left bg-white shadow-lg">
          <Header :header="resume[lang].header" />
          <Body :content="resume[lang].content" />
        </div>
      </article>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import content from "@/content.json";
export default {
  name: "home",
  components: {
    Header: () => import("@/components/Header.vue"),
    Body: () => import("@/components/Body.vue")
  },
  methods: {
    updateLang(val) {
      this.lang = val;
    }
  },
  data() {
    return {
      resume: content,
      lang: "en"
    };
  }
};
</script>
