<template>
    <div class="ecommerce ">
        <div class="container">
            <h2>Ecommerce Overview</h2>
            <div class="grid-cards">
                <div class="sales shadow-sm ">
                    <div class="icon d-flex justify-content-center align-items-center">
                       <fa icon="scale-balanced" class="text-white fs-1" />
                    </div>
                    <div class="text bg-white">
                        <h4 class="fw-bold m-0">
                            $4,590
                        </h4>
                        <i>Last month sale</i>
                    </div>
                </div>
                <div class="order shadow-sm">
                    <div class="icon d-flex justify-content-center align-items-center">
                        <fa icon="arrow-down" class="text-white fs-1" />
                    </div>
                    <div class="text bg-white">
                        <h4 class="fw-bold m-0">
                            360
                        </h4>
                        <i>New order recceived</i>
                        
                    </div>
                </div>
                <div class="products shadow-sm ">
                    <div class="icon d-flex justify-content-center align-items-center">
                       <fa icon="cart-shopping" class="text-white fs-1 fs-1" />
                    </div>
                    <div class="text bg-white">
                        <h4 class="fw-bold m-0">
                            1,680
                        </h4>
                        <i>Total products</i>
                        
                    </div>
                </div>
                <div class="visitors shadow-sm  ">
                    <div class="icon d-flex justify-content-center align-items-center">
                       <fa icon="eye" class="text-white fs-1" />
                    </div>
                    <div class="text bg-white">
                        <h4 class="fw-bold m-0">
                            1,10,500
                        </h4>
                        <i>Unigue visiters</i>
                        
                    </div>
                </div>
            </div>
        </div>
        

    </div>
</template>
<script>
export default {
  name: "ecom-comp",
};
</script>
<style lang="scss" scoped>
@import "../assets/component/ecom.scss";
</style>
