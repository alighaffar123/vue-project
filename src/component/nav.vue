<template>
  <div class="nav-bar position-relative">
    <div class="container">
      <div class="navbar">
        <div class="d-flex nav-left">
          <div class="menu me-4">
            <a href="">
              <fa icon="bars-staggered" />
            </a>
          </div>
          <div class="eng">
            <span class="pe-2"> English </span>
            <a href="">
              <fa icon="sort-down" class="mb-1" />
            </a>
          </div>
          <a href="" class="ms-3">
            <fa class="" icon="search" />
          </a>
        </div>
       <div class="d-flex nav-right align-items-center">
         <div class="bell">
          <a class="bell-badge" href="">
            <fa class="bell-badge" icon="bell" />
            <span
              class="
                position-absolute
                top-0
                start-100
                translate-middle
                badge
                rounded-pill
              "
            >
              8
            </span>
          </a>
        </div>
        <div class="envelope ">
          <a class="abc" href="">
            <fa class="abc" icon="envelope" />
            <span class="position-absolute top-0 badge rounded-pill"> 8 </span>
          </a>
        </div>
        <div class="bar ">
          <a href="">
            <fa icon="bars" />
            <span class="position-absolute top-0 badge rounded-pill"> 8 </span>
          </a>
        </div>
        <div class="hungf d-flex align-items-center">
          <a href="">
            <img
              class="rounded-circle"
              src="../assets/img/navbar/profile.jpg"
              alt=""
            />
          </a>
          <span>Hungft</span>
          <a href="" class="ms-auto">
            <fa class="arrow mb-1" icon="sort-down" />
          </a>
        </div>
       </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "nav-bar",
};
</script>
<style lang="scss" scoped>
@import "/src/assets/scss/component/nav.scss";
</style>