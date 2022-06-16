<template>
    <div class="ecommerce ">
        <div class="container">
            <h3>Ecommerce Overview</h3>
            <div class="grid-cards">
                <div class="sales shadow-sm ">
                    <div class="icon d-flex justify-content-center align-items-center">
                       <fa icon="scale-balanced" class="text-white fs-1" />
                    </div>
                    <div class="text bg-white">
                        <h4 class="fw-bold mb-1">
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
                        <h4 class="fw-bold mb-1">
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
                        <h4 class="fw-bold mb-1">
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
                        <h4 class="fw-bold mb-1">
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
@import '/src/assets/scss/component/ecom.scss';
</style>
