<template>
  <header class="header-wrapper d-flex justify-content-between">
    <div class="left d-flex">
      <div class="logo">
        <picture>
          <source srcset="@/assets/images/logo.png" />
          <img width="120" src="@/assets/images/logo.png" alt="Logo" />
        </picture>
      </div>
      <div class="main-menu d-flex align-items-center ms-5">
        <ul class="main-menu-list">
          <li class="main-menu-list-item">
            <nuxt-link class="main-menu-list-item-link" to="/">Home</nuxt-link>
            <nuxt-link class="main-menu-list-item-link" to="/"
              >Find Job</nuxt-link
            >
            <nuxt-link class="main-menu-list-item-link" to="/">About</nuxt-link>
            <nuxt-link class="main-menu-list-item-link" to="/"
              >Contact Us</nuxt-link
            >
          </li>
        </ul>
      </div>
    </div>
    <div class="right d-flex">
      <div class="user-actions d-flex">
        <nuxt-link class="btn login me-2 sm" to="/">Login</nuxt-link>
        <nuxt-link class="btn light-btn job-post ms-2 sm" to="/">
          <!-- <i class="fas fa-play"></i> -->
          <span>Post Job</span>
        </nuxt-link>
      </div>
    </div>
  </header>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_mixins.scss";
.header-wrapper {
  padding: 0 6%;
  height: 80px;
  @include flex-center;
  position: absolute;
  top: 0;
  z-index: 1;
  width: 100%;
  .left {
    .main-menu {
      &-list {
        &-item {
          &-link {
            color: var(--white);
            padding: 10px;
          }
        }
      }
    }
  }
  .right {
    .user-actions {
      .btn.login {
        color: var(--white);
      }
      .btn-job-post {
      }
    }
  }
}
</style>
