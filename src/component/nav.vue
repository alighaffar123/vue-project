<template>
  <div class="nav-bar position-relative">
    <div class="container d-flex align-items-center h-100">
      <div class="menu col-auto me-4">
        <a href="">
          <fa icon="bars-staggered" />
        </a>
      </div>
      <div class="col-auto eng">
        <span class="pe-2"> English </span>
        <a href="">
          <fa icon="sort-down" />
        </a>
      </div>
      <div class="search col-auto">
        <a href="">
          <fa icon="search" />
        </a>
        <a class="bell" href="">
          <fa class="bell" icon="bell" />
            <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill ">
                8
            </span>
        </a>
      </div>
      <div class="envelope col-auto">
        <a class="abc" href="">
            <fa  class="abc" icon="envelope" />
            <span class="position-absolute top-0  badge rounded-pill ">
                8
            </span>
        </a>
      </div>
      <div class="bar col-auto">
        <a href="">
          <fa icon="bars" />
          <span class="position-absolute top-0  badge rounded-pill ">
                8
            </span>
        </a>
      </div>
      <div class="hungf col-auto ">
        <a href="">
          <img
            class="rounded-circle"
            src="../assets/img/navbar/profile.jpg"
            alt=""
          />
        </a>
        <span>Hungft</span>
        <a href="" class="ms-auto">
          <fa class="arrow" icon="sort-down" />
        </a>
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
@import "../assets/component/nav.scss";
</style>