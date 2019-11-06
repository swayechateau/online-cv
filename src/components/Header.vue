<script>
export default {
  props: ["header"]
};
</script>
<template>
  <header class="resume-header pt-4 pt-md-0">
    <div class="media flex-column flex-md-row">
      <img class="mr-3 img-fluid picture mx-auto" :src="header.hero" alt />
      <div class="media-body p-4 d-flex flex-column flex-md-row mx-auto mx-lg-0">
        <div class="primary-info">
          <h1 class="name mt-0 mb-1 text-white text-uppercase">{{header.name}}</h1>
          <div class="title mb-3">{{header.position}}</div>
          <ul class="list-unstyled">
            <li class="mb-2">
              <a href="#">
                <i class="far fa-envelope fa-fw mr-2" data-fa-transform="grow-3"></i>
                {{header.email}}
              </a>
            </li>
            <!--<li><a href="#"><i class="fas fa-mobile-alt fa-fw mr-2" data-fa-transform="grow-6"></i>{{header.phone}}</a></li>-->
          </ul>
        </div>
        <!--//primary-info-->
        <div v-if="header.social_links" class="secondary-info ml-md-auto mt-2">
          <ul class="resume-social list-unstyled">
            <li class="mb-3" v-for="social in header.social_links" :key="social.title">
              <a :href="social.url">
                <span class="fa-container text-center mr-2">
                  <i :class="social.icon"></i>
                </span>
                {{social.title}}
              </a>
            </li>
          </ul>
        </div>
        <!--//secondary-info-->
      </div>
      <!--//media-body-->
    </div>
    <!--//media-->
  </header>
</template>