<template>
  <footer>
    <div class="top-wrapper">
      <div class="container">
        <div class="top d-flex justify-content-between">
          <div class="newsletter d-flex justify-content-between w-100">
            <div class="left d-flex flex-column justify-content-center">
              <span class="newsletter-title">
                Get New Jobs Notification!
              </span>
              <span class="newsletter-description">
                Subscribe & get all related jobs notification.
              </span>
            </div>
            <div class="right d-flex w-50">
              <input type="text" class="lg w-100" placeholder="Enter your email" />
              <button class="btn dark-btn lg text-white">Subscribe</button>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="center-wrapper">
      <div class="container">
        <div class="center d-flex justify-content-between">
          <ul class="footer-menu-list">
            <span class="footer-menu-list-title">About Us</span>
            <li class="footer-menu-list-item">
              <nuxt-link class="footer-menu-list-item-link" to="/"
                >Home</nuxt-link
              >
            </li>
            <li class="footer-menu-list-item">
              <nuxt-link class="footer-menu-list-item-link" to="/"
                >Home</nuxt-link
              >
            </li>
            <li class="footer-menu-list-item">
              <nuxt-link class="footer-menu-list-item-link" to="/"
                >Home</nuxt-link
              >
            </li>
            <li class="footer-menu-list-item">
              <nuxt-link class="footer-menu-list-item-link" to="/"
                >Home</nuxt-link
              >
            </li>
          </ul>
          <ul class="footer-menu-list">
            <span class="footer-menu-list-title">Contact</span>
            <li class="footer-menu-list-item">
              <nuxt-link class="footer-menu-list-item-link" to="/"
                >Contact us</nuxt-link
              >
            </li>
            <li class="footer-menu-list-item">
              <nuxt-link class="footer-menu-list-item-link" to="/"
                >Phone</nuxt-link
              >
            </li>
            <li class="footer-menu-list-item">
              <nuxt-link class="footer-menu-list-item-link" to="/"
                >Shop Now</nuxt-link
              >
            </li>
            <li class="footer-menu-list-item">
              <nuxt-link class="footer-menu-list-item-link" to="/"
                >Home</nuxt-link
              >
            </li>
          </ul>
          <ul class="footer-menu-list">
            <span class="footer-menu-list-title">Corporate</span>
            <li class="footer-menu-list-item">
              <nuxt-link class="footer-menu-list-item-link" to="/"
                >Home</nuxt-link
              >
            </li>
            <li class="footer-menu-list-item">
              <nuxt-link class="footer-menu-list-item-link" to="/"
                >Home</nuxt-link
              >
            </li>
            <li class="footer-menu-list-item">
              <nuxt-link class="footer-menu-list-item-link" to="/"
                >Home</nuxt-link
              >
            </li>
            <li class="footer-menu-list-item">
              <nuxt-link class="footer-menu-list-item-link" to="/"
                >Home</nuxt-link
              >
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="bottom-wrapper">
      <div class="container">
        <div class="row">
          <div class="bottom d-flex justify-content-between">
            <div class="copyright">
              <span
                >© 2020 Work Stocks. Designd By PixelExperts All Rights
                Reserved</span
              >
            </div>
            <div class="social-media">
              <ul>
                <li>
                  <a href="#">Facebook</a>
                  <a href="#">Twitter</a>
                  <a href="#">Instagram</a>
                  <a href="#">Linkedin</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
footer {
  background-color: var(--dark);
  margin-top: 50px;
  .top-wrapper {
    background-color: var(--secondary);
    padding: 30px 0;
    .top{
      .newsletter{
        .left{
          .newsletter-title, .newsletter-description{
            color: var(--white);
          }
           .newsletter-title{
             font-size: 18px;
             font-weight: 700;
           }
        }
      }
    }
  }
  .center-wrapper {
    padding-top: 50px;
    padding-bottom: 50px;
    .center {
      .footer-menu-list {
        flex-direction: column;
        &-title {
          color: var(--white);
          font-size: 18px;
          margin-bottom: 20px;
        }
        &-item {
          &-link {
            color: var(--white);
            padding: 5px 0;
            display: block;
          }
        }
      }
    }
  }
  .bottom-wrapper {
    background-color: var(--dark);
    padding: 10px 0;
    .bottom {
      .copyright {
        span {
          font-size: 12px;
          color: var(--white);
        }
      }
      .social-media {
        ul {
          li {
            a {
              font-size: 12px;
              color: var(--light);
              padding: 0 10px;
            }
          }
        }
      }
    }
  }
}
</style>
