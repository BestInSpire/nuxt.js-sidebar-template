<template>
<div>

    <div class="sidebar" :class="{closed: sidebarClosed}">
      <div class="logo-details">
        <i class="bx bxl-vuejs"></i>
        <span class="logo_name">BestInSpire</span>
      </div>
      <ul class="nav-links">
        <li>
          <a href="#">
            <i class="bx bx-grid-alt"></i>
            <span class="link_name">Dashboard</span>
          </a>
          <ul class="sub-menu blank">
            <li><nuxt-link tag="a" class="link_name" to="#">Dashboard</nuxt-link></li>
          </ul>
        </li>
        <li>
          <div class="icon-link">
            <a href="#">
              <i class="bx bx-collection"></i>
              <span class="link_name">Category</span>
            </a>
          </div>
          <ul class="sub-menu blank">
            <li><nuxt-link tag="a" class="link_name" to="#">Category</nuxt-link></li>
          </ul>
        </li>
        <li>
          <div class="icon-link">
            <a href="#">
              <i class="bx bx-book-alt"></i>
              <span class="link_name">Posts</span>
            </a>
            <ul class="sub-menu blank">
              <li><nuxt-link tag="a" class="link_name" to="#">Posts</nuxt-link></li>
            </ul>
          </div>
        </li>
        <li>
          <a href="#">
            <i class="bx bx-pie-chart-alt-2"></i>
            <span class="link_name">Analytics</span>
          </a>
          <ul class="sub-menu blank">
            <li><nuxt-link tag="a" class="link_name" to="#">Analytics</nuxt-link></li>
          </ul>
        </li>
        <li>
          <a href="#">
            <i class="bx bx-line-chart"></i>
            <span class="link_name">Chart</span>
          </a>
          <ul class="sub-menu blank">
            <li><nuxt-link tag="a" class="link_name" to="#">Chart</nuxt-link></li>
          </ul>
        </li>
        <li>
          <div class="icon-link">
            <a href="#">
              <i class="bx bx-plug"></i>
              <span class="link_name">Plugins</span>
            </a>
            <ul class="sub-menu blank">
              <li><nuxt-link tag="a" class="link_name" to="#">Plugins</nuxt-link></li>
            </ul>
          </div>
        </li>
        <li>
          <a href="#">
            <i class="bx bx-compass"></i>
            <span class="link_name">Explore</span>
          </a>
          <ul class="sub-menu blank">
            <li><nuxt-link tag="a" class="link_name" to="#">Explore</nuxt-link></li>
          </ul>
        </li>
        <li>
          <a href="#">
            <i class="bx bx-history"></i>
            <span class="link_name">History</span>
          </a>
          <ul class="sub-menu blank">
            <li><nuxt-link tag="a" class="link_name" to="#">History</nuxt-link></li>
          </ul>
        </li>
        <li>
          <a href="#">
            <i class="bx bx-cog"></i>
            <span class="link_name">Settings</span>
          </a>
          <ul class="sub-menu blank">
            <li><nuxt-link tag="a" class="link_name" to="#">Settings</nuxt-link></li>
          </ul>
        </li>
        <li>
          <div class="profile-details">
            <div class="profile-content">
              <img
                src="https://avatars.githubusercontent.com/u/56519674?v=4"
                alt="profile"
              />
            </div>
            <div class="name-job">
              <div class="profile_name">BestInSpire</div>
              <div class="profile_job">Vue.JS Lover</div>
            </div>
            <i class="bx bx-log-out"></i>
          </div>
        </li>
      </ul>
    </div>
    <section class="home-section">
      <div class="home-content">
        <i class="bx bx-menu" @click="sidebarClicked"></i>
      </div>
    </section>
</div>
</template>

<script>
export default {
    data() {
        return {
            sidebarClosed: false,
        }
    },
    methods: {
        sidebarClicked() {
            this.sidebarClosed = !this.sidebarClosed
        }
    }
};
</script>

<style scoped></style>
