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
import sidebar from "/src/component/sidebar.vue"
import nav from "/src/component/nav.vue"
import ecom from "/src/component/ecom.vue"
import chart from "/src/component/chart.vue"
import order from "/src/component/order.vue"
import map from "/src/component/map.vue"
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
@import 'src/assets/scss/view/dash.scss';
</style>
