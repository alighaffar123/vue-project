<template>
	<sidebar/>
    <div class="main-content">
        <!-- navbar -->
        <nav-bar />
        <div class="inner-content">
            <!-- ecommarce -->
            <ecom />
            <chart />
            <order />
            <map-component />
        </div>

    </div>

</template>
<script>
import sidebar from "../component/sidebar.vue"
import nav from "../component/nav.vue"
import ecom from "../component/ecom.vue"
import chart from "../component/chart.vue"
import order from "../component/order.vue"
import map from "../component/map.vue"
export default {
    name: "dash-bord",
        components: {
            'sidebar':sidebar,
            'nav-bar':nav,
            'ecom':ecom,
            'chart':chart,
            'order':order,    
            'map-component':map    
        }
}
</script>
<style lang="scss" scoped>
  @import "../assets/view/dash.scss";
</style>
