<template>
  <div class="hero">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 col-md-7">
          <div class="hero-content">
            <div class="hero-content-title">
              <h1>Find your job</h1>
            </div>
            <div class="hero-content-description">
              <h3>Find your job <span> in 10 minutes!</span></h3>
            </div>
            <div class="hero-content-action">
              <form>
                <div class="mb-3">
                  <input type="text" class="form-control lg" id="keyword" placeholder="Job Title or Keywords"/>
                </div>
                <div class="mb-3 d-flex">
                  <input type="text" class="form-control lg" id="location" placeholder="Search by Location"/>
                <button type="submit" class="btn light-btn lg w-25 ms-4">Find Job</button>

                </div>
                <div class="d-flex justify-content-end">

                </div>

              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="hero-content-img">
      <picture>
        <source srcset="@/assets/images/hero.png" />
        <img src="@/assets/images/hero.png" alt="Logo" />
      </picture>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.hero {
  position: relative;
  background-color: var(--primary);
  height: 100vh;
  &-content {
    margin-top: 40%;

    &-title {
      margin-bottom: 25px;
      h1{
        color: var(--white);
        font-size: 80px;
      }
    }
    &-description {
      margin-bottom: 35px;
      h3{
        font-size: 35px;
        color: var(--light);
        span{
          color: var(--secondary);
        }
      }
    }
    &-img {
      position: absolute;
      right: 50px;
      bottom: 0px;
      picture{
        img{
          max-width: 400px;
        }
      }
    }
  }
}
</style>
