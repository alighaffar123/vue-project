<template>
    <div class="chart ">
        <div class="container">
            <div class="chart-grid">
                <div class="sale shadow-sm bg-white">
                    <div class="navbar  px-3">
                        <div class="product">
                            <a href="" class="text-decoration-none">
                                <span class="fw-bold">PRODUCTS SALES</span>
                                <fa icon="sort-down" class="arrow"/>
                            </a>
                        </div>
                        <div class="navbar-right">
                            <div class="days">
                             <a href="">
                                <span>
                                    Daily
                                </span>
                            </a>
                            <a href="">
                                <span>
                                    Weekly
                                </span>
                            </a>
                            <a href="">
                                <span>
                                    Monthly
                                </span>
                            </a>
                            <a href="">
                                <span>
                                    Yearly
                                </span>
                            </a>                               
                            </div>
                            <a href="">
                                <fa icon="chevron-down" class="chevron-down ms-3 fs-6"/>
                                
                                

                            </a>
                            <a href="">
                                <fa icon="xmark" class="xmark ms-3 fs-5"/>
                            </a>
                        </div>
                    </div>
                    <div>
                        <div id="chart">
                            <apexchart type="area" height="300" :options="chartOptions" :series="series"></apexchart>
                        </div>
                    </div>
                </div>
                <div class="team shadow-sm bg-white" >
                    <div class="navbar px-3 ">
                        
                        <span class="fw-bold">TEAM MEMBER</span>
                        <a href="">
                                <fa icon="xmark" class="xmark ms-auto fs-5"/>
                        </a>
                    
                    </div>
                    <div class="name-list  p-4">
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
                        <span class="badges ">
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
export default {
    name: 'vue-chart',
  data(){
    return {
         series: [{
            name: 'series1',
            data: [31, 40, 28, 51, 42, 109, 100]
          },
          {
            name: 'series2',
            data: [ 0, 140, 0, 100, 0, 170,0]
          },
           {
            name: 'series3',
            data: [11, 32, 45, 32, 34, 52, 41]
          }],
          chartOptions: {
            chart: {
              height: 350,
              type: 'area'
            },
            dataLabels: {
              enabled: false
            },
            stroke: {
              curve: 'smooth'
            },
            xaxis: {
              type: 'datetime',
              categories: ["2018-09-19T00:00:00.000Z", "2018-09-19T01:30:00.000Z", "2018-09-19T02:30:00.000Z", "2018-09-19T03:30:00.000Z", "2018-09-19T04:30:00.000Z", "2018-09-19T05:30:00.000Z", "2018-09-19T06:30:00.000Z"]
            },
            tooltip: {
              x: {
                format: 'dd/MM/yy HH:mm'
              },
            },
          },
    }
  }
};
</script>
<style lang="scss" scoped>
@import '/src/assets/scss/component/chart.scss';
</style>
