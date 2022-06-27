<template>
  <aside class="sidebar ">
    <div class="logo">
      <fa class="fa-home me-2" icon="home" />
      <h2 class="fw-bold d-inline-block m-0">H.Dashboard</h2>
    </div>
    <div  class="collapes-section list-style-type: none">
      <ul class="m-0">
        <li class="collapes-heading">
          <span>GENERAL</span>
        </li>
        <li class="collapes">
          <a href="" class="text-decoration-none d-flex align-items-center"
           @click.prevent="arrowDown($event)"
           >
            <fa class="collapes-fi" icon="dashboard" />
            <p class="d-inline-block">Dashboard</p>
            <fa class="collapes-arrow ms-auto ms-auto" icon="angle-right" />
          </a>
          <ul class="side-collapse">
            <li class="mb-3">
              <a href="https://meet.google.com/" target="_blank">
                <span>option 1</span>
              </a>
            </li>
           <li>
              <a href="">
                <span>optiion 2</span>
              </a>
            </li>
          </ul>
        </li>
        <li class="collapes">
          <a href="" class="text-decoration-none d-flex align-items-center"
           @click.prevent="arrowDown($event)"
           >
            <fa class="collapes-fi" icon="display" />
            <p class="d-inline-block">Layout</p>
            <fa class="collapes-arrow ms-auto" icon="angle-right" />
          </a>
          <ul class="side-collapse">
            <li class="mb-3">
              <a href="https://meet.google.com/" target="_blank">
                <span>option 1</span>
              </a>
            </li>
           <li>
              <a href="">
                <span>optiion 2</span>
              </a>
            </li>
          </ul>
        </li>
        <li class="collapes">
          <a href="" class="text-decoration-none d-flex align-items-center"
           @click.prevent="arrowDown($event)"
           >
            <fa class="collapes-fi" icon="folder" />
            <p class="d-inline-block">Pages</p>
            <fa class="collapes-arrow ms-auto" icon="angle-right" />
          </a>
          <ul class="side-collapse">
            <li class="mb-3">
              <a href="https://meet.google.com/" target="_blank">
                <span>option 1</span>
              </a>
            </li>
           <li>
              <a href="">
                <span>optiion 2</span>
              </a>
            </li>
          </ul>
        </li>

        <li class="collapes-heading">
          <span>ELEMENT</span>
        </li>
        <li class="collapes">
          <a href="" class="text-decoration-none d-flex align-items-center"
           @click.prevent="arrowDown($event)"
           >
            <fa class="collapes-fi" icon="gear" />
            <p class="d-inline-block">UI Element</p>
            <fa class="collapes-arrow ms-auto ms-auto" icon="angle-right" />
          </a>
          <ul class="side-collapse">
            <li class="mb-3">
              <a href="https://meet.google.com/" target="_blank">
                <span>option 1</span>
              </a>
            </li>
           <li>
              <a href="">
                <span>optiion 2</span>
              </a>
            </li>
          </ul>
        </li>
        <li class="collapes">
          <a href="" class="text-decoration-none d-flex align-items-center"
           @click.prevent="arrowDown($event)"
           >
            <fa class="collapes-fi" icon="chart-line" />
            <p class="d-inline-block">Charts</p>
            <fa class="collapes-arrow ms-auto" icon="angle-right" />
          </a>
          <ul class="side-collapse">
            <li class="mb-3">
              <a href="https://meet.google.com/" target="_blank">
                <span>option 1</span>
              </a>
            </li>
           <li>
              <a href="">
                <span>optiion 2</span>
              </a>
            </li>
          </ul>
        </li>
        <li class="collapes">
          <a href="" class="text-decoration-none d-flex align-items-center"
           @click.prevent="arrowDown($event)"
           >
            <fa class="collapes-fi" icon="boxes-stacked" />
            <p class="d-inline-block">Structure</p>
            <fa class="collapes-arrow ms-auto" icon="angle-right" />
          </a>
          <ul class="side-collapse">
            <li class="mb-3">
              <a href="https://meet.google.com/" target="_blank">
                <span>option 1</span>
              </a>
            </li>
           <li>
              <a href="">
                <span>optiion 2</span>
              </a>
            </li>
          </ul>
        </li>

        <li class="collapes">
          <a href="" class="text-decoration-none d-flex align-items-center"
           @click.prevent="arrowDown($event)"
           >
            <fa class="collapes-fi" icon="gavel" />
            <p class="d-inline-block">Widgests</p>
            <fa class="collapes-arrow ms-auto" icon="angle-right" />
          </a>
          <ul class="side-collapse">
            <li class="mb-3">
              <a href="https://meet.google.com/" target="_blank">
                <span>option 1</span>
              </a>
            </li>
           <li>
              <a href="">
                <span>optiion 2</span>
              </a>
            </li>
          </ul>
        </li>
        <li class="collapes">
          <a href="" class="text-decoration-none d-flex align-items-center"
           @click.prevent="arrowDown($event)"
           >
            <fa class="collapes-fi" icon="table-list" />
            <p class="d-inline-block">Tables</p>
            <fa class="collapes-arrow ms-auto" icon="angle-right" />
          </a>
          <ul class="side-collapse">
            <li class="mb-3">
              <a href="https://meet.google.com/" target="_blank">
                <span>option 1</span>
              </a>
            </li>
           <li>
              <a href="">
                <span>optiion 2</span>
              </a>
            </li>
          </ul>
        </li>
        <li class="collapes">
          <a href="" class="text-decoration-none d-flex align-items-center"
           @click.prevent="arrowDown($event)"
           >
            <fa class="collapes-fi" icon="pen" />
            <p class="d-inline-block">Form Stuff</p>
            <fa class="collapes-arrow ms-auto" icon="angle-right" />
          </a>
          <ul class="side-collapse">
            <li class="mb-3">
              <a href="https://meet.google.com/" target="_blank">
                <span>option 1</span>
              </a>
            </li>
           <li>
              <a href="">
                <span>optiion 2</span>
              </a>
            </li>
          </ul>
        </li>

        <li class="collapes-heading">
          <span>EXTRA</span>
        </li>

        <li class="collapes">
          <a href="" class="text-decoration-none d-flex align-items-center"
           @click.prevent="arrowDown($event)"
           >
            <fa class="collapes-fi" icon="envelope" />
            <p class="d-inline-block">Email</p>
            <span class="badges"> 4 Unread </span>
            <fa class="collapes-arrow ms-auto" icon="angle-right" />
          </a>
          <ul class="side-collapse">
            <li class="mb-3">
              <a href="https://meet.google.com/" target="_blank">
                <span>option 1</span>
              </a>
            </li>
           <li>
              <a href="">
                <span>optiion 2</span>
              </a>
            </li>
          </ul>
        </li>

        <li class="collapes">
          <a href="" class="text-decoration-none d-flex align-items-center"
           @click.prevent="arrowDown($event)"
           >
            <fa class="collapes-fi" icon="comments" />
            <p class="d-inline-block">Chat</p>
            <fa class="collapes-arrow ms-auto" icon="angle-right" />
          </a>
          <ul class="side-collapse">
            <li class="mb-3">
              <a href="https://meet.google.com/" target="_blank">
                <span>option 1</span>
              </a>
            </li>
           <li>
              <a href="">
                <span>optiion 2</span>
              </a>
            </li>
          </ul>
        </li>
        <li class="collapes ">
          <a href="" class="text-decoration-none d-flex align-items-center"
           @click.prevent="arrowDown($event)"
           >
            <fa class="collapes-fi" icon="location-dot" />
            <p class="d-inline-block">Maps</p>
            <fa class="collapes-arrow ms-auto" icon="angle-right" />
          </a>
          <ul class="side-collapse">
            <li class="mb-3">
              <a href="https://meet.google.com/" target="_blank">
                <span>option 1</span>
              </a>
            </li>
           <li>
              <a href="">
                <span>optiion 2</span>
              </a>
            </li>
          </ul>
        </li>
        <li class="milestone">
          <p class="m-0 mb-1">Milestone</p>
          <div class="progress">
            <div class="progress-bar" role="progressbar"  aria-valuenow="25" aria-valuemin="0" aria-valuemax="100"></div>
          </div>
        </li>
        <li class="release mb-5">
          <p class="m-0 mb-1">Release</p>
          <div class="progress mb-2">
            <div class="progress-bar" role="progressbar"  aria-valuenow="25" aria-valuemin="0" aria-valuemax="100"></div>
          </div>
        </li>
      </ul>
    </div>
  </aside>
</template>
<script>
export default {
    name:"side-bar",
    
  methods: {
    arrowDown(event) {
      const active = document.querySelectorAll(".show");
      active.forEach((node) => {
        if (node != event.currentTarget.parentNode) {
          node.classList.remove("show");
        }
      });
      event.currentTarget.parentNode.classList.toggle("show");
    }
  }
};
</script>
<style lang="scss" scoped>
@import '/src/assets/scss/component/sidebar.scss';
</style>
