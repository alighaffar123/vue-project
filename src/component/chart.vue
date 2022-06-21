<template>
  <div class="products-sales">
    <div class="container">
      <div class="chart-grid">
        <div class="sale shadow-sm bg-white">
          <div class="navbar px-3">
            <div class="product">
              <a href="" class="text-decoration-none">
                <span class="fw-bold">PRODUCTS SALES</span>
                <fa icon="sort-down" class="arrow" />
              </a>
            </div>
            <div class="navbar-right">
              <div class="days">
                <a href="">
                  <span> Daily </span>
                </a>
                <a href="">
                  <span> Weekly </span>
                </a>
                <a href="">
                  <span> Monthly </span>
                </a>
                <a href="">
                  <span> Yearly </span>
                </a>
              </div>
              <a href="">
                <fa icon="chevron-down" class="chevron-down ms-3 fs-6" />
              </a>
              <a href="">
                <fa icon="xmark" class="xmark ms-3 fs-5" />
              </a>
            </div>
          </div>
          <div id="chart">
            <apexchart
              type="area"
              height="300"
              :options="chartOptions"
              :series="series"
            ></apexchart>
          </div>
        </div>
        <div class="team shadow-sm bg-white">
          <div class="navbar px-3">
            <span class="fw-bold">TEAM MEMBER</span>
            <a href="">
              <fa icon="xmark" class="xmark ms-auto fs-5" />
            </a>
          </div>
          <div class="name-list p-4">
            <div class="content d-flex align-items-center">
              <div class="me-3 crycle d-inline-block"></div>
              <span>Hung pham</span>
            </div>
            <div class="content d-flex align-items-center">
              <div class="me-3 crycle d-inline-block"></div>
              <span>Hung pham</span>
            </div>
            <div class="content d-flex align-items-center">
              <div class="me-3 crycle d-inline-block"></div>
              <span>Hung pham</span>
            </div>
            <div class="content d-flex align-items-center">
              <div class="me-3 crycle d-inline-block"></div>
              <span>Hung pham</span>
            </div>
          </div>
          <div class="view px-3">
            <span class="text">View All Member</span>
            <span class="badges">
              <a href="">
                <fa icon="plus" class="text-white fs-6" />
              </a>
            </span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import {  reactive } from "vue";
export default {
  name: "vue-chart",
    setup() {
        let series = reactive([
            {
            name: "Clothes",
            data: [31, 40, 28, 51, 42, 109, 100],
            },
            {
            name: "Electronics",
            data: [0, 140, 0, 100, 0, 170, 0],
            },
            {
            name: "shoes",
            data: [11, 32, 45, 32, 34, 52, 41],
            },
        ]),
        chartOptions = ({
            chart: {
                height: "300",
                type: "area",
            },
            dataLabels: {
                enabled: false,
            },
            stroke: {
                curve: "smooth",
            },
            xaxis: {
                type: "Day",
                categories: ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul"],
            },
        });

        return {
        series,
        chartOptions
        };
    },
};
</script>
<style lang="scss" scoped>
@import "/src/assets/scss/component/chart.scss";
</style>
