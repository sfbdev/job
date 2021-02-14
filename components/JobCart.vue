<template>
  <div class="job-cart d-flex justify-content-between">
    <div class="job-cart-left d-flex">
      <div class="image me-3">
        <picture>
          <source srcset="@/assets/images/company/company.png" />
          <img
            width="120"
            src="@/assets/images/company/company.png"
            alt="Logo"
          />
        </picture>
      </div>
      <div class="info">
        <div class="top d-flex">
          <div class="position-name me-4">
            <span>Front-end Developer</span>
          </div>
          <div class="badges">
            <span class="full-time">Full Time</span>
          </div>
        </div>
        <div class="center">
          <span class="company-name">Toronto Raptors</span>
        </div>
        <div class="bottom d-flex">
          <div class="salary d-flex flex-column me-3">
            <span class="key">Salary</span>
            <span class="value">$5k - $7.5k</span>
          </div>
          <div class="skills d-flex flex-column ms-3">
            <span class="key">Skills</span>
            <div class="values ">
              <span class="skill-badge">CSS3</span>
              <span class="skill-badge">HTML5</span>
              <span class="skill-badge">Vue</span>
              <span class="skill-badge">Git</span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="job-cart-right">
      <nuxt-link class="btn primary-btn apply-btn md" to="/apply">
        <span>Apply Now</span>
      </nuxt-link>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.job-cart {
  padding: 30px;
  box-shadow: 0px 5px 10px 0px rgb(130 136 184 / 20%);
  margin-bottom: 30px;
  border: 1px solid #c5c5c5;
  &:hover{
    border-color: var(--primary);
    cursor: pointer;
  }
  &-left {
    .info {
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      .top {
        .position-name {
          margin-bottom: -4px;
          span {
            font-size: 18px;
            font-weight: 700;
          }
        }
        .badges {
          .full-time{
            font-size: 12px;
            color: var(--white);
            background-color: var(--dark);
            padding: 2px 5px;
          }
        }
      }
      .center {
        margin-bottom: 10px;
        .company-name {
          font-size: 14px;
        }
      }
      .bottom {
        .salary {
          .key {
            font-size: 14px;
            font-weight: 700;
          }
          .value {
             font-size: 14px;
          }
        }
      }
      .skills {
        .key {
          font-size: 14px;
          font-weight: 700;
        }
        .values {
          .skill-badge {
            font-size: 12px;
            color: var(--white);
            background-color: var(--secondary);
            padding: 3px 8px;
            border-radius: 8px;

          }
        }
      }
    }
  }
  &-right{
    display: flex;
    align-items: center;
    .apply-btn{
      color: #ffffff;
    }
  } 
}
</style>
