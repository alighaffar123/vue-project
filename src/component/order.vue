<template>
  <div class="order">
    <div class="container">
      <div class="order-grid">
        <div class="recent shadow-sm bg-white">
          <div class="navbar px-3">
            <div class="product">
              <a href="" class="text-decoration-none">
                <span class="fw-bold">RECENT ORDER</span>
                <fa icon="sort-down" class="arrow" />
              </a>
            </div>
            <a href="">
              <fa icon="xmark" class="xmark ms-3 fs-5" />
            </a>
          </div>
          <div class="px-3 table-content overflow-auto">
            <table class="table">
              <tbody>
                <tr class="headding">
                  <th class="ps-0 text-start">Image</th>
                  <th class="text-start">Product Code</th>
                  <th class="text-start">Custmer</th>
                  <th class="text-start">Purchased On</th>
                  <th class="text-start">Status</th>
                  <th class="text-start">Tracking No#</th>
                </tr>
                <tr>
                  <td class="img ps-0">
                    <img
                      class=""
                      src="../assets/img/order/shirt1.jpeg"
                      alt=""
                    />
                  </td>
                  <td><span>3bn8d9s</span></td>
                  <td>
                    <span> salman </span>
                  </td>
                  <td>
                    <span> 27 sep 2015 </span>
                  </td>
                  <td>
                    <span class="paid badges"> Paid </span>
                  </td>
                  <td>
                    <span> #Gb58T8755675 </span>
                  </td>
                </tr>
                <tr>
                  <td class="img ps-0">
                    <img
                      class=""
                      src="../assets/img/order/shirt2.jpeg"
                      alt=""
                    />
                  </td>
                  <td>
                    <span> 3bn8d9s </span>
                  </td>
                  <td>
                    <span> salman </span>
                  </td>
                  <td>
                    <span> 27 sep 2015 </span>
                  </td>
                  <td>
                    <span class="failed badges"> Failed </span>
                  </td>
                  <td>
                    <span> #Gb58T8755675 </span>
                  </td>
                </tr>
                <tr>
                  <td class="img ps-0">
                    <img
                      class=""
                      src="../assets/img/order/shirt3.jpeg"
                      alt=""
                    />
                  </td>
                  <td>
                    <span> 3bn8d9s </span>
                  </td>
                  <td>
                    <span> salman </span>
                  </td>
                  <td>
                    <span> 27 sep 2015 </span>
                  </td>
                  <td>
                    <span class="pain badges"> Paid </span>
                  </td>
                  <td>
                    <span> #Gb58T8755675 </span>
                  </td>
                </tr>
                <tr>
                  <td class="img ps-0">
                    <img
                      class=""
                      src="../assets/img/order/shirt4.jpeg"
                      alt=""
                    />
                  </td>
                  <td>
                    <span> 3bn8d9s </span>
                  </td>
                  <td>
                    <span> salman </span>
                  </td>
                  <td>
                    <span> 27 sep 2015 </span>
                  </td>
                  <td>
                    <span class="failed badges"> Failed </span>
                  </td>
                  <td>
                    <span> #Gb58T8755675 </span>
                  </td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
        <div class="weakly-grid">
          <div class="income bg-white">
            <div id="chart">
              <apexchart
                type="area"
                height="123"
                :options="chartOptions"
                :series="series"
              ></apexchart>
            </div>
            <div class="celender p-2 pt-0 position-relative">
              <div class="position-absolute fw-bold d-inline-block text">
                <span>Weekly Income</span>
                <p class="fw-bold m-0">$10,000.00</p>
              </div>
              <div class="date">
                <fa icon="calendar" class="me-1 calendar" />
                <span class="fw-bold">15 SEP 2020</span>
                <fa icon="sort-down" class="ms-1 arrow" />
              </div>
            </div>
          </div>
          <div class="weather-grid bg-white">
            <div class="weather position-relative">
              <div class="top-left">
                <fa icon="location-dot" class="location text-white" />
                <span class="text-white"> Honoi, vietnam </span>
              </div>
              <div class="top-right">
                <span class="me-1">&#176;F</span>
                <span class="text-white">&#176;C</span>
              </div>
              <div class="bottom">
                <fa icon="cloud-sun" class="sun text-white" />
                <span class="text-white fw-bold degree">26&#176;</span>
                <span class="text-white text">partly cloudly</span>
              </div>
            </div>
            <div class="icon-grid">
              <div
                class="
                  mon
                  position-relative
                  d-flex
                  justify-content-center
                  flex-column
                  align-items-center
                "
              >
                <fa icon="cloud-sun" class="icon" />
                <p class="day m-0">MON</p>
              </div>
              <div
                class="
                  tue
                  position-relative
                  d-flex
                  justify-content-center
                  flex-column
                  align-items-center
                "
              >
                <fa icon="cloud" class="icon" />
                <p class="day m-0">TUE</p>
              </div>
              <div
                class="
                  wed
                  d-flex
                  justify-content-center
                  flex-column
                  align-items-center
                "
              >
                <fa icon="sun" class="icon" />
                <p class="day m-0">WED</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { reactive } from "vue";
export default {
  name: "vue-chart",
  setup() {
    let series = reactive([
        {
          name: "series1",
          data: [50, 60, 70, 80, 90, 109, 100],
        },
      ]),
    chartOptions = ({
        chart: {
          height: 123,
          type: "area",
        },
        dataLabels: {
          enabled: false,
        },
        stroke: {
          curve: "smooth",
        },
        xaxis: {
          type: "day",
          categories: ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
        },
        
      })
    return {
      series,
      chartOptions
    }
  }
};
</script>
<style lang="scss" scoped>
@import "/src/assets/scss/component/order.scss";
</style>